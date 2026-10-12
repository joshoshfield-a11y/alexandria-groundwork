# Exemplar — ANCHOR: idx 63, "Recursive Layering" (Choral)

Date: 2026-10-12.

## Canon row

- idx 63 · Choral · Graph-Theoretic Node · codex "Recursive Layering"
- Technical (v3.1): Recursive Layering
- Placeholder (retired): λ=sin²(63)≈0.028008, κ=log₂(64)=6.0, H_max≈0.184301 — index-derived scaffold values; no physical meaning was ever claimed for them, and they are retired for this row.

## Hardened spec

1. **State space:** a recursively defined structure: a base case plus a reduction rule that defines each layer in terms of smaller ones — a recursive function, a fractally nested data structure, stacked network layers where each layer's output feeds the next.
2. **Computable form:** f(base) = value_0; f(n) = combine(f(n−1), …, f(n−k)) for n above the base. The layering is the call tree; its depth is the recursion depth d(n). Worked example: factorial F(0) = 1, F(n) = n·F(n−1). Then F(5) = 5·F(4) = … = 120, with recursion depth 5 — five nested layers of pending multiplication, each waiting on the one below. Termination is guaranteed iff every reduction strictly decreases a well-founded measure (here, n itself).
3. **Measurable quantity:** recursion depth (integer count of nested layers, dimensionless); stack memory in bytes (depth × frame size). Instrument: profiler / call-stack inspection; stack-overflow at the implementation's frame limit is the empirical depth ceiling.
4. **Standard theory:** computability and programming-language theory — structural recursion, well-founded induction; in machine learning, the same layering idea appears as depth in stacked architectures.
5. **Delta assessment:** none. This operator is the standard recursive definition / layered recursion under a mythic name.

## Verdict: ANCHOR

"Recursive Layering" is structural recursion: base case plus reduction rule, depth measured in nested layers — F(5) = 120 at depth 5. Relabel admitted; no novelty claimed. The placeholder λ/κ/H_max are retired; the operator's application is the depth accounting above.

Verdict: ANCHOR
