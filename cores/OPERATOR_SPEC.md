# Operator Hardening Spec

Every one of the 72 operators must carry this spec before it counts as hardened. This is the external review's challenge, formalized: a mapping to a mathematical symbol is not a derivation until it answers these.

## Required fields per operator

1. **Name** (plain-language, per the v0.6.0 grounded register) + `codexName` (provenance only).
2. **Variables** — what participates? Name them; give domains and units where applicable.
3. **Mechanism** — if it claims feedback: sign (positive/negative), gains, time delays. If it claims resonance: what oscillates, at what frequency, with what Q. No mechanism, no operator — it stays ANALOGY.
4. **Predicted effect on system stability/behavior** — stated quantitatively where possible, qualitatively with a named observable otherwise.
5. **Conventional analogue** — the closest established concept (control theory, graph theory, information theory, thermodynamics). If none exists, say so explicitly.
6. **Delta claim** — what does this operator predict that the conventional analogue does not? This is the load-bearing field. "New vocabulary for a familiar mechanism" is a legitimate finding, not a failure — but it must be labeled as such.
7. **Falsifier** — a concrete observation that would demote this operator. No falsifier, no promotion past SCHEMATIC.

## Worked example of the bar (operator 15, Feedback Loop)

- As written: "Closed-Loop Gain (A_CL) / Recirculation: Self-amplifying information cycles."
- To harden: specify the loop variables, whether the gain is positive or negative feedback, the delay in the loop, the stability criterion (e.g. Nyquist / gain margin), and one prediction that differs from a textbook closed-loop analysis. If there is none, the honest grade is REPRODUCES-ESTABLISHED — useful as vocabulary, not as new physics.

## Status

The 72 operators are inventoried in `../audits/utitd-math/operators-audit.csv` with a first-pass textual auto-tag (54 SYMBOLIC-ONLY, 18 ESTABLISHED-CONCEPT). Reviewer verdicts are open. This spec is the checklist each verdict must satisfy.
