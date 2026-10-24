# Terminal Text Editor

## Purpose

Create a small terminal text editor inspired by kilo.

**Difficulty:** Advanced  
**Main concepts:** terminal raw mode, key input, screen redraw, text buffer, file save

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

1. Read the kilo tutorial and note each subsystem.
2. Implement terminal setup/restore safely.
3. Display a text buffer and cursor.
4. Support movement and insertion.
5. Support opening and saving a file.
6. Handle resize and quit without corrupting the terminal state.

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

- [ ] Terminal settings are restored on normal exit and errors.
- [ ] Cursor movement respects buffer bounds.
- [ ] Saving writes the intended content.
- [ ] Empty files and long lines are handled according to documented limits.

Also:
- [ ] I can build and run it from the documented commands.
- [ ] I can explain the important functions without reading a tutorial aloud.
- [ ] I added one feature or variation of my own.
- [ ] I recorded one bug and how I diagnosed it in `NOTES.md`.

## Common stuck points

- **Terminal left in raw mode:** ensure cleanup paths restore settings; test interruption behavior carefully.
- **Screen artifacts:** centralize redraw logic and clear/redraw the correct region.
- **Buffer indexing bugs:** test empty, one-character, and end-of-line cases.

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

Reference: https://viewsourcecode.org/snaptoken/kilo/ . Build one subsystem at a time.

## Completion log

- Started:
- Finished:
- Most useful concept:
- Hardest bug:
- What I can now do without help:
- Next project:
