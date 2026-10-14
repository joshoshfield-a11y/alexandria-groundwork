# Exemplar — ANCHOR: idx 39, "Unions" (Choral)

Date: 2026-10-12.

## Canon row

- idx 39 · Choral · Graph-Theoretic Node · codex "Unions"
- Technical (v3.1): Unions
- Placeholder (retired): λ=sin²(39)≈0.928902, κ=log₂(40)≈5.321928, H_max≈0.37001 — index-derived scaffold values; no physical meaning was ever claimed for them, and they are retired for this row.

## Hardened spec

1. **State space:** two sets (or events) A and B in a common universe — two sensor coverage regions, two failure-mode event sets, two node neighborhoods in a graph.
2. **Computable form:** A ∪ B = {x : x ∈ A or x ∈ B}. Measure form (inclusion–exclusion): μ(A ∪ B) = μ(A) + μ(B) − μ(A ∩ B) — the overlap is subtracted once so it is not double-counted. Worked example: P(A) = 0.4, P(B) = 0.5, P(A ∩ B) = 0.2 gives P(A ∪ B) = 0.4 + 0.5 − 0.2 = 0.7. For disjoint sets the intersection term vanishes and the union measure is the plain sum. Graph form: the union of two subgraphs takes all vertices and edges of both.
3. **Measurable quantity:** probability (dimensionless, 0–1) or the measure's units (area in m² for coverage regions, count for discrete sets). Instrument: counting / frequency observation over trials; planimetry or GIS overlay for spatial unions.
4. **Standard theory:** elementary set theory; Kolmogorov's probability axioms, where finite additivity with inclusion–exclusion is the union's working form.
5. **Delta assessment:** none. This operator is the standard set union under a mythic name.

## Verdict: ANCHOR

"Unions" is A ∪ B with inclusion–exclusion μ(A ∪ B) = μ(A) + μ(B) − μ(A ∩ B) — the overlap counted once. Relabel admitted; no novelty claimed. The placeholder λ/κ/H_max are retired; the operator's application is the counting/overlay procedure above.

Grounded: Kolmogorov probability axioms; standard set-theory / probability textbook.

Verdict: ANCHOR
