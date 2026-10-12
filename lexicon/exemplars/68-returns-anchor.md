# Exemplar — ANCHOR: idx 68, "Returns" (Transcendent T17)

Date: 2026-10-12.

## Canon row

- idx 68 · Transcendent · Probabilistic Field · codex "Returns"
- Technical (v3.1): Returns
- Placeholder (retired): λ=sin²(68)≈0.8063, κ=log₂(69)≈6.1085 — index-derived scaffold values, no physical meaning; retired for this row.

## Hardened spec

1. **State space:** a measure-preserving dynamical system
   (X, μ, T) with μ(X) < ∞; the return set of a neighborhood U,
   T⁻ⁿ(U) ∩ U ≠ ∅.
2. **Computable form:** Poincaré recurrence — almost every x
   returns arbitrarily close to x after some finite n.
   Kac's lemma: mean return time to A is τ_A = 1/μ(A).
   Worked example: a fair coin observed until the pattern HHH
   returns — mean return time τ = 2³ = 8 tosses.
3. **Measurable quantity:** recurrence/return time in seconds
   (or steps). For macroscopic systems τ_rec grows as ~10^N
   with particle count N — effectively infinite; returns are
   directly measured only in few-body or small systems (e.g.
   spin-echo experiments). Instruments: repeated state
   monitoring (e.g. NMR, particle detectors).
4. **Standard theory:** ergodic theory — Poincaré's recurrence
   theorem, Kac's lemma; Loschmidt's paradox resolution for why
   macroscopic returns are unobservable.
5. **Prediction differing from standard theory:** none.

## Verdict: ANCHOR

Relabel admitted. "Returns" is Poincaré recurrence: a finite
measure-preserving system comes back arbitrarily close to its
start, with mean return time 1/μ(A) — the coin-pattern example
worked above, the spin echo as the laboratory instance. The
theory explains both the returns and why macroscopic ones never
happen. The placeholder λ/κ/H_max are retired; the operator's
application is return-time computation (Kac's lemma) and
recurrence measurement in small systems.

**Why not DEFINE:** the recurrence theorem is proved; the only
novelty on offer would be a measurable violation of
measure-preserving dynamics, which is a claim about dynamics,
not about this operator.

Verdict: ANCHOR
