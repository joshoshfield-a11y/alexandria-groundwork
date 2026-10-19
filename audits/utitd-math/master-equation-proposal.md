# Master Equation — Reconstruction Proposal

Status: PROPOSAL, not source text. UT-ITD §1.1 names five quantities but writes no relation between them. This file proposes the minimal typed formalization that would make the framework testable. Everything here is falsifiable scaffolding — adopt, modify, or reject, but don't mistake the proposal for the original.

## Types

- `S_f(t) ∈ X` — the finite/observed state. `X` is the measurable state space (whatever the domain: positions, prices, survey scores).
- `S_a(t) ∈ E` — the absorptive component: dissipative variables (noise, friction, loss) with their own dynamics.
- `S_d(t) ⊆ P(X)` — the divergent component: the set of potential next states. Typed as a subset of the power set, i.e. "the alternatives currently on the table".
- `[L]_tensor`, 13 drivers → `L ∈ R^13` parametrizes a transition kernel `K_L : X × E → P(X)`. The "curving of the probability field" is just: context selects which transitions are possible.
- `Σ(A_kernel)` — the active operators `{A_i}`. Each `A_i` is a map on states; the "summation" is application: the kernel factors through them, `K_L = A_{i_k} ∘ … ∘ A_{i_1}` (or a weighted mixture — pick one and write it down).
- `Ψ_intent` — two readings, and the framework must choose:
  - **Weak (honest default):** a control signal `u(t) ∈ U`, ordinary agency — same role as `u` in `ẋ = f(x,u,t)`.
  - **Strong (the actual claim):** a selection functional `c_Ψ : P(X) → X`, choosing within the potential set. Agency as choice, formalized.
- `T_p` — the projector `T_p : P(X) × E → X`: resolves a potential set plus dissipative state into one observed outcome (measurement, collapse, decision — the domain names it).

## The equation

```
S_d(t+1)  =  K_L( S_f(t), S_a(t) )        # context + dissipation → possibilities
S_f(t+1)  =  T_p( c_Ψ( S_d(t+1) ), S_a(t) ) # intent selects, projector resolves
```

Two lines. Everything in §1.1 now has a type and a job.

## Why this matters: "paracausal" finally has a definition

Under this formalization, the strong claim (Op 61, SOP-CHRONO-001) is exactly:

> **An observed transition with `S_f(t+1) ∉ support( K_L(·) )`** — the outcome lies outside the possibility set the context kernel allowed.

That is a real falsifier. It converts "manifestation of statistically unlikely outcomes" from a slogan into a statistical test: fit `K_L` to baseline data, then count out-of-support transitions under the protocol vs control. If the count doesn't exceed the kernel's own tail, there is no paracausality — only unlikely outcomes, which conventional stochastic models already produce.

## Thermodynamic budget (non-negotiable)

Any "syntropy harvest" (Op 60, SOP-ECO-001) is order extraction and must pay Landauer's price: erasing/extracting one bit costs at least `kT ln 2`, booked to `S_a`. Constraint:

```
ΔS_total = ΔS_sys + ΔS_env ≥ 0, with the harvest's entropy export named explicitly.
```

A syntropy claim with no identified entropy export is a THERMODYNAMIC_VIOLATION by construction — no experiment needed. This is the cheapest filter in the whole program: it kills perpetual-harvest readings before they cost lab time.

## What this proposal concedes

Written this way, the framework reduces to **a controlled stochastic system with an explicit choice functional** — i.e., standard stochastic control theory plus agency formalized as selection within a possibility set. That is not an insult: it's the bridge the review asked for. The "new physics", if any, lives in exactly one place: out-of-support transitions. Everything else is vocabulary — useful vocabulary, but vocabulary.

## Open decisions for the author

1. Is `Ψ_intent` the weak control signal, the strong selection functional, or both at different scales? Pick one per claim.
2. Is `Σ(A_kernel)` composition or mixture? Write it down.
3. What are the 13 drivers as functions `d_i : X × E → R`? Until three of them are written, `[L]_tensor` stays SCHEMATIC.
4. Does any SOP predict an out-of-support transition rate above the kernel tail? Name it — that's the experiment.
