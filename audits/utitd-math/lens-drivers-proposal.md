# The 13 [L] Drivers — Typed Proposal

Status: PROPOSAL. UT-ITD §III lists 13 drivers with placeholder "mappings" (a "Resonant Matrix" with no matrix, "[7] Matrix", "Ψ = 1"). For `[L]_tensor` to be computable, each driver needs to be a typed function `d_i : X × E → R` — a number you can actually calculate from the state. This file proposes all 13.

Recall the role (master-equation-proposal.md): `L ∈ R^13` parametrizes the transition kernel `K_L`. The drivers are the context measurements that select which transitions are possible.

## The 13, typed

**d1 — Structural coupling** (I, Structural Rules). `λ₂`, the algebraic connectivity of the system's adjacency graph (second-smallest Laplacian eigenvalue). 0 = disconnected; larger = harder to fragment. *Compute:* from the adjacency matrix. *Status: READY.*

**d2 — Dominant mode** (II, Resonant Modes). Peak frequency of the system's activity power spectrum (FFT of the state time series); if no peak exceeds the noise floor, report spectral entropy instead and flag it. *Compute:* FFT. *Status: READY.*

**d3 — Kinetic drive** (III, Kinetic Feedback). `‖F‖`, magnitude of the net generalized force on the state — in physical domains literally F=ma; in abstract domains, the gradient magnitude of whatever potential drives state change (write the potential down). *Status: READY once the potential is named.*

**d4 — Net flux** (IV, Network Flux). `∇·J`, divergence of the flow field: inflow minus outflow rate of the conserved quantity (mass, money, messages). *Compute:* from flow measurements. *Status: READY where a flow is defined.*

**d5 — Syntropy rate** (V, Syntropy Rate). `-dS/dt` of the system *minus* the erasure/export ledger — order produced, with the entropy exported to the environment itemized (Landauer: ≥ kT ln 2 per bit). A syntropy number reported without its export ledger is rejected by construction. *Status: READY, with the ledger mandatory.*

**d6 — Reproduction number** (VI, Viral Density). `R₀`: mean secondary adoptions per adopter. The document's "K > 1" is exactly the epidemic threshold; define K := R₀ and the driver is the measured value, not the inequality. *Compute:* from adoption time series. *Status: READY.*

**d7 — Filter strength** (VII, Transformation Matrix). `‖T‖`, the operator norm of the frame-change/filter map — how much the interpretive filter (cultural, philosophical, sensorimotor) distorts the representation. A filter is a map; its norm is its strength. *Hard part: the map T must be written down per application. Status: NEEDS-WORK.*

**d8 — Selection rate** (VIII, "Wavefunction Collapse"). Probability per unit time that the potential set resolves to an outcome — the measurement/decision rate. In master-equation terms: how often `c_Ψ` is applied. This is deliberately the *weak* reading (a rate, not a metaphysics); the strong Ψ claim lives in the selection functional, not in this driver. *Compute:* count resolutions per unit time. *Status: READY.*

**d9 — Geometric complexity** (IX). Box-counting dimension estimate `D` of the state trajectory or spatial pattern. *Compute:* standard algorithms. *Status: READY.*

**d10 — Constraint saturation** (X, Boundary Conditions). Feasible-set volume fraction in [0,1]: 1 = unconstrained, →0 = fully pinned by scope/scale/duration limits. *Compute:* from the constraint set. *Status: READY once constraints are listed.*

**d11 — Novelty rate** (XI, Generative Function). Distinct new artifacts/states per unit time, normalized by activity — needs a fixed similarity threshold for "novel", stated up front. *Hard part: the threshold is a judgment call; preregister it. Status: NEEDS-WORK.*

**d12 — Quality factor** (XII). `Q = 2π × (energy stored)/(energy dissipated per cycle)`, or generally the signal-to-loss ratio of the dominant mode. *Compute:* from d2's spectrum. *Status: READY.*

**d13 — Terminal proximity** (XIII, Limit State). `s ∈ [0,1]`: normalized distance to the system's absorbing regime — 0 = at the sink (∅: depleted, thermalized, bankrupt), 1 = unbounded growth (∞). Defined per-domain (a battery's s is charge fraction; a market's is distance to saturation). *"∅ or ∞" as written is a disjunction, not a definition; this replaces it with a number. Status: NEEDS-WORK (domain-specific).*

## Score

READY or near-ready: d1, d2, d3, d4, d5, d6, d8, d9, d10, d12 (10 of 13). NEEDS-WORK: d7 (write the filter map), d11 (preregister the novelty threshold), d13 (define per domain).

## What this unlocks

With these typed, `[L]_tensor` becomes a 13-vector you can actually compute per system per timestep — which means `K_L` can be fit to data, which means the master equation's out-of-support test for paracausality can actually run. The three NEEDS-WORK drivers are now the precise locations where the framework is still philosophy; everything else is engineering.
