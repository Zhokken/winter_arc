# Retro Horror Prototype

## Purpose

Create a short atmospheric game slice rather than a huge unfinished game.

**Difficulty:** Intermediate  
**Main concepts:** scene state, interaction, asset loading, audio, level design

## What you are building

Build a working first version before adding optional features. This document gives you the target and the steps, but intentionally does not give you a full copy-paste solution. You learn more by designing and implementing each milestone.

## Before coding

Create a folder for this project and add:
- `README.md` — this guide, plus your own changes and build instructions.
- `NOTES.md` — decisions, bugs, fixes, and concepts you learned.
- source file(s), added as needed.
- `Makefile` once the project has multiple files or dependencies.

Write down:
1. What does the program do?
2. What input does it accept?
3. What should happen when input is invalid?
4. What is the smallest version that would count as working?

## Milestones

1. Define one small level and one objective.
2. Create player movement and collision.
3. Add an interactable object with a prompt.
4. Add a door/exit condition and one ending.
5. Add lighting/color/audio atmosphere using manageable assets.
6. Write a short playtest checklist.

Do not begin the next milestone until the current one works and you can explain it.

## Suggested design process

1. Write pseudocode in plain language.
2. Identify the data the program must remember.
3. Split responsibilities into small functions.
4. Implement the simplest working path.
5. Compile with warnings and fix them.
6. Test one normal case and one edge case.
7. Refactor only after behavior is correct.

## Definition of done

- [ ] The player can complete the objective from start to end.
- [ ] All assets load from documented paths.
- [ ] Missing assets fail gracefully or show an error.
- [ ] The game can be restarted.

Also:
- [ ] I can build and run it from the documented commands.
- [ ] I can explain the important functions without reading a tutorial aloud.
- [ ] I added one feature or variation of my own.
- [ ] I recorded one bug and how I diagnosed it in `NOTES.md`.

## Common stuck points

- **Scope grows endlessly:** freeze the level size and feature list for version one.
- **Asset paths fail from another directory:** define a working-directory convention or use a resource path strategy.
- **Atmosphere does not replace readable interaction cues; test whether a player knows what to do.:** Atmosphere does not replace readable interaction cues; test whether a player knows what to do.

## Example debugging note

```text
Problem:
I expected:
What actually happened:
Smallest reproduction:
Cause:
Fix:
How I verified the fix:
What I learned:
```

## Hints, not solutions

If you get stuck:
1. Identify which milestone is failing.
2. Reduce it to the smallest possible case.
3. Print or inspect the values that control the failing behavior.
4. Check the related section in `reference/C_CHEATSHEET.md`, `reference/DEBUGGING.md`, or `reference/MEMORY.md`.
5. Ask for a hint about the next step rather than asking for the whole project to be written.

## Stretch challenge

Make a 5-minute playable slice before adding extra levels, enemies, or VHS effects.

## Completion log

- Started:
- Finished:
- Most useful concept:
- Hardest bug:
- What I can now do without help:
- Next project:
