# Exemplar — ANCHOR: idx 11, "Waveforms" (Choral)

Date: 2026-10-12.

## Canon row

- idx 11 · Choral · Thermodynamic Ensemble · codex "Waveforms"
- Technical (v3.1): Waveforms
- Placeholder (retired): λ=sin²(11)≈0.99998, κ=log₂(12)≈3.584963, H_max≈0.000335 — index-derived scaffold values; no physical meaning was ever claimed for them, and they are retired for this row.

## Hardened spec

1. **State space:** a periodic time-domain signal x(t) = x(t + T) — a voltage trace, a pressure wave, any repeating physical oscillation.
2. **Computable form:** the Fourier series x(t) = a_0/2 + Σ_k [a_k·cos(2πk t/T) + b_k·sin(2πk t/T)], with coefficients from the projection integrals a_k = (2/T)∫_0^T x(t)cos(2πk t/T)dt. The waveform's shape is its harmonic content. Worked example: a ±1 square wave of period T has only odd sine harmonics, b_k = 4/(πk) for k odd, so x(t) ≈ (4/π)(sin(2πt/T) + sin(6πt/T)/3 + sin(10πt/T)/5 + …). Three terms already show the flat top and the Gibbs overshoot (~9%) at the edges — the classic waveform-synthesis demo.
3. **Measurable quantity:** amplitude in the signal's units (V, Pa), period T in seconds, harmonic amplitudes, and total harmonic distortion (dimensionless, %). Instrument: oscilloscope for the time trace; spectrum analyzer or FFT for the harmonic decomposition.
4. **Standard theory:** Fourier series for periodic signals (Fourier 1822); the Fourier transform for the aperiodic case.
5. **Delta assessment:** none. This operator is the standard concept of a waveform and its harmonic decomposition under a mythic name.

## Verdict: ANCHOR

"Waveforms" is the Fourier description of a periodic signal: the time trace is the shape, the harmonic series is its content. Relabel admitted; no novelty claimed. The placeholder λ/κ/H_max are retired; the operator's application is the measurement procedure above.

Grounded: Fourier 1822; standard signals-and-systems textbook (e.g. Oppenheim & Willsky Ch. 3, Fourier series).

Verdict: ANCHOR
