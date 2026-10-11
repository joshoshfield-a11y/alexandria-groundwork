# Charter

## What this repo is

A workshop for answering one question about each Alexandria core: **does the math do work, or does it decorate?**

The cores under test:

| Core | Source of truth | This repo asks |
|---|---|---|
| 72 field operators | `alexandria-engine` (machinery) + UT-ITD §II (claims) | Which mappings are derivations, which are analogies? |
| 936-lens context tensor `[L]` | UT-ITD §III | Are the 13 drivers defined enough to compute with? |
| Syntactic engine + SOPs | UT-ITD §IV–V | Do the SOPs make predictions that differ from the null? |
| RGH 5-chamber pipeline | `RGH-Reality-Grounding-Harness` | Does the code run, and can it reject unfalsifiable claims? |
| Location Baseline Awareness | UT-ITD §VI | What would a controlled test look like, preregistered? |

## What this repo is not

- Not a rewrite of the Codex. The metaphysical register is out of scope by design.
- Not a second copy of the engine. `alexandria-engine` remains the machinery; this repo holds verdicts about it.
- Not a defense brief. Findings that weaken a claim get recorded the same as findings that strengthen it.

## Verdict grades

- **VERIFIED** — ran it / measured it, evidence on file.
- **PARTIAL** — some evidence; gaps explicitly named.
- **SCHEMATIC** — described in words, not defined in math or code.
- **ANALOGY** — evocative mapping with no demonstrated mechanism.
- **UNTESTED** — no data either way; do not mistake for disproven.

## Definition of done (per core)

A core is "hardened" when every one of its load-bearing claims carries a grade, every ANALOGY/SCHEMATIC is either promoted (with derivation or data) or relabeled honestly, and the audit trail is reproducible from this repo alone.
