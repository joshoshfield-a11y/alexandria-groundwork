# Exemplar — ANCHOR: idx 29, "Dawn Spark" (Foundational)

Date: 2026-10-12.

## Canon row

- idx 29 · Foundational · Automata-Theoretic State · codex "Dawn Spark"
- Technical (v3.1): Impulse
- Placeholder (retired): λ=sin²(29)=0.44041, κ=log₂(30)=4.906891, H_max=0.98973 — scaffold values, no meaning claimed

## Hardened spec

1. **State space:** linear time-invariant systems with input x(t)
   and output y(t); distributions over time for the idealized kick.
2. **Computable form:** the Dirac impulse δ(t), with the sifting
   property ∫f(t)δ(t−a)dt = f(a); system response to an arbitrary
   input is the convolution y = h ∗ x with the impulse response
   h(t). Worked example: RC low-pass filter,
   h(t) = (1/RC)e^{−t/RC}θ(t); a unit voltage kick produces an
   output decaying with time constant τ = RC. Mechanically:
   a 70 kg runner stopping from 5 m/s absorbs impulse
   J = Δp = 350 N·s — the same integral-of-force over the brief
   braking interval.
3. **Measurable quantity:** mechanical impulse J = ∫F dt in
   newton-seconds (kg·m/s); signal impulses in volt-seconds.
   Instrument: force transducer with time integration, or a
   calibrated pulser into an oscilloscope.
4. **Standard theory:** distribution theory (Dirac delta);
   linear systems theory — the impulse response fully
   characterizes any LTI system; the impulse-momentum theorem
   J = Δp.
5. **Delta assessment:** none. This operator is the impulse —
   the infinitesimally brief, finite-effect excitation and its
   system response — under a mythic name.

## Verdict: ANCHOR

Relabel admitted. "Dawn Spark" is the impulse: the delta-function
kick whose response characterizes the system, and the
impulse-momentum relation of mechanics. The placeholder λ/κ/H_max
are retired for this row; the operator's "application" is the
impulse-response computation above. No novelty claimed.

Grounded: Oppenheim & Schafer (LTI impulse response); standard mechanics (J = Δp)

Verdict: ANCHOR
