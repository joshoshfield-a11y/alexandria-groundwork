# Canon 78 — the reconciled operator ledger

Date: 2026-10-12. Decision (user): **78 is canonical.** Source of record:
`lexicon_alexandria__1__13_nnqk.py` (78-operator runtime, generated 2026-07-25).

## Reconciliation

Three numberings existed across sessions:

| Source | Count | Notes |
|---|---|---|
| Codex v3.1 (`.docx`) | 72 named (F1–F18, D1–D18, R1–R18, T1–T18) + 72 mirror | Mythic name ↔ technical operator per slot |
| UT-ITD §II table (audited) | 72 | Different names again ("Primary Observer", …); audit verdicts in `audits/utitd-math/` |
| Lexicon runtime (`.py`) | **78**, unnamed indices 1–78 + 91 glyphs | **Canonical** |

Mapping: Codex v3.1 names joined to `.py` indices **by pillar order**
(Foundational indices 1,5,9,… ↔ F1–F18; Cosmic 2,6,10,… ↔ D1–D18;
Choral 3,7,11,… ↔ R1–R18; Transcendent 4,8,12,… ↔ T1–T18).
This mapping is a proposal documented here, not a discovered fact —
flagged per row so it can be corrected.

**Indices 73–78 are unnamed in every source.** They are the extension
slots: 2 Foundational (73, 77), 2 Cosmic (74, 78), 1 Choral (75),
1 Transcendent (76). Naming them is open work.

## Placeholder-parameter flag

Every `.py` operator carries λ, κ, H_max generated **from the index**:
λ=sin²(n), κ=log₂(n+1), H_max=binary-entropy(λ); pillar by n mod 4,
domain by (n−1) mod 12, related by n+7/+13/+29 mod 78.
These are **PLACEHOLDER** — deterministic scaffold values, not measured
or derived quantities. The ledger records them as-is so the scaffold
stays runnable, but no physical meaning is claimed for them.
Hardening an operator means replacing its placeholder row with the
7-field spec (see below), or explicitly marking it symbolic-only.

## The next phase: hardening

For each of the 78, one of three outcomes:

1. **ANCHOR** — the operator reproduces an established concept.
   Write the standard form, cite it, attach the measurable quantity
   with units, admit the relabel. No novelty claimed.
2. **DEFINE** — the operator names something real but undefined.
   Supply: state space, computable form, measurable quantity with
   units, and one prediction that differs from standard theory.
3. **SYMBOLIC-ONLY** — the operator is mythic/scaffold by design
   (perspective machinery for the Engine, not physics). Marked
   explicitly; no physical claims attached.

The 7-field spec per operator lives in `cores/OPERATOR_SPEC.md`.
Worked exemplars: `lexicon/exemplars/` (Frequency as ANCHOR,
Vigil Flame as DEFINE-attempt with the delta stated or declined).

## Files

- `lexicon/canon-78.csv` — the ledger (idx, pillar, domain, codex_name,
  technical, placeholder λ/κ/H_max)
- `lexicon/CANON-78.md` — this file
- `lexicon/exemplars/` — worked hardening exemplars establishing the template
