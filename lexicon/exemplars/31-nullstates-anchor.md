# Exemplar — ANCHOR: idx 31, "Null States" (Choral)

Date: 2026-10-12.

## Canon row

- idx 31 · Choral · Algebraic Group Action · codex "Null States"
- Technical (v3.1): Null States
- Placeholder (retired): λ=sin²(31)≈0.163246, κ=log₂(32)=5.0, H_max≈0.64202 — index-derived scaffold values; no physical meaning was ever claimed for them, and they are retired for this row.

## Hardened spec

1. **State space:** a linear operator L: V → W between vector spaces — a transfer matrix, a discretized differential operator, a measurement map from inputs to outputs.
2. **Computable form:** the null space (kernel) ker(L) = {v ∈ V : Lv = 0}: the set of inputs the operator annihilates. Found by solving the homogeneous system Lx = 0 (row reduction / SVD). Worked example: L = [[1, 2],[2, 4]]. Row reduction gives x + 2y = 0, so ker(L) is spanned by (−2, 1)ᵀ — nullity 1, rank 1, and indeed 1 + 1 = 2 = dim V (rank–nullity). These are the inputs that produce exactly zero output: the operator's blind directions.
3. **Measurable quantity:** the eigenvalue/singular value exactly zero (in the operator's spectral units); nullity as an integer count of independent null directions. Instrument: singular-value decomposition of a measured transfer matrix — singular values at the noise floor mark the empirical null space.
4. **Standard theory:** linear algebra — kernel, rank–nullity theorem; zero modes of differential operators (e.g., the constant functions annihilated by the gradient).
5. **Delta assessment:** none. This operator is the standard null space / kernel under a mythic name. It is not the quantum vacuum (which would be a separate, separately nameable operator) — the scaffolded technical term is the algebraic null state.

## Verdict: ANCHOR

"Null States" is ker(L) = {v : Lv = 0}, computed by solving Lx = 0 and measured as the SVD noise floor of a transfer matrix. Relabel admitted; no novelty claimed. The placeholder λ/κ/H_max are retired; the operator's application is the kernel computation above.

Grounded: standard linear-algebra textbook (rank–nullity theorem).

Verdict: ANCHOR
