# Exemplar — ANCHOR: idx 03, "Amplitude Envelopes" (Choral)

Date: 2026-10-12.

## Canon row

- idx 3 · Choral · Graph-Theoretic Node · codex "Amplitude Envelopes"
- Technical (v3.1): Amplitude Envelopes
- Placeholder (retired): λ=sin²(3)≈0.019915, κ=log₂(4)=2.0, H_max≈0.140962 — index-derived scaffold values; no physical meaning was ever claimed for them, and they are retired for this row.

## Hardened spec

1. **State space:** a real-valued time signal x(t) carrying a fast oscillation whose amplitude varies slowly — amplitude-modulated radio, voiced-speech formants, tremolo, a ringing bell's decay.
2. **Computable form:** the envelope is the magnitude of the analytic signal, e(t) = |x(t) + i·H{x(t)}|, where H is the Hilbert transform. Equivalently, full-wave rectification followed by low-pass filtering at the modulation bandwidth. Worked example: x(t) = A(1 + m·cos(2πf_m t))·cos(2πf_c t) with A = 2, m = 0.5, f_m = 10 Hz, f_c = 440 Hz. The envelope is e(t) = 2(1 + 0.5·cos(20πt)), swinging between 1 and 3 in the same units as x; the 440 Hz carrier is removed and the 10 Hz modulation stands alone. If m > 1 the envelope crosses zero and phase reversals appear — overmodulation, a standard diagnostic.
3. **Measurable quantity:** envelope amplitude in the signal's own units (volts, pascals, photon counts/s); modulation depth m, dimensionless. Instrument: oscilloscope trace of the rectified/low-passed waveform, or the Hilbert magnitude computed from a digitized recording.
4. **Standard theory:** amplitude modulation and the analytic signal (Gabor 1946). Envelope detection by rectifier plus low-pass filter is the textbook AM demodulator; the Hilbert form is its exact mathematical statement.
5. **Delta assessment:** none. This operator is the standard signal-processing envelope under a mythic name.

## Verdict: ANCHOR

"Amplitude Envelopes" is the analytic-signal envelope e(t), computed and measured exactly as the textbooks prescribe — no fog, no extra claim. Relabel admitted; no novelty claimed. The placeholder λ/κ/H_max are retired; the operator's application is the measurement procedure above.

Verdict: ANCHOR
