# Exemplar — ANCHOR: idx 51, "Triadic Stability" (Choral)

Date: 2026-10-12.

## Canon row

- idx 51 · Choral · Graph-Theoretic Node · codex "Triadic Stability"
- Technical (v3.1): Triadic Stability
- Placeholder (retired): λ=sin²(51)≈0.449207, κ=log₂(52)≈5.70044, H_max≈0.992543 — index-derived scaffold values; no physical meaning was ever claimed for them, and they are retired for this row.

## Hardened spec

1. **State space:** a three-node structure with fixed pairwise connections — a triangular truss, a 3-cycle graph, three mutually constraining components.
2. **Computable form:** structural rigidity in the plane. A graph with n vertices is minimally rigid in 2D iff it has exactly 2n − 3 edges and every subgraph on k vertices has at most 2k − 3 edges (Laman's condition). The triangle (n = 3, edges = 3 = 2·3 − 3) is the smallest rigid graph: fixing its three edge lengths fixes its shape completely — zero internal degrees of freedom. Worked contrast: a 4-node cycle (square, 4 edges < 2·4 − 3 = 5) has one flex mode — it can shear into a rhombus without changing edge lengths. Add one diagonal (5 edges) and it becomes minimally rigid. Rigidity is certified by the rank of the rigidity matrix: full rank 2n − 3 means rigid.
3. **Measurable quantity:** internal degrees of freedom (integer count, dimensionless); equivalently the rank deficiency of the measured rigidity matrix. Instrument: the computation itself on measured geometry — edge lengths from calipers/laser tracking; a structure that holds its shape under load confirms rigidity empirically.
4. **Standard theory:** structural rigidity theory — Maxwell's counting rule (1864), Laman's theorem (1970).
5. **Delta assessment:** none. This operator is the standard rigidity of the triad — the triangle as the minimal stable three-node structure — under a mythic name.

## Verdict: ANCHOR

"Triadic Stability" is the triangle's rigidity: 3 nodes, 3 edges, 2n − 3 satisfied, zero flex modes — the reason three legs never wobble. Relabel admitted; no novelty claimed. The placeholder λ/κ/H_max are retired; the operator's application is the rigidity-count procedure above.

Grounded: Maxwell 1864 (counting rule); Laman 1970 (structural rigidity theory).

Verdict: ANCHOR
