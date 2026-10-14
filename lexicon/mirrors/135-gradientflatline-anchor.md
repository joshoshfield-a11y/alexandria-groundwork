# Exemplar — ANCHOR: idx 135, "Gradient Flatline" (Mirror of idx 57, "Architect's Seal")

Date: 2026-10-14. Mirror-canon proposal (WS4): the shadow dual of primal idx 57 "Architect's Seal" (gradients), named in Codex v3.1 §11 as S15. Where the gradient points the way, the flatline is the way vanishing.

## Canon row

- idx 135 · Foundational · Computational Complexity Class · codex "Gradient Flatline" — mirror of idx 57 "Architect's Seal" (Codex v3.1 §11, named)
- Technical (v3.1): Optimization death, local minimum trap, zero slope
- Placeholder (retired): λ=sin²(135)≈0.007809, κ=log₂(136)≈7.087463, H_max≈0.065890 — index-derived scaffold values; no physical meaning was ever claimed for them, and they are retired for this row.

## Hardened spec

1. **State space:** A parameterized model with loss L(θ) trained by gradient descent, θ ← θ − η∇L. Deep or recurrent architectures where gradients propagate through many composed maps.
2. **Computable form:** Vanishing gradient: ‖∂L/∂θ_early‖ ≤ γ^L ‖∂L/∂θ_late‖ with γ < 1 the layer-wise contraction factor — gradients decay exponentially with depth L, so early parameters freeze: optimization death while loss is still high. Saddle/flat-region trapping is the same signature: ∇L ≈ 0 far from any good minimum.
3. **Measurable quantity:** Gradient norm ‖∇L‖ (dimensionless, per-parameter) vs. depth; stall epochs (count). Instrument: gradient-norm logging during training — exponential decay with depth is the signature.
4. **Standard theory:** Optimization / deep learning: the vanishing-gradient problem (Hochreiter 1991; standard).
5. **Prediction differing from standard theory:** none.
6. **Delta assessment:** No delta. This operator is the standard concept of vanishing gradients — optimization death by zero slope — under the mythic name "Gradient Flatline". The name is unusually literal: the gradient trace goes flat.

## Verdict: ANCHOR

Relabel admitted. "Gradient Flatline" is retained as the canonical name for vanishing-gradient arrest wherever the Engine's constraint machinery needs that slot. No novelty claimed; the measurable is the gradient norm, and the placeholder λ/κ/H_max are retired for this row.

Grounded: Codex v3.1 §11 (named S15); anchor: vanishing gradients (standard deep learning / optimization theory)

Verdict: ANCHOR
