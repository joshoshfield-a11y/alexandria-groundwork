# Exemplar — ANCHOR: idx 72, "Asymptotic Limits" (Transcendent T18)

Date: 2026-10-12.

## Canon row

- idx 72 · Transcendent · Network-Theoretic Hub · codex "Asymptotic Limits"
- Technical (v3.1): Asymptotic Limits
- Placeholder (retired): λ=sin²(72)≈0.0644, κ=log₂(73)≈6.1898 — index-derived scaffold values, no physical meaning; retired for this row.

## Hardened spec

1. **State space:** functions f(x) on an unbounded domain with
   their asymptotic scale sequences {φ_n(x)} (e.g. x^(−n),
   e^(−nx)); limits at x → ∞ or at a singular point.
2. **Computable form:** asymptotic expansion
   f(x) ~ Σ a_n φ_n(x), and limits, e.g. lim_{x→∞} e^(−x)/x = 0.
   Worked example: Stirling's formula n! ~ √(2πn)(n/e)ⁿ —
   for n = 100, √(2π·100)(100/e)¹⁰⁰ ≈ 9.3248×10¹⁵⁷ vs.
   100! = 9.3326215×10¹⁵⁷, relative error ≈ 8.3×10⁻⁴
   (the 1/(12n) correction closes it to ~3×10⁻⁷).
3. **Measurable quantity:** the limit value (dimensionless or in
   the function's units) and the truncation error bound —
   relative error, dimensionless. This is a mathematical
   operator: the "measurement" is numerical evaluation to a
   stated tolerance, checked against the error bound.
4. **Standard theory:** asymptotic analysis — Landau big-O /
   little-o notation, asymptotic series, Laplace's method for
   integrals; dominated convergence for limits of sequences.
5. **Prediction differing from standard theory:** none.

## Verdict: ANCHOR

Relabel admitted, with the same scope note as Singularities
(idx 24). "Asymptotic Limits" is the mathematical practice of
taking limits at infinity and bounding asymptotic expansions —
Stirling's formula worked above, error bounds as the quality
measure. It is complete in the textbooks; there is no bench
instrument, and none is pretended. The placeholder λ/κ/H_max are
retired; the operator's application is limit computation and
asymptotic-expansion error accounting.

**Why not DEFINE:** asymptotic methods are closed mathematics;
the error bounds are the content, and no physical prediction is
attached to them.
Grounded: asymptotic analysis — Stirling's formula (standard mathematical reference)

Verdict: ANCHOR
