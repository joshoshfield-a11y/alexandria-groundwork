# Exemplar — ANCHOR: idx 67, "Fractal Iteration" (Choral)

Date: 2026-10-12.

## Canon row

- idx 67 · Choral · Algebraic Group Action · codex "Fractal Iteration"
- Technical (v3.1): Fractal Iteration
- Placeholder (retired): λ=sin²(67)≈0.731914, κ=log₂(68)≈6.087463, H_max≈0.838704 — index-derived scaffold values; no physical meaning was ever claimed for them, and they are retired for this row.

## Hardened spec

1. **State space:** the complex plane under a fixed iteration rule — the quadratic family z_{n+1} = z_n² + c with z_0 = 0, the defining iteration of the Mandelbrot set.
2. **Computable form:** iterate z_{n+1} = z_n² + c; the orbit is bounded (c is in the set) iff it never exceeds |z| = 2, since beyond 2 it escapes to infinity monotonically. The escape time — the first n with |z_n| > 2 — is the standard computable signature. Worked example: c = 0 gives z_n = 0 forever — bounded, in the set. c = 1 gives 0, 1, 2, 5, 26, … — |z| exceeds 2 at n = 3, escaped, not in the set. c = −1 gives 0, −1, 0, −1, … — a 2-cycle, bounded. Coloring pixels by escape time renders the familiar fractal boundary.
3. **Measurable quantity:** escape iteration count (integer, dimensionless); box-counting or Hausdorff dimension of the resulting boundary (dimensionless, e.g., 2 for the Mandelbrot boundary per Shishikura's theorem). Instrument: numerical iteration; image-analysis box counting on the rendered set.
4. **Standard theory:** complex dynamics — the Mandelbrot and Julia sets (Mandelbrot 1980, building on Fatou/Julia); fractal dimension (Hausdorff 1918).
5. **Delta assessment:** none. This operator is the standard escape-time fractal iteration under a mythic name.

## Verdict: ANCHOR

"Fractal Iteration" is z_{n+1} = z_n² + c with the |z| > 2 escape test — bounded at c = 0 and c = −1, escaped at n = 3 for c = 1. Relabel admitted; no novelty claimed. The placeholder λ/κ/H_max are retired; the operator's application is the escape-time computation above.

Verdict: ANCHOR
