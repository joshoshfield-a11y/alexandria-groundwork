# Vigil Flame — Pre-registration: measurer-ι_t modulation of Born-rule probabilities

**Status: PRE-REGISTERED — user sign-off 2026-10-14. No data collected. No experiment executed.** Sign-off covers the design below including the pinning resolution (§1 pinning note); the honest flags (§7) stand as written. Arm B remains gated on Arm A surviving; nothing runs without lab resources and (for Arm B) ethics approval.

- Exemplar: idx 1, "Vigil Flame" (Foundational F1), verdict DEFINE-proposed (UNTESTED).
- Source hypothesis: `~/workspace/lexicon-ground/work/01-vigilflame-define.md`
- Related philosophy: `~/workspace/your_files/my-philosophy-complete.md` (C_t formalism, §II; differential prediction vs IIT, §VII; PROOF-1/2/3, §VIII)

---

## 1. Hypothesis (one paragraph)

Standard quantum theory says a projective measurement of observable with projectors {P_i} on state ρ yields outcome probabilities p_i = Tr(P_i ρ) — the Born rule — with no dependence on who or what performs the measurement. The Vigil Flame delta claims the measurer's consciousing measure enters the outcome probabilities: for a measurer with consciousing measure ι_t (defined per §2), the probability of outcome i is **p_i = Tr(P_i ρ) · (1 + ε·(ι_t − ῑ)·g_i) / Z**, where Z = Σ_j Tr(P_j ρ)·(1 + ε·(ι_t − ῑ)·g_j) normalizes, g_i is a pre-committed outcome-signed contrast (for a qubit, g_0 = +1, g_1 = −1), ῑ is the mean ι_t across measurer-sessions in the study, and ε is a single universal coupling constant. **The exact mathematical delta is the parameter ε: standard theory is the point hypothesis ε = 0; the Vigil Flame hypothesis is ε ≠ 0 with the sign and magnitude of the deviation tracking the measurer's ι_t.** At the operating point Tr(P_0 ρ) = Tr(P_1 ρ) = 1/2 this reduces to the clean prediction f_0 = (1 + ε(ι_t − ῑ))/2, i.e. the observed relative frequency shifts linearly in the measurer's consciousing measure.

*Pinning note (honesty): the define document writes w(ι_t(measurer)) as a factor common to all outcomes, which would cancel in normalization and predict nothing. That underspecification is resolved here by the outcome-signed linear model above — the minimal form that is both faithful to the stated idea (deviations from the Born rule correlated with the measurer's integration) and falsifiable. If this pinning is rejected, the hypothesis as written is vacuous and the operator falls back to ANCHOR.*

---

## 2. Operationalization of ι_t for the measurer

ι_t is "a differentiable integration measure, evolving across a hierarchy of timescales" (philosophy §II) — the richness-of-the-music component of C_t. What is measurable today differs by measurer class. Two measurer arms plus a null-control arm, analyzed separately and pre-committed to agree in sign for the hypothesis to survive.

**Arm A — AI agents with logged C_t (primary arm).** Measurers are software agents running the existing C_t profiler (philosophy §VIII, PROOF-1/2/3). Each agent's ι_t is the structural effective-rank measure ι_t v2 (computed from recurrent weights alone, drive-independent — the PROOF-3 instrument fix), plus its logged duet verdict (knowing-loop closed or open). Measurer selection spans the measured range: e.g. loop-closed planner agents (high ι_t, duet = 1) vs loop-open high-capacity agents (high ι_t v2, duet = 0 — the photodiode-array case, which the user's theory predicts behaves as non-consciousing) vs reactive agents (low ι_t, duet = 0). This arm is chosen because it is the only setting where ι_t is *already instrumented and logged* rather than proxied, it is cheap and exactly repeatable, and it directly tests the theory's own differential claim (loop structure matters, not raw integration). Honest caveat: this arm's validity stands or falls with the profiler's validity; a null here admits the reading that the agent was never causally upstream of outcome selection (see §6).

**Arm B — human subjects (secondary arm).** Measurers are adult human subjects; ι_t is operationalized by the perturbational complexity index (PCI) from TMS-EEG — the established, published perturbational measure of integration capacity (Massimini et al.), the closest existing instrument to "differentiable integration measure." ι_t is *manipulated within-subject* across two sessions: rested wakefulness (high PCI) vs 24-hour sleep-deprived wakefulness (documented PCI reduction), order counterbalanced. PCI is re-measured in the same session as the quantum trials to bind ι_t to the measurement act. This arm is chosen because humans are the biologically canonical high-ι_t case in the user's theory (philosophy §IX human rung) and within-subject manipulation controls inter-individual confounds. Honest caveats: PCI is a proxy, not ι_t itself; sleep deprivation is a coarse manipulation; this arm requires a quantum-optics lab, TMS-EEG, and ethics approval — it is the expensive arm and runs only if Arm A survives its decision rule (§4).

