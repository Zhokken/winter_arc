# Text Adventure

## Purpose

Build a small branching story with clear program state.

**Difficulty:** Beginner  
**Main concepts:** functions, enums, state, branching, input

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

1. Write a story with three locations or scenes.
2. Represent the current scene with an enum or integer constants.
3. Put each scene's choices in functions.
4. Add one item or flag that changes a later scene.
5. Add a restart or ending.

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

- [x] Every choice leads to a valid scene or a clear error.
- [ ] Impossible transitions are prevented.
- [x] Story state is kept separate from printing where practical.

Also:
- [x] I can build and run it from the documented commands.
- [x] I can explain the important functions without reading a tutorial aloud.
- [ ] I added one feature or variation of my own.
- [x] I recorded one bug and how I diagnosed it in `NOTES.md`.

## Common stuck points

- **Many nested if statements:** extract functions or use a state variable and switch.
- **Choice skipped:** inspect input parsing and leftover newline behavior.
- **State becomes inconsistent:** write down which variables define the current situation.

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

Draw the scenes and transitions on paper before coding.

## Completion log

- Started:
- Finished:
- Most useful concept:
- Hardest bug:
- What I can now do without help:
- Next project:
