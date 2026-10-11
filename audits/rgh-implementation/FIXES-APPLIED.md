# RGH v0.2 — Fixes Applied Upstream

Date: 2026-10-10. All seven recommendations from RESULTS.md were implemented and pushed to `RGH-Reality-Grounding-Harness` main. `tests/test_chambers.py` (9 tests) passes.

## What changed

1. Import fix + smoke test (Chambers 2–3 imported a nonexistent module).
2. Token-based keyword matching — "rapid" no longer matches "api".
3. `MEASURABLE_QUANTIFIED` (number + unit/scale) vs `MEASURABLE_UNTESTED`; change-words added so quantitative claims pass the gate.
4. Digit heuristic removed — falsifiability needs quantity + comparison or a withholdable cause; adversarial prediction cites the actual quantity.
5. No auto-SURVIVED — `FALSIFIABLE` (pending) until evidence is supplied via `evidence_by_id`.
6. Chamber 4: `operator_name` required; registry with `identity` (control), `metcalfe_scaling` (defined), `mod_13_reduction` (LEGACY, marked numerological).
7. Thermodynamic gate honest — free-energy language is a violation, named energy quantity is OK, everything else is `CANNOT_ASSESS`. No hardcoded gradient.
8. README rewritten: the verdict list now matches the enums the code actually emits.

## Re-run: same 10 claims + probes under v0.2

| ID | v0.1 verdict | v0.2 verdict | Assessment |
|---|---|---|---|
| U01 3–7x pattern recognition | gated (no keyword) | QUANTIFIED → FALSIFIABLE | Fixed — the doc's own quantitative claim now passes |
| U02 retrocausal SOP | auto-SURVIVED (digits in label) | → UNFALSIFIABLE | Fixed — correctly identified, no escape hatch |
| U03 HRV >5% | SURVIVED ("signal" in "signaling") | QUANTIFIED → FALSIFIABLE | Fixed — pending evidence, as it should be |
| U04 MAAS >10% | gated (no keyword) | QUANTIFIED → FALSIFIABLE | Fixed |
| U05 observer collapse | gated | gated | Correct — no measurable content as phrased |
| U06/U07/U10 | gated | gated | Correct |
| U08 resonance/damping→0 | misfiled as engineering ("api" in "rapid") | UNTESTED → FALSIFIABLE (causal branch) | Fixed |
| U09 Metcalfe's law | UNFALSIFIABLE (no digits) | UNFALSIFIABLE (no quantity named) | Honest — "scales with the square" names a relationship but no measurable metric; routed with a reformulate action item |
| P1 sophisticated retrocausality | UNFALSIFIABLE | UNFALSIFIABLE | Correct, stable across versions |
| P2 vacuous "7 resonance units" | auto-SURVIVED | FALSIFIABLE | Fixed |
| P3 mythic | UNMEASURABLE | UNMEASURABLE | Correct, stable |
| P4 free energy 500W | — (new probe) | QUANTIFIED → FALSIFIABLE; thermo gate → VIOLATION | Correct |

Synthesis on the suite: `NEEDS_EVIDENCE` by default; `PHYSICALLY_GROUNDED` only when a claim survives against supplied evidence (demonstrated with U03 measured at 6.1%); `UNFALSIFIABLE_ROUTED` for U09 with a reformulate-or-relabel action item.

## Remaining limitations (honest)

- Quantity extraction is first-match and English-only; "3 to 7 times" records as "7 times".
- Chamber 3 still only fires on procedural verbs — descriptive claims are ineligible by construction (correct for a replication chamber, but it means most UT-ITD claims can't reach it).
- `UNFALSIFIABLE` for U09 shows the chamber grades claims *as stated* — a true law phrased without a metric gets routed. That's the right conservatism for a fail-closed harness, but the action items matter more than the flag.
