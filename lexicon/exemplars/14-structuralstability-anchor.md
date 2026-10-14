# Exemplar — ANCHOR: idx 14, "Structural Stability" (Cosmic D4)

Date: 2026-10-12.

## Canon row

- idx 14 · Cosmic · Category-Theoretic Morphism · codex "Structural Stability"
- Technical (v3.1): Structural Stability
- Placeholder (retired): λ=sin²(14)≈0.9813, κ=log₂(15)≈3.9069 — index-derived scaffold values, no physical meaning claimed

## Hardened spec

1. **State space:** C¹ vector fields on a compact manifold M — the space of dynamical systems ẋ = f(x) with the C¹ topology.
2. **Computable form:** f is structurally stable if there exists ε > 0 such that every g with ‖g − f‖_{C¹} < ε is topologically equivalent to f (an orbit-preserving homeomorphism exists). Worked example: ẋ = −x, ẏ = −2y has Jacobian eigenvalues −1, −2 — a hyperbolic sink, hence structurally stable (small perturbations keep a sink nearby). Contrast ẋ = −x³, whose zero eigenvalue is non-hyperbolic: an arbitrarily small perturbation ẋ = −x³ + δ changes the equilibrium structure, so it is structurally unstable.
3. **Measurable quantity:** persistence of attractor type under parameter sweeps — e.g., the largest Lyapunov exponent in s⁻¹ staying negative across a perturbation interval. Instrument: parameter-sweep experiment with state recording, bifurcation diagram construction.
4. **Standard theory:** Andronov–Pontryagin (1937); Peixoto's theorem (1962) characterizing structurally stable flows on compact surfaces.
5. **Delta assessment:** none. This operator is the classical structural-stability concept under a mythic name.

## Verdict: ANCHOR

Relabel admitted. "Structural Stability" is the Andronov–Pontryagin property of a vector field; the hardening writes the definition, contrasting worked examples of stable and unstable equilibria, and the parameter-persistence measurement, claiming no novelty. A practical check: in a planar system, verifying that all equilibria are hyperbolic, all limit cycles have non-unit Floquet multipliers, and no saddle connections exist certifies stability via Peixoto's full criterion — a finite, checkable condition. The placeholder λ/κ/H_max are retired for this row.

Grounded: Guckenheimer & Holmes, Nonlinear Oscillations (structural stability, Peixoto's theorem)

Verdict: ANCHOR
