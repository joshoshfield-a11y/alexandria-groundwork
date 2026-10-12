# Exemplar — ANCHOR: idx 27, "Feedback Loops" (Choral)

Date: 2026-10-12.

## Canon row

- idx 27 · Choral · Graph-Theoretic Node · codex "Feedback Loops"
- Technical (v3.1): Feedback Loops
- Placeholder (retired): λ=sin²(27)≈0.914655, κ=log₂(28)≈4.807355, H_max≈0.420738 — index-derived scaffold values; no physical meaning was ever claimed for them, and they are retired for this row.

## Hardened spec

1. **State space:** a forward path of gain A with a fraction β of the output returned to the input — an amplifier with a feedback network, a thermostat loop, a population with density-dependent regulation.
2. **Computable form:** closed-loop gain A_f = A / (1 − Aβ); for negative feedback (β given the sign that opposes the input) this is A_f = A/(1 + Aβ), trading gain for stability, linearity, and bandwidth. Stability is decided by the loop gain Aβ: the Nyquist criterion — the loop is stable iff the Nyquist plot of Aβ does not encircle −1. Worked example: A = 100, β = 0.09 gives A_f = 100/(1 + 9) = 10 — gain desensitivity: a 10% drift in A now moves A_f by only ~1%. If β were chosen with the wrong sign so that Aβ = −1 at some frequency, the denominator vanishes and the circuit oscillates — positive feedback into instability.
3. **Measurable quantity:** loop gain (dimensionless), gain margin in dB, phase margin in degrees. Instrument: network/impedance analyzer producing the Bode or Nyquist plot of the measured loop transfer function.
4. **Standard theory:** classical control theory — Black's negative-feedback amplifier (1927), Nyquist stability criterion (1932), Bode's gain–phase relations.
5. **Delta assessment:** none. This operator is the standard closed feedback loop under a mythic name.

## Verdict: ANCHOR

"Feedback Loops" is A_f = A/(1 − Aβ) with Nyquist stability — the whole of classical feedback in one fraction. Relabel admitted; no novelty claimed. The placeholder λ/κ/H_max are retired; the operator's application is the loop-gain measurement above.

Verdict: ANCHOR
