# Exemplar — ANCHOR: idx 07, "Eigenvalue Dynamics" (Choral)

Date: 2026-10-12.

## Canon row

- idx 7 · Choral · Algebraic Group Action · codex "Eigenvalue Dynamics"
- Technical (v3.1): Eigenvalue Dynamics
- Placeholder (retired): λ=sin²(7)≈0.431631, κ=log₂(8)=3.0, H_max≈0.986471 — index-derived scaffold values; no physical meaning was ever claimed for them, and they are retired for this row.

## Hardened spec

1. **State space:** a linear dynamical system ẋ = Ax (continuous) or x_{n+1} = Ax_n (discrete), with A an n×n real or complex matrix — a linearized pendulum, a coupled oscillator network, a discretized PDE.
2. **Computable form:** solve det(A − λI) = 0 for the eigenvalues λ_i. The dynamics are the superposition of modes e^{λ_i t} (continuous): the system is asymptotically stable iff Re(λ_i) < 0 for all i; Re(λ_i) is the growth/decay rate and Im(λ_i) the oscillation frequency of mode i. Worked example: A = [[−1, 2],[0, −3]] has eigenvalues λ = −1 and λ = −3 (triangular, read off the diagonal); both real parts negative, so the origin is a stable node and every trajectory decays like e^{−t} or faster. If one eigenvalue were +0.5, that mode would grow without bound.
3. **Measurable quantity:** decay/growth rates in s⁻¹ (Re λ) and modal frequencies in rad/s (Im λ). Instrument: system identification — fit exponentials and sinusoids to a measured impulse or step response; the fitted exponents are the eigenvalues' real parts.
4. **Standard theory:** linear stability theory and spectral analysis of linear operators; the continuous-time criterion Re(λ_i) < 0 and its discrete analogue |λ_i| < 1 are textbook.
5. **Delta assessment:** none. This operator is the eigenvalue analysis of a linear dynamical system under a mythic name.

## Verdict: ANCHOR

"Eigenvalue Dynamics" is the standard spectral analysis of ẋ = Ax: compute the spectrum, read stability and modal structure off the real and imaginary parts. Relabel admitted; no novelty claimed. The placeholder λ/κ/H_max are retired (note: the placeholder was also literally named λ — it has nothing to do with eigenvalues, which is exactly why the scaffold values had to go). The operator's application is the measurement procedure above.

Verdict: ANCHOR