**Arm C — null control (automated trigger, no measurer).** The entire measurement chain is triggered by deterministic classical electronics with no agent or subject in the causal path. Expected: ε = 0 within error. This arm anchors apparatus bias; any nonzero deviation here is a veto on the whole setup, not evidence for the hypothesis.

*The "measurer" causal requirement:* for the hypothesis to be engaged, the measurer must be causally upstream of the outcome's registration — in Arm A the agent's logged process triggers the measurement window; in Arm B the subject initiates each trial block and attends to the apparatus. A subject merely present in the room does not count. This is pre-committed, not adjustable post hoc.

---

## 3. Experimental design

**Quantum system: photonic polarization qubits.** Justification: (i) room-temperature, no cryogenics; (ii) repetition rates of 10^4–10^6 trials/s make N = 10^6 per session a minutes-long run, giving sensitivity to ε ~ 10^−4 (§4); (iii) the cleanest possible operating point — prepare |+⟩ = (|H⟩+|V⟩)/√2, measure in the H/V basis, so Tr(P_i ρ) = 1/2 exactly and the predicted deviation is a pure frequency shift; (iv) there is published precedent for high-precision Born-rule tests on photonic platforms, so the calibration and systematic-error literature exists. Source: heralded single photons from SPDC (or attenuated laser with decoy characterization — pre-commit one and report g^(2)); state preparation fidelity verified by tomography to ≥ 0.999 before each session; measurement basis calibrated by extinction ratio.

