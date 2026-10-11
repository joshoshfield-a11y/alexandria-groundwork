# RGH Implementation Audit

Source: `joshoshfield-a11y/RGH-Reality-Grounding-Harness`, main branch. Five chambers + five validators. Audited 2026-10-10 by reading the code (not just the README).

## Verdict up front

The architecture is a legitimate falsification pipeline design, but **the shipped code does not run end-to-end as documented**, and several chambers are stubs or keyword heuristics rather than the tests their names promise. Grade of the implementation as shipped: **PARTIAL, with blocking defects**. Findings below, ordered by severity.

## Blocking defects

1. **Chamber 2 and Chamber 3 cannot import.** Both do `from rgh_chamber1_external_measurement import ...`, but no such module exists — the file is `Chamber1.py`. Chamber 5 instead does `from Chamber1 import ClaimResult`. Two different import conventions, one of them broken. The pipeline has never executed as a pipeline in this state. (Fix: rename imports to `Chamber1`; add a smoke test that imports all five chambers.)
2. **Doc/code drift on verdicts.** The README advertises verdicts like PHYSICALLY_GROUNDED; the code's enums produce MEASURABLE_UNTESTED / MEASURABLE_CONFIRMED / UNMEASURABLE / NOT_A_MEASURABLE_CLAIM. No code path ever *confirms* measurability — there is no dataset-checking step — so MEASURABLE_CONFIRMED is unreachable and PHYSICALLY_GROUNDED does not exist in code. A verdict the code cannot emit is marketing, not instrumentation.

## Chamber-by-chamber

- **Chamber 1 (External Measurement Gate)** — keyword-list classifier. Ten framework-vocab translations, 16 measurable keywords, 11 unmeasurable keywords, 3 physics constants. Fail-closed ordering is sound design, but: the vocab map is tiny (any new framework term sails through untranslated), and "MEASURABLE_UNTESTED" is a terminal state — nothing downstream ever tests it. Grade: PARTIAL (design) / SCHEMATIC (coverage).
- **Chamber 2 (Falsifiability Stress Test)** — generates an adversarial prediction from regexes: contains a digit → "measure the quantity"; contains a causal word → "withhold the cause". Any numerate sentence is thereby "falsifiable", which confuses *having a number* with *being testable*. It also never executes the test — SURVIVED means "no contradiction found in this pass", i.e. it survived nothing. The right question (can it *reject* a sophisticated unfalsifiable claim?) is untested. Grade: SCHEMATIC.
- **Chamber 3 (Independent Replication)** — extracts a "stripped pipeline" only if the claim contains one of five verbs (form, aggregate, requires, model, propagat), then emits a canned two-line function. The "fresh independent execution" compares a hardcoded string against itself. This chamber demonstrates the *shape* of a replication protocol, not a replication. Grade: SCHEMATIC.
- **Chamber 4 (Domain-Crossing Consistency)** — the strongest idea in the repo (random domain-pair sampling vs cherry-picking), but ships with exactly one operator: `mod_13_reduction`. A consistency auditor that can only test "x mod 13" cannot audit the 72-operator registry it is meant to check. Grade: PARTIAL (design) / SCHEMATIC (implementation).
- **Chamber 5 (Synthesis)** — `check_thermodynamics` hardcodes `field_gradient = 1.0e10` with the comment "Needs to be derived from claim", and gates on the magic number 433000. The thermodynamic guardrail is a placeholder wearing a lab coat. Grade: SCHEMATIC.

## Adversarial probes (to run once imports are fixed)

1. Feed Chamber 1 a sophisticated unfalsifiable claim with no mythic keywords, e.g. a SOP-CHRONO-001-style retrocausality claim phrased in physics vocabulary. Does it pass as MEASURABLE_UNTESTED? (Prediction: yes — the keyword lists can't catch it.)
2. Feed Chamber 2 a numerate-but-vacuous claim ("the field strength is 7 resonance units"). Does it return FALSIFIABLE_AND_SURVIVED? (Prediction: yes — digit present, no contradiction check possible.)
3. Run the full pipeline on 10 UT-ITD claims end to end. Record how many reach each terminal state. That table is the real audit result; everything above is the hypothesis going in.

## What would promote this repo

- Fix the imports; add a CI smoke test importing all chambers.
- Replace at least one keyword heuristic with a real check (e.g. Chamber 1: require a named unit + quantity + instrument class before MEASURABLE_*).
- Give Chamber 4 three real operators from the 72 (with OPERATOR_SPEC specs from cores/) instead of mod-13.
- Derive Chamber 5's field gradient from the claim or delete the gate; a hardcoded guardrail is worse than none because it looks like safety.
