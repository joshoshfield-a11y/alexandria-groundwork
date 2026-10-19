# Alexandria Proof

The hardening layer for the Alexandria cores. Not a new philosophy — an evidence ledger.

## Why this repo exists

An external review (ChatGPT, 2026-10-10) read the portfolio, the UT-ITD document, and the RGH repository and landed here:

> "The right way to resolve that question is to inspect the equations, run the code, and test the predictions — not to accept or reject the philosophy based on its terminology."

This repo does exactly that, for the three cores of the Alexandria program:

1. **The 72 operators** — are the mathematical mappings derivations or decorations?
2. **The RGH pipeline** — does the falsification harness actually work when you run it?
3. **The Location Baseline Awareness protocol** — does it survive contact with a controlled study design?

## Layout

- `cores/` — the formal cores under test, and the spec each one must meet to count as hardened. The machinery itself lives in [`alexandria-engine`](https://github.com/joshoshfield-a11y/alexandria-engine); this repo holds the evidence about it, not a second copy of it.
- `audits/utitd-math/` — equation-by-equation reconstruction of the UT-ITD document. Every equation gets one of four grades: DEFINED, SCHEMATIC, REPRODUCES-ESTABLISHED, or INTRODUCES-NEW. The question that matters: does anything here predict differently than existing models?
- `audits/rgh-implementation/` — chamber-by-chamber audit of the actual RGH code. Does it run? Can it reject a sophisticated-sounding unfalsifiable claim?
- `experiments/location-baseline-awareness/` — the awareness protocol converted into a preregistered controlled study, using the document's own metrics (MAAS, HRV).
- `references/` — source links and the motivating assessment.

## Ground rules

1. Every finding is graded: **VERIFIED** (ran it, saw it), **PARTIAL** (some evidence, gaps named), **SCHEMATIC** (described but not defined), **ANALOGY** ( evocative, not mechanistic), **UNTESTED** (no data either way).
2. A mapping between a named concept and a mathematical symbol is not a derivation. Say which one it is.
3. The framework is allowed to fail here. A failed test is a result, not an insult.
4. Metaphysical claims stay out of the machinery. This repo tests the machinery.
