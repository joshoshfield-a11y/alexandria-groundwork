# Runbook — Location Baseline Awareness study

How a human actually runs the study in PROTOCOL.md. No lab required — phone + free apps.

## What you need

- A phone with a camera-based HRV app (e.g. HRV4Training, Welltory, or any app that exports RMSSD from a 5-min seated PPG reading — pick one and use it for every measurement).
- The MAAS questionnaire (15 items, free, ~3 min). Print it or use any survey form.
- A 20-min audio guide you record once: Arm A script (3 steps as written in UT-ITD §VI) and Arm B script (box breathing + body scan, no nullification/interference-pattern framing). Same voice, same length, same background silence.

## Measurement discipline (this is where studies live or die)

- **HRV:** same time of day (±1h), seated, back supported, no caffeine 2h prior, no exercise 12h prior, 2-min settle before the 5-min read. Record RMSSD only — ignore the app's "readiness scores".
- **MAAS:** pre (day 0), post (day 15), follow-up (day 45). Same quiet setting. Don't look at your previous answers.
- **Daily log (1 min):** date, arm, minutes practiced, "raw sensation vividness" 0–10, any adverse event (dissociation, anxiety spike, unusual distress).

## The scripts (keep them fixed — no improvising mid-study)

- **Arm A (full protocol):** 5 min lexical nullification guidance ("let the names of things drop; attend to what remains") → 7 min field entanglement ("extend attention to the room's edge; feel touch as interference, pressure rising and falling like waves") → 8 min anchor calibration (box breathing 4-4-4-4, attention on raw tactile oscillation).
- **Arm B (active control):** 10 min box breathing 4-4-4-4 → 10 min body scan (attention moving slowly joint to joint, no framing language).
- **Arm C:** no audio; same measurement schedule.

## Stop rules

- 2+ related adverse events in an arm → pause that arm, review before resuming.
- Missed >4 practice days → excluded from per-protocol analysis (kept in intention-to-treat).

## Analysis (do it blind)

1. Export the daily logs + MAAS + RMSSD into one sheet.
2. Have someone else (or a coin flip you don't look at) label the arms; analyze as X/Y/Z.
3. ANCOVA: post ~ arm + pre, for MAAS and RMSSD separately. Intention-to-treat first, per-protocol second.
4. Unblind only after the numbers are computed.
5. Read the interpretation ladder in PROTOCOL.md *before* unblinding — decide which branch you're on from the numbers, not from how the practice felt.

## What success and failure look like (concrete)

- **Protocol wins:** Arm A beats B on both metrics at the preregistered thresholds. → Replicate with a bigger n.
- **Breathing wins:** A ≈ B > C. → The framework's framing is inert; keep the breathing, drop the metaphysics from the instructions.
- **Nothing wins:** all arms ≈ equal. → The §VI metrics claim fails as stated. Back to the drawing board, not to a reinterpretation.
