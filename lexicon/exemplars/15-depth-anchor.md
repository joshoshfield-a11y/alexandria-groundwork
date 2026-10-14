# Exemplar — ANCHOR: idx 15, "Depth" (Choral)

Date: 2026-10-12.

## Canon row

- idx 15 · Choral · Graph-Theoretic Node · codex "Depth"
- Technical (v3.1): Depth
- Placeholder (retired): λ=sin²(15)≈0.422874, κ=log₂(16)=4.0, H_max≈0.982768 — index-derived scaffold values; no physical meaning was ever claimed for them, and they are retired for this row.

## Hardened spec

1. **State space:** a rooted graph or tree G = (V, E) with designated root r — a file-system hierarchy, a call tree, a network with a gateway node.
2. **Computable form:** depth(v) = dist(r, v), the length (in edges) of the shortest path from the root to v; depth(r) = 0. The tree's depth is max_v depth(v). Worked example: root r with children a, b; a has child c. Then depth(r) = 0, depth(a) = depth(b) = 1, depth(c) = 2, and the tree depth is 2. Computed by breadth-first search in O(|V| + |E|); in an unrooted graph the same quantity is the node's eccentricity relative to the chosen reference.
3. **Measurable quantity:** depth is an integer count of edges/hops — dimensionless. Instrument: BFS traversal of a measured adjacency (network topology scan, stack-frame walk for call depth, `find` for directory depth).
4. **Standard theory:** elementary graph theory; BFS correctness and the definition of distance in unweighted graphs are textbook.
5. **Delta assessment:** none. This operator is the standard graph-theoretic depth (distance from a root) under a mythic name. It does not mean profundity, ocean depth, or optical depth — those are different, separately nameable quantities, and the operator as scaffolded is the graph one (its domain is Graph-Theoretic Node).

## Verdict: ANCHOR

"Depth" is depth(v) = dist(r, v) in edges, computed by BFS, measured as a hop count. Relabel admitted; no novelty claimed. The placeholder λ/κ/H_max are retired; the operator's application is the traversal procedure above.

Grounded: standard graph-theory textbook (e.g. Diestel, Graph Theory — BFS and distance).

Verdict: ANCHOR