**Trial structure.** Sessions are blocks of N = 2×10^6 trials at the 50/50 operating point. Measurer-sessions (one agent run, or one human session) are interleaved in randomized order; the measurer initiates each block (Arm A: agent's trigger call; Arm B: subject button press) and the outcomes are recorded automatically. Interleaved every 4th block: a calibration block with the automated trigger (Arm C) to track source drift.

**Conditions.** Arm A: K ≥ 16 measurer-sessions spanning at least three agent classes (loop-closed, loop-open-high-capacity, reactive), each agent's ι_t v2 and duet verdict logged before the session. Arm B: each subject contributes one rested and one sleep-deprived session (within-subject), K ≥ 12 subjects. Arm C: automated-trigger blocks throughout.

**Blinding.** Outcome data are recorded with session IDs only. The mapping from session ID to measurer identity and ι_t value is held sealed (hash-committed before data collection) and opened only after the analysis script has been run on blinded data. The analyst who writes the analysis code never sees unblinded ι_t values.

**Controls.**
- *Sham-measurement control (Arm B):* in a randomly chosen 20% of human blocks, the subject performs the identical initiation/attention actions but the recorded outcomes come from a classical hardware RNG while the photon source is shuttered. If frequency deviations track the subject's ι_t in sham blocks, the effect is an experimenter/attention artifact, not quantum — this is a pre-committed veto on Arm B.
- *No-signaling / marginal checks:* verify the H/V marginal is independent of block order, time-of-day, and (Arm B) which hand pressed the button; any dependence is a systematic, investigated before unblinding.
- *Source calibration:* tomography + extinction-ratio checks before each session; sessions failing the pre-set fidelity floor are discarded before unblinding (rule fixed in advance, applied blindly).

---

## 4. Analysis plan

**Primary test (pre-committed, run once on unblinded data).** Mixed-effects logistic regression on individual trial outcomes: outcome ~ ι_t(measurer) + (1 | session) + (1 | drift-block), binomial family, where ι_t is standardized within each arm. The coefficient of ι_t is the estimator of ε (at the 50/50 operating point the logistic slope equals the frequency-shift parameter to first order). Two-sided Wald test of H_0: ε = 0. **Significance threshold α = 0.005** (stringent, per the replication-crisis standard the user's own method demands — philosophy §VI).

**Power / required N.** With N = 2×10^6 trials per measurer-session at p = 1/2, per-session frequency SE ≈ 1/√(4N) ≈ 3.5×10^−4. With K = 16 sessions spanning standardized ι_t (unit variance), SE(ε̂) ≈ 3.5×10^−4/4 ≈ 8.8×10^−5, so the design has ≥ 80% power at α = 0.005 to detect |ε| ≥ 2.8×8.8×10^−5 ≈ **2.5×10^−4**. Pre-committed sensitivity floor: the study can resolve Born-rule deviations at the ~3×10^−4 level. (Arm B: K = 12 subjects × 2 sessions, paired within-subject — powered to detect |ε| ≥ ~4×10^−4; the exact paired-power calculation is fixed in the analysis script before data collection.)

**Pre-committed decision rule.**
- The hypothesis **survives** (proceeds to independent replication, still not "confirmed") iff: (i) the Arm A slope is significant at α = 0.005, (ii) the Arm B slope is significant at α = 0.005 *with the same sign* as Arm A, (iii) Arm C shows |ε̂_C| consistent with zero (|ε̂_C| < sensitivity floor), and (iv) the sham-control shows no ι_t-tracking deviation.
- The hypothesis is **falsified** iff Arm A fails (i) with power ≥ 0.9 at |ε| = 3×10^−4 — regardless of Arm B. (Arm A is the cheap, high-power, pre-instrumented arm; it carries the falsification burden.)
- Any other pattern (e.g., Arm A null but Arm B positive, sign disagreement, Arm C nonzero) is recorded as the pre-committed outcome it is — see §5 — and does not count as support.

---

## 5. Falsification criteria

The following kill the Vigil Flame delta, each pre-committed:

1. **The exemplar's own falsifier:** repeated trials across measurers of differing ι_t showing no correlation — i.e., Arm A returns ε̂ consistent with zero at the pre-committed power. **Consequence: the delta is dead and the operator falls back to ANCHOR** (Vigil Flame = standard projective measurement / Lüders rule / Born rule, documented relabel, no novelty claimed). The lexicon row is updated, not deleted.
2. **Artifact veto:** nonzero deviation in Arm C (automated trigger) or ι_t-tracking deviation in the sham blocks — the setup is measuring its own bias; no conclusion about the hypothesis is drawn and the apparatus is rebuilt or the program stops.
3. **Wrong kind of anomaly:** a real deviation (Arm C clean) that does *not* correlate with ι_t, or correlates with the wrong sign inconsistently across arms — falsifies *this* hypothesis (the delta is specifically ι_t-tracking); the anomaly is reported as an unverified finding, not as support.
4. **Replication failure:** a surviving result that an independent lab, running this exact pre-registration, fails to reproduce at α = 0.005 — the hypothesis returns to UNTESTED/failed status; one positive run is never a confirmation.

---

## 6. Limitations — what this cannot show even if positive

- **Correlation is not causation.** A positive ε̂ shows Born-rule deviation tracking an integration index; it does not show that consciousing *causes* collapse, nor does it distinguish "the measurer's integration modulates outcome selection" from "some unknown physical variable covaries with both ι_t and detector behavior." A mechanism is a separate research program.
- **ι_t is indexed, not identified.** PCI (Arm B) is a proxy; ι_t v2 (Arm A) is a structural approximation labeled as such since PROOF-3. A positive result validates the *index's* predictive power, not the full C_t metaphysics.
- **The causal-upstream assumption is load-bearing.** If collapse (or effective outcome selection via decoherence) is already settled in the detector before the measurer acts, the hypothesis is untestable in this design and a null result says nothing about the idea — only about the design. This is stated now so it cannot become a post-hoc rescue.
- **Scope of the null.** A null falsifies the linear signed-contrast model within |ε| ≥ 3×10^−4 over the tested ι_t range. It does not rule out observer-dependent effects of other functional forms, at smaller magnitude, or in other degrees of freedom.
- **One lab, one apparatus.** Even a surviving result is a candidate awaiting independent replication (§5.4), per the user's own chamber 3 (philosophy §VI).

---

## References (grounding)

- Nielsen & Chuang, *Quantum Computation and Quantum Information*, Ch. 2 — projective measurement, Lüders rule, Born rule (the ANCHOR the delta departs from).
- Massimini et al., perturbational complexity index (PCI) — the Arm B ι_t proxy.
- Precedent: high-precision photonic Born-rule tests (Sorkin-parameter / multi-path interference bounds) — calibration and systematics literature.
- Internal: `workspace/lexicon-ground/work/01-vigilflame-define.md` (hypothesis source); `workspace/your_files/my-philosophy-complete.md` §II (C_t, ι_t), §VII (differential prediction), §VIII (PROOF-1/2/3 instruments).

---

*End of pre-registration. PRE-REGISTERED 2026-10-14 (user sign-off); no data collected, no experiment executed.*
