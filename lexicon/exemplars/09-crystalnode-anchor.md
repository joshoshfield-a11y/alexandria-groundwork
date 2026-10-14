# Exemplar — ANCHOR: idx 09, "Crystal Node" (Foundational)

Date: 2026-10-12.

## Canon row

- idx 9 · Foundational · Computational Complexity Class · codex "Crystal Node"
- Technical (v3.1): Coherence
- Placeholder (retired): λ=sin²(9)=0.169842, κ=log₂(10)=3.321928, H_max=0.657342 — scaffold values, no meaning claimed

## Hardened spec

1. **State space:** density matrices ρ on a finite-dimensional Hilbert
   space ℂ^d, expressed in a fixed reference basis {|i⟩}.
2. **Computable form:** the l₁-norm of coherence,
   C_{l1}(ρ) = Σ_{i≠j} |ρ_{ij}|, the sum of the magnitudes of all
   off-diagonal elements (Baumgratz–Cramer–Plenio, 2014). Worked
   example: a qubit with ρ = [[0.5, 0.4],[0.4, 0.5]] gives
   C_{l1} = 2×0.4 = 0.8; a fully decohered diagonal state gives 0.
   Under a dephasing channel ρ → (1−p)ρ + p·ZρZ, the off-diagonals
   shrink by (1−2p) per application and C_{l1} decays to zero —
   decoherence is coherence leaking away.
3. **Measurable quantity:** dimensionless (0 ≤ C_{l1} ≤ d−1).
   Instrument: quantum state tomography followed by the sum above,
   or inferred operationally from interference fringe visibility,
   which scales with the off-diagonal magnitude.
4. **Standard theory:** the resource theory of quantum coherence;
   decoherence theory (environment-induced suppression of
   off-diagonal elements in the pointer basis).
5. **Delta assessment:** none. This operator is quantum coherence —
   the magnitude of superposition retained in a stated basis,
   the resource consumed by every interference experiment —
   under a mythic name.

## Verdict: ANCHOR

Relabel admitted. "Crystal Node" is coherence: the quantified
presence of off-diagonal density-matrix elements, the standard
measure of how much superposition a system retains against
decoherence. The placeholder λ/κ/H_max are retired for this row;
the operator's "application" is the l₁-norm computation above.
No novelty claimed.

Grounded: Baumgratz–Cramer–Plenio, PRL 113, 140401 (2014) (l1-norm of coherence)

Verdict: ANCHOR
