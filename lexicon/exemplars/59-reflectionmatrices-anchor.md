# Exemplar — ANCHOR: idx 59, "Reflection Matrices" (Choral)

Date: 2026-10-12.

## Canon row

- idx 59 · Choral · Thermodynamic Ensemble · codex "Reflection Matrices"
- Technical (v3.1): Reflection Matrices
- Placeholder (retired): λ=sin²(59)≈0.405435, κ=log₂(60)≈5.906891, H_max≈0.974041 — index-derived scaffold values; no physical meaning was ever claimed for them, and they are retired for this row.

## Hardened spec

1. **State space:** a Euclidean vector space ℝⁿ with a chosen mirror hyperplane through the origin, specified by its unit normal u.
2. **Computable form:** the Householder reflection R = I − 2uuᵀ. Properties: R is orthogonal (RᵀR = I), involutory (R² = I — reflecting twice returns the original), det(R) = −1, eigenvalues +1 (multiplicity n − 1, the mirror plane) and −1 (the normal direction). Worked example in 2D: mirror across the y-axis, u = (1, 0), so R = [[−1, 0],[0, 1]]. Applied to v = (3, 4): Rv = (−3, 4) — the x-component flips, y is untouched. Check: R² = I, det = −1, eigenvalues −1 and +1. Householder reflections are the workhorse of QR decomposition: any matrix is reduced to triangular form by a product of such reflections.
3. **Measurable quantity:** matrix entries (dimensionless); the reflection is verified numerically by R² = I and RᵀR = I to machine precision. Instrument: the computation on measured transformation data (e.g., a calibrated mirror's action on basis vectors).
4. **Standard theory:** linear algebra — Householder transformations (1958), the standard tool of numerical QR factorization.
5. **Delta assessment:** none. This operator is the standard Householder reflection matrix under a mythic name.

## Verdict: ANCHOR

"Reflection Matrices" is R = I − 2uuᵀ: orthogonal, involutory, determinant −1 — the mirror in matrix form. Relabel admitted; no novelty claimed. The placeholder λ/κ/H_max are retired; the operator's application is the matrix verification above.

Verdict: ANCHOR
