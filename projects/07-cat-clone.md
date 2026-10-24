# cat Clone

## Purpose

Read one or more files and print their contents.

**Difficulty:** Beginner–intermediate  
**Main concepts:** argc/argv, FILE, fopen, fread or fgetc, perror

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

1. Print usage when no filenames are supplied.
2. Open each file in read mode.
3. Copy bytes to stdout.
4. Handle missing/unreadable files and continue or stop according to documented policy.
5. Optional: support stdin when filename is '-'.

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

- [ ] Small text files print correctly.
- [ ] Multiple files are processed in order.
- [ ] Missing file produces a useful error.
- [ ] Binary-safe byte copying works if you use byte-oriented I/O.

Also:
- [ ] I can build and run it from the documented commands.
- [ ] I can explain the important functions without reading a tutorial aloud.
- [ ] I added one feature or variation of my own.
- [ ] I recorded one bug and how I diagnosed it in `NOTES.md`.

## Common stuck points

- **fopen returns NULL on failure; never use the FILE pointer before checking.:** fopen returns NULL on failure; never use the FILE pointer before checking.
- **Use ferror to distinguish read errors from normal EOF when relevant.:** Use ferror to distinguish read errors from normal EOF when relevant.
- **Do not assume one read returns an entire file.:** Do not assume one read returns an entire file.

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

Start with one file and fgetc; later consider buffered fread for efficiency.

## Completion log

- Started:
- Finished:
- Most useful concept:
- Hardest bug:
- What I can now do without help:
- Next project:
