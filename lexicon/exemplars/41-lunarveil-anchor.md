# Exemplar — ANCHOR: idx 41, "Lunar Veil" (Foundational)

Date: 2026-10-12.

## Canon row

- idx 41 · Foundational · Automata-Theoretic State · codex "Lunar Veil"
- Technical (v3.1): Memory
- Placeholder (retired): λ=sin²(41)=0.025161, κ=log₂(42)=5.392317, H_max=0.169512 — scaffold values, no meaning claimed

## Hardened spec

1. **State space:** a finite-state device with state set Q
   (automata) or a register of n bits; the retained past is the
   current state q ∈ Q.
2. **Computable form:** information stored = Shannon entropy of
   the state distribution, H = −Σ_q p(q) log₂ p(q) bits; capacity
   of n binary cells is n bits. Worked example: a 2-bit register
   holds one of 4 patterns (00, 01, 10, 11) — 2 bits of memory;
   overwriting it with a fixed pattern erases that information
   (Landauer: erasure dissipates ≥ kT ln 2 per bit).
3. **Measurable quantity:** bits (dimensionless). Instrument:
   read out the register and count distinguishable configurations;
   capacity verified by write-then-readback tests.
4. **Standard theory:** automata theory — memory is exactly the
   finite state distinguishing pasts (Myhill–Nerode: the states
   of the minimal DFA); Shannon information theory; Landauer's
   principle for the physics of erasure. Concretely, a RAM with n
   address lines holds 2^n cells — memory capacity is the state
   count, logarithmic in bits.
5. **Delta assessment:** none. This operator is memory — retained
   state distinguishing past histories — under a mythic name.

## Verdict: ANCHOR

Relabel admitted. "Lunar Veil" is memory: the state of a finite
device encoding which past occurred, quantified in bits by
Shannon entropy, bounded by Landauer's principle on erasure. The
placeholder λ/κ/H_max are retired for this row; the operator's
"application" is the state-retention accounting above. No novelty
claimed.

Grounded: Cover & Thomas (Shannon entropy); Landauer, IBM J. Res. Dev. 1961 (kT ln 2)

Verdict: ANCHOR
