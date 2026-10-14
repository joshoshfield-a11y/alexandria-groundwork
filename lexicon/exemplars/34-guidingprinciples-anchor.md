# Exemplar — ANCHOR: idx 34, "Guiding Principles" (Cosmic D9)

Date: 2026-10-12.

## Canon row

- idx 34 · Cosmic · Signal-Processing Operator · codex "Guiding Principles"
- Technical (v3.1): Hamiltonian/Jacobi
- Placeholder (retired): λ=sin²(34)≈0.2799, κ=log₂(35)≈5.1293 — index-derived scaffold values, no physical meaning claimed

## Hardened spec

1. **State space:** Hamilton's principal function S(q, t) — a scalar field on configuration space × time whose gradient gives the canonical momentum.
2. **Computable form:** the Hamilton–Jacobi equation H(q, ∂S/∂q) + ∂S/∂t = 0. Worked example: free particle of mass m = 2 kg traveling Δx = 10 m in t = 5 s. A solution is S(x, t) = m(x − x₀)²/2t; then p = ∂S/∂x = mΔx/t = 4 kg·m/s, and S evaluates to 2·100/10 = 20 J·s. Trajectories are the characteristic curves of this first-order PDE — the "guiding" of motion by S.
3. **Measurable quantity:** action in joule-seconds (J·s); momentum in kg·m/s follows from p = ∇S. Instrument: action is inferred from measured trajectories and forces (tracking + load cells), not read off a dial.
4. **Standard theory:** classical mechanics — Hamilton (1834), Jacobi; Goldstein's formulation. The HJ equation is the classical limit of the Schrödinger equation under the WKB ansatz ψ = e^{iS/ħ}.
5. **Delta assessment:** none. The operator's own technical column names Hamiltonian/Jacobi outright; this is a direct relabel of the standard theory.

## Verdict: ANCHOR

Relabel admitted — and the codex's own technical gloss ("Hamiltonian/Jacobi") concedes it. "Guiding Principles" is the Hamilton–Jacobi formulation of mechanics; the hardening writes the PDE, a worked free-particle example with action and momentum numbers, and the trajectory-inference procedure, claiming no novelty. The placeholder λ/κ/H_max are retired for this row.

Grounded: Goldstein, Classical Mechanics (Hamilton–Jacobi equation)

Verdict: ANCHOR
