# Exemplar — ANCHOR: idx 35, "Divergence" (Choral)

Date: 2026-10-12.

## Canon row

- idx 35 · Choral · Thermodynamic Ensemble · codex "Divergence"
- Technical (v3.1): Divergence
- Placeholder (retired): λ=sin²(35)≈0.18334, κ=log₂(36)≈5.169925, H_max≈0.68733 — index-derived scaffold values; no physical meaning was ever claimed for them, and they are retired for this row.

## Hardened spec

1. **State space:** a vector field F: ℝ³ → ℝ³ — a fluid velocity field, an electric field, a heat flux.
2. **Computable form:** ∇·F = ∂F_x/∂x + ∂F_y/∂y + ∂F_z/∂z, the net outward flux per unit volume at a point. Integral form (divergence theorem): ∭_V (∇·F) dV = ∯_S F·dA. Worked example: F = (2x, −y, 0) gives ∇·F = 2 − 1 + 0 = 1 everywhere — each unit cube emits one unit of flux per unit time; a source field. By contrast G = (−y, x, 0) (pure rotation) has ∇·G = 0: circulation without sources. Positive divergence marks sources, negative marks sinks, zero marks incompressibility (∇·v = 0 for an incompressible flow).
3. **Measurable quantity:** for a velocity field, s⁻¹ (volume outflow per unit volume per unit time); for electric field, ∇·E = ρ/ε_0 in V/m². Instrument: particle-image velocimetry or flux probes integrated over a control volume, then divided by the volume.
4. **Standard theory:** vector calculus — the divergence theorem (Gauss/Ostrogradsky); the continuity equation ∂ρ/∂t + ∇·J = 0 as its physical expression.
5. **Delta assessment:** none. This operator is the standard vector-calculus divergence under a mythic name. (The information-theoretic KL divergence is a different, separately nameable quantity; this row anchors to the field operator.)

## Verdict: ANCHOR

"Divergence" is ∇·F, flux per unit volume, positive at sources and negative at sinks — the divergence theorem is its integral face. Relabel admitted; no novelty claimed. The placeholder λ/κ/H_max are retired; the operator's application is the control-volume flux measurement above.

Grounded: standard vector-calculus textbook (divergence theorem; e.g. Griffiths, Introduction to Electrodynamics).

Verdict: ANCHOR
