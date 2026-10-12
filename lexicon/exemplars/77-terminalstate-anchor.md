# Exemplar — ANCHOR: idx 77, "Terminal State" — PROPOSED (Foundational)

Date: 2026-10-12.

## Canon row

- idx 77 · Foundational · Automata-Theoretic State · codex UNNAMED
- Proposed name: **"Terminal State"** (PROPOSED — user confirms or rejects)
- Technical (v3.1): none given; hardened structurally from pillar/domain
- Placeholder (retired): λ=sin²(77)=0.999041, κ=log₂(78)=6.285402, H_max=0.011003 — scaffold values, no meaning claimed

## Hardened spec

1. **State space:** a finite automaton (Q, Σ, δ) — or a finite
   Markov chain with transition matrix P — over states Q.
2. **Computable form:** a state q_t is terminal (absorbing) iff
   δ(q_t, a) = q_t for every input a ∈ Σ (equivalently
   P(q_t, q_t) = 1). Worked example: Q = {run, halt},
   δ(run,·) = run or halt, δ(halt,·) = halt — once the machine
   reaches "halt" it never leaves; absorption probability from
   "run" is computed from the chain's fundamental matrix.
3. **Measurable quantity:** dwell counts / absorption probability,
   dimensionless (0 to 1). Instrument: the machine's own
   execution trace, or simulation statistics over N runs.
4. **Standard theory:** automata theory (accepting/halt states of
   DFAs and Turing machines); absorbing Markov chains —
   terminal states partition the state space into transient and
   recurrent classes.
5. **Delta assessment:** none. This operator is the terminal state —
   the fixed, inescapable end-state of a transition system —
   under a proposed mythic name.

## Verdict: ANCHOR

Relabel admitted, name proposed. The Foundational Automata-Theoretic
State slot at idx 77 anchors to the terminal/absorbing state: the
standard end-of-computation fixed point of automata and Markov
theory. The name "Terminal State" is PROPOSED pending the user's
decision; if rejected, any replacement name keeps this anchor.
The placeholder λ/κ/H_max are retired for this row. No novelty
claimed.

Verdict: ANCHOR
