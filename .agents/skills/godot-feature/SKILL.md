---
name: godot-feature
description: Implement a small, testable Godot feature in Cauldron Crops Prototype 0. Use when adding or changing a bounded gameplay/system feature that should be integrated into the existing project and verified in the running game.
---

# Godot Feature

Use this skill for one bounded feature at a time.

## Before coding

Read:

- the relevant section of `PROTOTYPE_0.md`;
- any relevant domain documentation;
- the existing scripts/scenes directly involved.

Do not read the entire legacy repository unless the task explicitly requires archaeology.

State the intended change internally as:

**input → behavior → output → verification**

If the requested feature is larger than one coherent slice, reduce it to the smallest useful slice before coding.

## Implementation rules

- Follow the architecture already present in the new repository.
- Prefer composition over global managers.
- Keep gameplay logic out of UI where possible.
- Keep item data separate from systems that consume it.
- Add no unrelated systems.
- Do not migrate legacy architecture wholesale.
- Reuse a legacy implementation only after understanding and isolating the useful behavior.

When adding a new data model, make it compatible with the existing item/tag/aspect direction instead of inventing a parallel representation.

## Verification

After implementation:

1. Run the project's available automated tests.
2. Open/run the affected Godot scene or project.
3. Exercise the feature through the player-facing flow.
4. Check the main success case.
5. Check at least one invalid, edge, or failure case relevant to the feature.
6. Fix any issue found before finishing.

If a required verification cannot be run, say exactly what could not be verified.

## Completion criteria

A feature is complete only when:

- the intended behavior works in the running project;
- relevant tests pass;
- no unnecessary systems were introduced;
- the diff is limited to the task;
- the implementation respects Prototype 0 scope.

At the end, report:

- what changed;
- what was tested;
- any limitation.
