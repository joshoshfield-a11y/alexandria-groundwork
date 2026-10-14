# Exemplar — ANCHOR: idx 65, "Fractal Bloom" (Foundational)

Date: 2026-10-12.

## Canon row

- idx 65 · Foundational · Automata-Theoretic State · codex "Fractal Bloom"
- Technical (v3.1): Growth
- Placeholder (retired): λ=sin²(65)=0.683646, κ=log₂(66)=6.044394, H_max=0.900373 — scaffold values, no meaning claimed

## Hardened spec

1. **State space:** a non-negative population size N(t) ≥ 0
   (cells, individuals, or automaton live-cells).
2. **Computable form:** exponential growth dN/dt = rN, giving
   N(t) = N₀e^{rt}; with a carrying capacity K, the logistic
   form dN/dt = rN(1 − N/K). Worked example: N₀ = 100 cells,
   r = 0.1 h⁻¹ → after 10 h, N = 100·e¹ ≈ 272 cells; doubling
   time ln 2/r ≈ 6.9 h. With capacity K the logistic solution
   N(t) = K/(1 + A·e^{−rt}), A = (K−N₀)/N₀, bends the exponential
   over: K = 1000, N₀ = 100 gives A = 9 and a sigmoid approach
   to saturation — unbounded bloom checked by limits.
3. **Measurable quantity:** counts (dimensionless) and the growth
   rate r in s⁻¹. Instrument: hemocytometer / plate counts for
   cells; census for organisms; step-counter for automaton
   generations.
4. **Standard theory:** Malthusian and logistic growth models;
   branching processes (Galton–Watson) for stochastic growth;
   cellular-automaton growth rules (e.g., Life gliders expanding
   a live region).
5. **Delta assessment:** none. This operator is growth — the
   rate-proportional increase of a population, saturating under
   resource limits — under a mythic name.

## Verdict: ANCHOR

Relabel admitted. "Fractal Bloom" is growth: exponential increase
at rate r, bounded by carrying capacity in the logistic form,
the standard population-dynamics object. The placeholder λ/κ/H_max
are retired for this row; the operator's "application" is the
growth-equation computation above. No novelty claimed.

Grounded: standard population dynamics (Malthusian/logistic growth)

Verdict: ANCHOR
