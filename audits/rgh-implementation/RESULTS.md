# RGH Audit — Execution Results

Date: 2026-10-10. Method: cloned `RGH-Reality-Grounding-Harness` main, fixed the two broken imports in a work copy (patch: `rgh-import-fix.patch`), ran Chambers 1–4 on 10 real UT-ITD claims plus 3 adversarial probes. Upstream repo untouched — fixes are offered, not pushed.

## Setup

- `import Chamber2` / `import Chamber3` failed before the fix: `ModuleNotFoundError: No module named 'rgh_chamber1_external_measurement'`. After the one-line-per-file fix, all five chambers import.
- Chamber 5 was read but not executed end-to-end: its thermodynamic gate hardcodes `field_gradient = 1.0e10` ("Needs to be derived from claim"), so executing it would only demonstrate the placeholder.

## 10 UT-ITD claims through Chambers 1 → 2

| ID | Claim (abridged) | Chamber 1 | Chamber 2 | What actually drove the verdict |
|---|---|---|---|---|
| U01 | SOP-COG-001: 3–7x increase in pattern recognition | NOT_A_MEASURABLE_CLAIM | gated | The doc's most quantitative claim fails the gate — no keyword for "increase", "times", or percent |
| U02 | SOP-CHRONO-001: retrocausal reframing via quantum eraser | MEASURABLE_UNTESTED | FALSIFIABLE_AND_SURVIVED | "Falsifiable" because the SOP label **CHRONO-001 contains digits** |
| U03 | HRV increase >5% | MEASURABLE_UNTESTED | FALSIFIABLE_AND_SURVIVED | Passed only via substring "signal" in "**signal**ing" |
| U04 | MAAS increase >10% | NOT_A_MEASURABLE_CLAIM | gated | Same keyword gap as U01 |
| U05 | Observer field collapses potential into observed reality | NOT_A_MEASURABLE_CLAIM | gated | The doc's central metaphysical claim doesn't register as a claim at all |
| U06 | Information is conserved across all domains | NOT_A_MEASURABLE_CLAIM | gated | — |
| U07 | Deleted timelines stored in the dissipative well | NOT_A_MEASURABLE_CLAIM | gated | — |
| U08 | Amplitude grows as damping reaches zero (real physics) | NOT_A_MEASURABLE_CLAIM | gated | **"rapid" contains the substring "api"** → misfiled as an engineering/API spec |
| U09 | Metcalfe's law (n² value scaling) | MEASURABLE_UNTESTED | UNFALSIFIABLE | A genuinely testable textbook claim graded unfalsifiable — phrasing had no digits |
| U10 | Syntropy generated when resonance exceeds noise | NOT_A_MEASURABLE_CLAIM | gated | — |

## Adversarial probes

- **P1** — retrocausality phrased in physics vocabulary, no digits: C1 MEASURABLE_UNTESTED → C2 **UNFALSIFIABLE**. Chamber 2 caught it — but U02 shows the same claim with an "001" label would have survived. The difference between UNFALSIFIABLE and FALSIFIABLE_AND_SURVIVED is whether the text contains a digit.
- **P2** — "The measured field value is 7 resonance units" (numerate but vacuous): C1 MEASURABLE_UNTESTED → C2 **FALSIFIABLE_AND_SURVIVED**. A meaningless number survives; the chamber cannot distinguish vacuous numeracy from a real measurement claim.
- **P3** — mythic language ("truth requires no proof"): C1 **UNMEASURABLE**. The one thing the keyword lists reliably do.

## Chamber 3

All sampled claims → NOT_APPLICABLE_NO_PIPELINE. Pipeline extraction fires only on five verbs (form, aggregate, requires, model, propagat); descriptive claims — i.e. nearly every claim in the UT-ITD doc — are ineligible by construction.

## Chamber 4

Ran the repo's own shipped demo: **6/6 domain pairs flagged INCONSISTENT_CHERRY_PICK_RISK**, including GR physics vs Newtonian physics. With mod-13 as the only operator, "consistency" means "the two chosen numbers happen to be congruent mod 13" — numerology, not a test of whether an operator holds across domains. The demo's own numbers were picked to look meaningful and still fail.

## Bottom line

The audit hypothesis in AUDIT.md is confirmed and sharpened: the pipeline's verdicts are driven by **textual accidents** — digit presence, substring matches ("api" in "rapid", "signal" in "signaling") — not by the epistemic properties the chamber names promise. FALSIFIABLE_AND_SURVIVED can mean "the SOP label contained 001". A harness that cannot tell U09 (Metcalfe's law) from P2 (7 resonance units) is not yet a falsification instrument.

## Recommended fixes (in priority order)

1. Apply `rgh-import-fix.patch`; add a CI smoke test importing all five chambers.
2. Replace substring keyword matching with token matching ("api" must not fire inside "rapid").
3. Chamber 1: require quantity + unit + instrument class before any MEASURABLE_* verdict; add keywords for increase/decrease/percent/change so U01/U04-style claims pass the gate they were built for.
4. Chamber 2: the digit heuristic must go — replace with "does the claim name a quantity with a unit and a comparison?", and actually attempt the comparison where data exists instead of declaring SURVIVED.
5. Chamber 4: add real operators from the 72 (with OPERATOR_SPEC specs) instead of mod-13; until then, quarantine its verdicts.
6. Chamber 5: derive the field gradient from the claim or delete the gate — a hardcoded guardrail is worse than none.
