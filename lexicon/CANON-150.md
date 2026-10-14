# Canon 150 — mirror-expansion proposal (WS4)

Date: 2026-10-14. Status: **PROPOSAL — not canon.** Nothing here is
merged, pushed, or written into `canon-78.csv`. The user decides.

## Decision

The 72 mirror/shadow operators of Codex v3.1 §11 ("The Mirror Canon —
72 Shadow/Constraint Operators", the Nocturna Grimoire) become indices
**79–150**, each paired to its primal by the rule:

> **mirror of canon idx N → canon idx N+78** (N = 1…72)

The extension slots (idx 73–78: Empty Root, Duality, Sympathetic
Resonance, Channel Capacity, Terminal State, Cosmic Horizon) have **no
mirrors** — the docx pairs shadows only with the 72 primals
(F1–F18, D1–D18, R1–R18, T1–T18), i.e. canon idx 1–72. That is why the
mirror block is exactly 72 wide and starts at 79.

Because canon indices interleave pillars (Foundational 1,5,9,…; Cosmic
2,6,10,…; Choral 3,7,11,…; Transcendent 4,8,12,…), the 18 *named*
shadows S1–S18 land non-contiguously: S1→79, S2→83, S3→87, …,
S18→147 (mirror idx = 4(k−1)+79 for S_k). Each mirror inherits its
primal's pillar and domain (the shadow is isomorphic to its primal's
pillar, per §11).

## Source fidelity — the naming gap (read this first)

Codex v3.1 names only **18** of the 72 shadows individually (S1–S18,
the Foundational mirrors; table in §11 with shadow name + primal +
constraint function). For the remaining 54 (mirrors of the Cosmic,
Choral, and Transcendent primals), §11 asserts only that "each of the
54 remaining generative operators (D1–D18, R1–R18, T1–T18) possesses
an isomorphic shadow constraint" — **no individual names are given**
anywhere in the document (verified by full-text search of the
pandoc-extracted source).

Resolution (documented, reversible): the 54 unnamed mirrors are named
by transparent proposal convention — **"Shadow of \<primal codex
name\>"** — and every affected file and CSV row marks the name as
constructed, never as source material. Their `technical` fields are
likewise *derived* constraint readings (the regulatory/deconstructive
dual of the primal's core function), labeled "(derived constraint)".
The 18 named shadows use the docx's shadow names and constraint
functions verbatim.

No mythic names were invented for the 54. If the user (or a later
source) supplies real names, the convention names swap out
mechanically.

## Pairing table (mirror idx → primal idx → shadow name)

| Mirror | Primal | Shadow name | Source |
|---|---|---|---|
| 79 | 1 | Blind Seer | §11 named (S1) |
| 83 | 5 | Ouroboros Bite | §11 named (S2) |
| 87 | 9 | Fracture Line | §11 named (S3) |
| 91 | 13 | Venom Lock | §11 named (S4) |
| 95 | 17 | False Mirror | §11 named (S5) |
| 99 | 21 | Void Lattice | §11 named (S6) |
| 103 | 25 | Babel Fall | §11 named (S7) |
| 107 | 29 | Stillbirth | §11 named (S8) |
| 111 | 33 | Barren Core | §11 named (S9) |
| 115 | 37 | Frost Star | §11 named (S10) |
| 119 | 41 | River Lethe | §11 named (S11) |
| 123 | 45 | Amorphous | §11 named (S12) |
| 127 | 49 | Gordian Cut | §11 named (S13) |
| 131 | 53 | Ariadne Abandoned | §11 named (S14) |
| 135 | 57 | Gradient Flatline | §11 named (S15) |
| 139 | 61 | Dissonance Storm | §11 named (S16) |
| 143 | 65 | Malthusian Collapse | §11 named (S17) |
| 147 | 69 | Time Abyss | §11 named (S18) |
| 80,84,88,92,96,100,104,108,112,116,120,124,128,132,136,140,144,148 | 2,6,10,…,70 | Shadow of \<Cosmic primal\> | convention |
| 81,85,89,93,97,101,105,109,113,117,121,125,129,133,137,141,145,149 | 3,7,11,…,71 | Shadow of \<Choral primal\> | convention |
| 82,86,90,94,98,102,106,110,114,118,122,126,130,134,138,142,146,150 | 4,8,12,…,72 | Shadow of \<Transcendent primal\> | convention |

(Full per-row listing is in `canon-150-proposal.csv`, `mirror_of` column.)

## Hardening results

All 72 mirrors hardened to the batch template (250–450 words; 7-field
spec; placeholder λ/κ/H_max computed mechanically for n=79–150 as
λ=sin²(n), κ=log₂(n+1), H_max=binary-entropy(λ), and retired in-file;
exact `Verdict:` footer; `Grounded:` line from the start). Output:
`mirrors/out/79-…-anchor.md` through `150-…-symbolic.md`.

**Verdict distribution: 71 ANCHOR / 0 DEFINE / 1 SYMBOLIC-ONLY.**

- The high ANCHOR rate is expected, not suspicious: mirrors are *by
  construction* the null-space/constraint duals of anchored concepts,
  and each file anchors to a real, named, standard concept (decoherence,
  destructive interference, Landauer erasure, buckling, avoided
  crossing, open-loop control, evanescent waves, …). No novelty is
  claimed anywhere; no DEFINE was warranted (no mirror states a new
  falsifiable hypothesis).
- The single SYMBOLIC-ONLY is idx 149, "Shadow of Choral Closure" —
  the mirror of a symbolic-only primal (idx 71). Forcing a physical
  anchor there (Gödel incompleteness was considered and rejected)
  would have been inflation. Its honesty is inherited lack of physics.
- Thin/interpretive anchors are flagged **in-file** in the delta
  assessment, not hidden: idx 99 (Void Lattice — narrowed to
  percolation), 108 (Boundaries — absorbing BCs), 109 (Null States —
  vacuum non-emptiness), 114/124 (zero-vector/rest nulls), 125
  (Harmonic Means — bottleneck reading), 131 (Ariadne — path loss),
  144 (Light — spacelike separation, with explicit refusal of any
  superluminal reading), 148 (Cosmic Closure — inherits primal
  thinness). Conjecture-labeled anchors: 102 (cosmic censorship),
  110 (SUSY cancellation). Shared anchor declared: 93/141 (heterarchy).
  Guardrailed: 134 (local negentropy only — no 2nd-law violation
  claimed).

## Files

- `canon-150-proposal.csv` — 150 rows: the 78 canon rows unchanged
  (plus empty `mirror_of`) + 72 mirror rows with `mirror_of` = N−78.
- `mirrors/out/` — 72 hardened exemplar files.
- Build script (reproducible): `/tmp/build_mirrors.py` with data in
  `/tmp/mirror_data_{1,2,3,4}.py` — regenerates everything, verifies
  word counts (observed 318–403), footers, Grounded lines,
  placeholders, filename format, and the CSV mapping.

## Open for the user's word

1. Adopt or reject the N+78 numbering and the "Shadow of X"
   convention names (rename any/all).
2. Whether the mirror block enters the Engine integration (WS2's
   78-operator work is unaffected — this proposal only appends).
3. Push of any of this to a repo — not done, not queued.
