# Exemplar — ANCHOR: idx 16, "High-Q Resonators" (Transcendent T4)

Date: 2026-10-12.

## Canon row

- idx 16 · Transcendent · Information-Theoretic Channel · codex "High-Q Resonators"
- Technical (v3.1): High-Q Resonators
- Placeholder (retired): λ=sin²(16)≈0.0829, κ=log₂(17)≈4.0875 — index-derived scaffold values, no physical meaning; retired for this row.

## Hardened spec

1. **State space:** the two-mode energy partition (stored vs.
   dissipated per cycle) of a linear oscillator — electrical,
   mechanical, or optical.
2. **Computable form:** Q = 2π·(energy stored)/(energy lost per
   cycle) = ω₀/Δω = ω₀τ, with ω₀ the resonant frequency and τ the
   amplitude decay time. Worked example: series LCR with
   L = 10 μH, C = 100 pF → f₀ = 1/(2π√(LC)) ≈ 5.03 MHz;
   R = 2 Ω → Q = ω₀L/R ≈ 158.
3. **Measurable quantity:** Q is dimensionless; linewidth Δf in
   hertz. Instrument: vector network analyzer (S₂₁ peak at −3 dB),
   ring-down measurement for high-Q optical cavities.
4. **Standard theory:** the damped driven harmonic oscillator;
   linear circuit theory. Superconducting cavities reach
   Q ~ 10¹¹; optical whispering-gallery resonators ~ 10⁸.
5. **Prediction differing from standard theory:** none.

## Verdict: ANCHOR

Relabel admitted. "High-Q Resonators" is the standard quality
factor of a linear resonator — dimensionless, measured with a
network analyzer, explained by the damped oscillator. A high-Q
value is an engineering specification, not a new physical
principle. The placeholder λ/κ/H_max are retired; the operator's
application is the Q/linewidth measurement above.

**Why not DEFINE:** Q is a specification number of a known
differential equation, not a discovery. Higher-Q designs are
engineering progress inside the same theory, and this operator
adds no parameter to the damped oscillator.

Verdict: ANCHOR
