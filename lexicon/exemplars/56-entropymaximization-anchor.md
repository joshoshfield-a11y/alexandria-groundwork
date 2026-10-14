# Exemplar — ANCHOR: idx 56, "Entropy Maximization" (Transcendent T14)

Date: 2026-10-12.

## Canon row

- idx 56 · Transcendent · Probabilistic Field · codex "Entropy Maximization"
- Technical (v3.1): Entropy Maximization
- Placeholder (retired): λ=sin²(56)≈0.2720, κ=log₂(57)≈5.8329 — index-derived scaffold values, no physical meaning; retired for this row.

## Hardened spec

1. **State space:** the probability simplex {p_i ≥ 0, Σ p_i = 1}
   over microstates, possibly constrained by observed averages
   ⟨f_k⟩ = Σ p_i f_k(i).
2. **Computable form:** Jaynes' principle — maximize
   S = −k Σ p_i ln p_i subject to constraints → the Boltzmann
   distribution p_i = e^(−βE_i)/Z. Worked example: two states,
   E₀ = 0, E₁ = ε, fixed ⟨E⟩ → p₁/p₀ = e^(−βε), the textbook
   ratio.
3. **Measurable quantity:** entropy S in J/K (thermodynamics) or
   in nats/bits (information theory). Instruments: calorimetry
   (ΔS = ∫ δQ_rev/T); compression/statistics for Shannon H.
4. **Standard theory:** statistical mechanics (Boltzmann, Gibbs);
   the second law, ΔS_total ≥ 0 for isolated systems; Jaynes'
   maximum-entropy inference as the information-theoretic form.
5. **Prediction differing from standard theory:** none.

## Verdict: ANCHOR

Relabel admitted. "Entropy Maximization" is the second law plus
Jaynes' principle: systems evolve toward, and inference should
assume, the highest-entropy distribution consistent with the
constraints — the Boltzmann distribution worked above. It is
measured in J/K by calorimetry and explained by statistical
mechanics, and nonequilibrium extensions (e.g. maximum caliber)
build on the same principle. The placeholder λ/κ/H_max are retired; the operator's
application is the MaxEnt computation and entropy measurement.

**Why not DEFINE:** MaxEnt is both a physical principle and an
inference rule with known derivations; no departure from the
Boltzmann form is asserted, and no falsifier is available.
Grounded: statistical mechanics (Boltzmann/Gibbs); Jaynes' maximum-entropy principle

Verdict: ANCHOR
