# Exemplar — ANCHOR: idx 10, "Summation" (Cosmic D3)

Date: 2026-10-12.

## Canon row

- idx 10 · Cosmic · Signal-Processing Operator · codex "Summation"
- Technical (v3.1): Summation
- Placeholder (retired): λ=sin²(10)≈0.2960, κ=log₂(11)≈3.4594 — index-derived scaffold values, no physical meaning claimed

## Hardened spec

1. **State space:** finite real-valued sequences x = (x₀, …, x_{N−1}) ∈ ℝ^N — sampled signals, charge increments, or event counts.
2. **Computable form:** S_N = Σ_{n=0}^{N−1} x_n, the discrete integral; the running version is the cumulative sum y_k = Σ_{n=0}^{k} x_n. Worked example: samples x = [1, 2, 3, 4] (volts sampled at 1 kHz) → S = 10, and the running sums are [1, 3, 6, 10]. Convergence of infinite sums is governed by standard tests (ratio, comparison); the operator as used in the Engine is finite accumulation.
3. **Measurable quantity:** accumulated charge in coulombs (C) when summing current samples via an integrator circuit (Q = Σ I_n Δt), or a dimensionless count when summing events. Instrument: op-amp integrator, or digital accumulation in software.
4. **Standard theory:** elementary analysis — Riemann sums, the discrete-time integrator (accumulator) in DSP, and the fundamental theorem linking summation to finite differences.
5. **Delta assessment:** none. This operator is textbook discrete integration under a mythic name.

## Verdict: ANCHOR

Relabel admitted. "Summation" is finite discrete accumulation S_N = Σ x_n; the hardening writes the standard form, a worked numerical example, and the integrator-measurement procedure, claiming no novelty. Note the engine's running use: the accumulator is the discrete-time integrator with z-domain transfer function 1/(1−z⁻¹) — standard DSP, included so the signal-processing entry points at a checkable object. The placeholder λ/κ/H_max are retired for this row.

Grounded: Oppenheim & Schafer, Discrete-Time Signal Processing (accumulator, 1/(1−z⁻¹))

Verdict: ANCHOR
