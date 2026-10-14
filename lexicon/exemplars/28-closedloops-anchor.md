# Exemplar — ANCHOR: idx 28, "Closed Loops" (Transcendent T7)

Date: 2026-10-12.

## Canon row

- idx 28 · Transcendent · Information-Theoretic Channel · codex "Closed Loops"
- Technical (v3.1): Closed Loops
- Placeholder (retired): λ=sin²(28)≈0.0734, κ=log₂(29)≈4.8580 — index-derived scaffold values, no physical meaning; retired for this row.

## Hardened spec

1. **State space:** a plant G(s) and feedback controller H(s) in
   the Laplace domain; the closed signal path formed by the loop
   equation.
2. **Computable form:** closed-loop transfer function
   T(s) = G(s)/(1 + G(s)H(s)); stability via Nyquist or
   gain/phase margins. Worked example: G(s) = 10/(s+1), H = 1 →
   T(s) = 10/(s+11), pole at s = −11 (stable), DC gain 10/11,
   bandwidth 11 rad/s.
3. **Measurable quantity:** loop gain (dimensionless, quoted in
   dB), gain margin (dB), phase margin (degrees). Instrument:
   frequency-response / network analyzer injecting a test signal
   around the loop.
4. **Standard theory:** classical control theory — Black's
   negative-feedback amplifier, Nyquist stability criterion,
   Bode plots.
5. **Prediction differing from standard theory:** none.

## Verdict: ANCHOR

Relabel admitted. "Closed Loops" is the standard feedback-control
loop: plant, feedback path, loop gain, and stability margins —
measurable with a network analyzer and fully covered by
Nyquist/Bode theory. Feedback appears across domains
(electronics, biology, economics), but the operator adds nothing
to the formalism. The lead/lag compensators and PID variants
used to shape those margins are likewise standard catalog
items. The placeholder λ/κ/H_max are retired; the
operator's application is the loop-gain and margin measurement
above.

**Why not DEFINE:** closed-loop analysis is a complete
engineering formalism; nonlinear or adaptive extensions are
separate theories already named elsewhere, not delta on this
operator.
Grounded: classical control theory — Black/Nyquist/Bode closed-loop formalism

Verdict: ANCHOR
