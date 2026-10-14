# Exemplar — ANCHOR: idx 83, "Ouroboros Bite" (Mirror of idx 5, "Spiral Tongue")

Date: 2026-10-14. Mirror-canon proposal (WS4): the shadow dual of primal idx 5 "Spiral Tongue" (recursion), named in Codex v3.1 §11 as S2. Where recursion builds by self-reference with a base case, the Ouroboros Bite is recursion that never reaches one.

## Canon row

- idx 83 · Foundational · Automata-Theoretic State · codex "Ouroboros Bite" — mirror of idx 5 "Spiral Tongue" (Codex v3.1 §11, named)
- Technical (v3.1): Recursive deadlock, infinite regress without exit
- Placeholder (retired): λ=sin²(83)≈0.937730, κ=log₂(84)≈6.392317, H_max≈0.336392 — index-derived scaffold values; no physical meaning was ever claimed for them, and they are retired for this row.

## Hardened spec

1. **State space:** The space of partial recursive functions on ℕ, with a distinguished class of computations that do not halt: evaluation sequences (e_0 → e_1 → …) with no terminal normal form.
2. **Computable form:** A recursive definition f(x) = F(f, x) whose unfolding never bottoms out: for every n, the n-th unfold still contains a redex. Computable test: the computation's step-count function is unbounded on the given input (semi-decidable — non-termination is co-RE, not decidable, and the spec says so).
3. **Measurable quantity:** Dimensionless: observed step count before resource exhaustion, and the (undecidable in general) halting predicate. Instrument: a step-bounded interpreter with a fuel counter; exceeding fuel is the operational signature.
4. **Standard theory:** Computability theory: non-terminating recursion, the halting problem (Turing 1936). Infinite regress without exit is the standard concept of non-halting.
5. **Prediction differing from standard theory:** none.
6. **Delta assessment:** No delta. This operator is the standard concept of non-terminating recursion under the mythic name "Ouroboros Bite". The serpent imagery adds nothing to the mathematics; the honesty here is that deadlock is undecidable in general, so the operator can only ever name the phenomenon, not decide it.

## Verdict: ANCHOR

Relabel admitted. "Ouroboros Bite" is retained as the canonical name for non-terminating recursion wherever the Engine's constraint machinery needs that slot. It makes no claim beyond the textbook — including the textbook's own limit: non-termination cannot be decided in general. Placeholder λ/κ/H_max retired for this row.

Grounded: Codex v3.1 §11 (named S2); anchor: non-terminating recursion (standard computability theory)

Verdict: ANCHOR
