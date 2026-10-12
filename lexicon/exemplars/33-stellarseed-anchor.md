# Exemplar — ANCHOR: idx 33, "Stellar Seed" (Foundational)

Date: 2026-10-12.

## Canon row

- idx 33 · Foundational · Computational Complexity Class · codex "Stellar Seed"
- Technical (v3.1): Seed States
- Placeholder (retired): λ=sin²(33)=0.999824, κ=log₂(34)=5.087463, H_max=0.002452 — scaffold values, no meaning claimed

## Hardened spec

1. **State space:** the internal state of a deterministic
   pseudorandom generator (a finite bit-string), or equivalently
   the initial condition of a deterministic dynamical system.
2. **Computable form:** given seed s₀, the full trajectory is fixed:
   s_{n+1} = F(s_n) for a deterministic transition F. Worked
   example: linear congruential generator
   s_{n+1} = (a·s_n + c) mod m with a=1664525, c=1013904223,
   m=2³², s₀=42 → 1083814273, 378494188, … — the same seed always
   replays the same stream. In dynamical systems the same holds:
   identical initial conditions give identical orbits, and in
   chaotic systems infinitesimally different seeds diverge
   exponentially — the seed is the entire future, compressed.
3. **Measurable quantity:** the seed itself is a dimensionless
   integer (or bit-string); reproducibility is verified by
   re-running and comparing outputs bit-for-bit. Instrument: the
   computer; verification by hash comparison of output streams.
4. **Standard theory:** pseudorandom number generation theory;
   dynamical systems — a trajectory is determined by its initial
   condition (existence–uniqueness for ODEs; deterministic update
   for maps).
5. **Delta assessment:** none. This operator is the seed state —
   the initial condition that fixes a deterministic unfolding —
   under a mythic name.

## Verdict: ANCHOR

Relabel admitted. "Stellar Seed" is the seed/initial condition:
the small input that deterministically fixes the whole
trajectory, the standard notion behind PRNG seeds and dynamical
initial-value problems. The placeholder λ/κ/H_max are retired for
this row; the operator's "application" is the seeded-recurrence
computation above. No novelty claimed.

Verdict: ANCHOR
