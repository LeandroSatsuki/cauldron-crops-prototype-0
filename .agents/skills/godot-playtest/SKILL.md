---
name: godot-playtest
description: Playtest a bounded Cauldron Crops Prototype 0 gameplay flow in the running Godot project and report defects, friction, and scope issues. Use when validating whether an implemented slice actually works for a player rather than only compiling.
---

# Godot Playtest

This skill validates player-facing behavior.

It is not a substitute for automated tests and it is not a request to redesign the game while testing.

## Before testing

Read:

- the relevant Prototype 0 acceptance criteria;
- the feature's design documentation;
- the affected scene or system structure.

Define a short test flow before execution.

Example:

**start → move → interact → plant → wait → harvest → inspect result**

Keep the flow bounded.

## During playtest

Check four things:

### Function

Does the expected action work?

### Clarity

Can the player understand what can be interacted with and what happened?

### Continuity

Does the next action follow naturally from the previous result?

### Scope

Did implementation accidentally introduce systems or dependencies that Prototype 0 does not need?

Do not invent new design requirements during the test.

## Failure classification

Classify findings as:

- **blocking** — prevents the tested flow from completing;
- **functional** — behavior is wrong but the flow may continue;
- **UX** — behavior works but is unclear or unnecessarily difficult;
- **scope** — implementation introduced unnecessary complexity/dependency;
- **visual** — readability or coherence problem;
- **design question** — requires a human design decision and should not be silently changed.

## Verification

For each tested flow, record:

- starting state;
- action;
- expected result;
- observed result;
- classification;
- severity.

Retest after fixes.

A successful compile is not a successful playtest.

## Completion criteria

Finish with a concise report containing:

- tested flow;
- pass/fail result;
- blocking issues;
- non-blocking findings;
- design questions;
- recommended next action.

Do not fix unrelated findings discovered during a playtest.
