# Exemplar — ANCHOR: idx 2, "Wavefunction Amplitude" (Cosmic D1)

Date: 2026-10-12.

## Canon row

- idx 2 · Cosmic · Category-Theoretic Morphism · codex "Wavefunction Amplitude"
- Technical (v3.1): Wavefunction Amplitude
- Placeholder (retired): λ=sin²(2)≈0.8268, κ=log₂(3)≈1.5850 — index-derived scaffold values, no physical meaning claimed

## Hardened spec

1. **State space:** normalized complex-valued functions ψ ∈ L²(ℝ³) with ∫|ψ|² d³x = 1; the exemplar works a 1-D ground state on [0, L].
2. **Computable form:** the Born rule — |ψ(x)|² is the position probability density; P(a < x < b) = ∫_a^b |ψ(x)|² dx. Worked example: particle in a 1-D box of length L = 1 m, ψ₁(x) = √2 sin(πx). P(0.25 < x < 0.5) = 2∫_{0.25}^{0.5} sin²(πx) dx = 2[(x/2) − sin(2πx)/4π]_{0.25}^{0.5} ≈ 0.409. The amplitude ψ itself is complex and not directly observable; only |ψ|² carries statistics.
3. **Measurable quantity:** probability density in m⁻³ (dimensionless probabilities over finite volumes), estimated as relative frequencies of position outcomes over N repeated preparations (binomial statistics, σ = √(p(1−p)/N)). Instrument: position-resolving detector (CCD array, scanning probe).
4. **Standard theory:** quantum mechanics — Born rule (1926); normalization and the spectral theorem for the position observable.
5. **Delta assessment:** none. The morphism framing (ψ as an arrow into the probability simplex via the Born rule) is standard category-flavored rephrasing, not new physics.

## Verdict: ANCHOR

Relabel admitted. "Wavefunction Amplitude" is the complex amplitude ψ whose squared modulus gives observable statistics; the hardening writes the Born rule, a worked normalization example, and the measurement procedure, claiming no novelty. The placeholder λ/κ/H_max are retired for this row.

Verdict: ANCHOR
