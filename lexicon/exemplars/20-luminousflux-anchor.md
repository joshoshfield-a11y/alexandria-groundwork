# Exemplar — ANCHOR: idx 20, "Luminous Flux" (Transcendent T5)

Date: 2026-10-12.

## Canon row

- idx 20 · Transcendent · Probabilistic Field · codex "Luminous Flux"
- Technical (v3.1): Luminous Flux
- Placeholder (retired): λ=sin²(20)≈0.8335, κ=log₂(21)≈4.3923 — index-derived scaffold values, no physical meaning; retired for this row.

## Hardened spec

1. **State space:** spectral power distribution Φ_e(λ) of a light
   source, weighted by the human photopic response V(λ).
2. **Computable form:** Φ_v = K_m ∫ V(λ) Φ_e(λ) dλ, with
   K_m = 683 lm/W. Worked example: 10 W of pure 555 nm light
   (V = 1 at the photopic peak) → Φ_v = 6830 lm, the maximum
   luminous efficacy.
3. **Measurable quantity:** luminous flux in lumens (lm = cd·sr).
   Instrument: integrating sphere with a calibrated photodetector;
   luminous efficacy in lm/W for sources.
4. **Standard theory:** photometry as defined by the CIE —
   radiometry folded through the human visual response. A 60 W
   incandescent lamp emits ≈ 800 lm; the Sun's total luminous
   output ≈ 3.6×10²⁸ lm.
5. **Prediction differing from standard theory:** none.

## Verdict: ANCHOR

Relabel admitted. "Luminous Flux" is the standard CIE photometric
quantity — radiometric power weighted by V(λ), measured in
lumens with an integrating sphere. It is a human-vision
convention layered on radiometry, and it is fully specified.
The placeholder λ/κ/H_max are retired; the operator's
application is the integrating-sphere measurement above.

**Why not DEFINE:** photometry is a human-response convention
fixed by the CIE; a define would need a physical departure —
e.g. wavelength-dependent light-matter interaction outside
radiometry — which is outside this operator's scope and is
not proposed.

Verdict: ANCHOR
