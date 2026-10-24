
# Persistent Notes App

## Purpose

Create, list, view, and delete simple notes saved to disk.

**Difficulty:** Intermediate  
**Main concepts:** file format, input parsing, CRUD, persistence, validation

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

1. Define a simple record format.
2. Implement add and list.
3. Implement viewing by ID.
4. Implement deletion or marking a note as deleted.
5. Handle missing or malformed data files.

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

- [ ] Notes survive restarting the program.
- [ ] Malformed records do not crash the application.
- [ ] IDs are unique for the chosen storage design.
- [ ] User text cannot accidentally break the file format.

Also:
- [ ] I can build and run it from the documented commands.
- [ ] I can explain the important functions without reading a tutorial aloud.
- [ ] I added one feature or variation of my own.
- [ ] I recorded one bug and how I diagnosed it in `NOTES.md`.

## Common stuck points

- **Plain delimiter formats fail if text contains the delimiter; escape it or choose a format with clear rules.:** Plain delimiter formats fail if text contains the delimiter; escape it or choose a format with clear rules.
- **Write to a temporary file and rename for safer whole-file updates where appropriate.:** Write to a temporary file and rename for safer whole-file updates where appropriate.
- **Always check file and allocation errors.:** Always check file and allocation errors.

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

Keep version one simple: one note per line with a clearly documented restriction, then improve the format.

## Completion log

- Started:
- Finished:
- Most useful concept:
- Hardest bug:
- What I can now do without help:
- Next project:
