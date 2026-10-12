# Exemplar — ANCHOR: idx 47, "Harmonic Means" (Choral)

Date: 2026-10-12.

## Canon row

- idx 47 · Choral · Thermodynamic Ensemble · codex "Harmonic Means"
- Technical (v3.1): Harmonic Means
- Placeholder (retired): λ=sin²(47)≈0.01527, κ=log₂(48)≈5.584963, H_max≈0.113989 — index-derived scaffold values; no physical meaning was ever claimed for them, and they are retired for this row.

## Hardened spec

1. **State space:** n positive quantities x_i that are rates with a common numerator — speeds over equal distances, parallel resistances via conductances, pixel rates.
2. **Computable form:** H = n / Σ_i (1/x_i), the reciprocal of the arithmetic mean of the reciprocals. It is the correct average when the denominator varies and the numerator is fixed. Worked example: drive 60 km/h one way and 40 km/h back over the same distance. The arithmetic mean (50 km/h) is wrong — total distance 2d over total time d/60 + d/40 gives 2/(1/60 + 1/40) = 48 km/h, the harmonic mean. Equivalently, H ≤ G ≤ A (harmonic ≤ geometric ≤ arithmetic), with equality iff all x_i are equal.
3. **Measurable quantity:** the harmonic mean carries the same units as the inputs (km/h, ohms for parallel-resistor equivalent via conductances, etc.). Instrument: whatever measures the underlying rates — speedometer/odometer and stopwatch for the travel example; the mean itself is computed.
4. **Standard theory:** elementary statistics; the Pythagorean means and their ordering; the standard result that averaging rates over equal numerators requires the harmonic mean.
5. **Delta assessment:** none. This operator is the standard harmonic mean under a mythic name.

## Verdict: ANCHOR

"Harmonic Means" is H = n/Σ(1/x_i) — the right average for rates over equal numerators, 48 km/h for the 60/40 round trip, not 50. Relabel admitted; no novelty claimed. The placeholder λ/κ/H_max are retired; the operator's application is the rate-averaging computation above.

Verdict: ANCHOR
