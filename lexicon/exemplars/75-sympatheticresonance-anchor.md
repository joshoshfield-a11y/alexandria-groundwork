# Exemplar — ANCHOR: idx 75, "Sympathetic Resonance" (Choral)

Date: 2026-10-12.

## Canon row

- idx 75 · Choral · Graph-Theoretic Node · codex "Sympathetic Resonance" (final name, confirmed 2026-10-14)
- Technical (v3.1): (none — extension slot, unnamed in every source)
- Placeholder (retired): λ=sin²(75)≈0.150375, κ=log₂(76)≈6.247928, H_max≈0.610777 — index-derived scaffold values; no physical meaning was ever claimed for them, and they are retired for this row.

## Hardened spec

1. **State space:** a damped harmonic oscillator driven by a periodic force — a mass on a spring with damping, an RLC circuit, a wine glass under a loudspeaker.
2. **Computable form:** m·ẍ + c·ẋ + k·x = F_0·cos(ωt). The steady-state amplitude is A(ω) = F_0 / √((k − mω²)² + (cω)²), which peaks at the natural frequency ω_0 = √(k/m) (lightly damped). At resonance the amplitude is A_max ≈ F_0/(c·ω_0) and the quality factor Q = √(mk)/c measures the sharpness: the resonance bandwidth is Δω ≈ ω_0/Q. Worked example: m = 1 kg, k = 100 N/m, c = 2 N·s/m, F_0 = 10 N. Then ω_0 = 10 rad/s, Q = √(100)/2 = 5, and A_max = 10/(2·10) = 0.5 m — five times the static deflection F_0/k = 0.1 m. Drive it at 5 rad/s instead and the amplitude collapses to ≈ 0.132 m.
3. **Measurable quantity:** resonant frequency in Hz (rad/s angular); amplitude in meters (or volts for circuits); Q factor, dimensionless. Instrument: frequency sweep with a shaker table and accelerometer (mechanical) or a signal generator and oscilloscope (electrical); the amplitude-vs-frequency peak is the direct observation.
4. **Standard theory:** classical mechanics of driven oscillations; the identical mathematics governs series/parallel RLC resonance in circuit theory.
5. **Delta assessment:** none. "Sympathetic Resonance" names the standard driven-oscillator resonance under a finalized name (the slot was unnamed in every v3.1 source). The physics it anchors to is textbook — and it is distinct from idx 16 "High-Q Resonators": that row anchors the resonator's Q; this row names the phenomenon of sympathetic response at a natural frequency.

Why this name: the Choral pillar is the wave/oscillation pillar (envelopes, waveforms, wave vectors, feedback, opposition), and sympathetic resonance — the pillar's central phenomenon of a system responding at its natural frequency — is conspicuously absent from its eighteen named operators. It completes the set rather than duplicating it.

## Verdict: ANCHOR

Final name **"Sympathetic Resonance"** (confirmed 2026-10-14) for idx 75: the driven oscillator's amplitude peak A(ω) at ω_0 = √(k/m), Q = √(mk)/c — 0.5 m at 10 rad/s for the worked 1-kg system. Relabel admitted; no novelty claimed. The placeholder λ/κ/H_max are retired; the operator's application is the frequency-sweep measurement above.

Grounded: standard classical-mechanics textbook (driven oscillations; e.g. French, Vibrations and Waves).

Verdict: ANCHOR
