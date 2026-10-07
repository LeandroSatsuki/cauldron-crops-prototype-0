---
name: godot-debug
description: Diagnose and fix reproducible Godot bugs in Cauldron Crops Prototype 0. Use when behavior is broken, inconsistent, crashes, or fails a known test or gameplay flow.
---

# Godot Debug

Treat debugging as diagnosis first, patch second.

## Before changing code

Identify:

- expected behavior;
- actual behavior;
- reproduction steps;
- affected scene/system;
- first observable failure.

Read the smallest relevant set of files and documentation.

Do not start with a broad refactor.

## Investigation

Follow evidence in this order:

1. Reproduce the problem.
2. Capture the first meaningful error or incorrect state.
3. Trace ownership of that state.
4. Find the smallest root cause.
5. Verify that the proposed fix addresses the cause rather than the symptom.

Check for:

- duplicated state;
- signal connections;
- node lifecycle;
- scene ownership;
- incorrect resource references;
- timing/order dependencies;
- stale data;
- hidden global state;
- incorrect assumptions imported from the legacy project.

## Fix

Make the smallest robust correction.

Do not add a new manager, abstraction, fallback, or global state merely to hide the bug.

Do not change unrelated behavior.

## Verification

After the fix:

1. Reproduce the original failure.
2. Confirm the failure is gone.
3. Run relevant automated tests.
4. Exercise the normal gameplay path.
5. Exercise the nearest relevant edge case.
6. Review the diff for accidental changes.

If the bug cannot be reproduced locally, do not claim it was fixed with certainty. Document what was inspected and what remains unverified.

## Completion criteria

A debugging task is complete when the original failure is reproduced and resolved, or when the evidence clearly shows why reproduction is currently impossible and the investigation has identified the most likely cause.

Report:

- root cause;
- files changed;
- verification performed;
- remaining uncertainty, if any.
