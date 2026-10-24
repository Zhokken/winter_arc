# File Analyzer

## Purpose

Summarize a file's size and content characteristics.

**Difficulty:** Intermediate  
**Main concepts:** file I/O, counters, modular functions, error handling

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

1. Accept a filename from argv.
2. Report whether the file opens and how many bytes are read.
3. Count lines, whitespace-separated words, and byte frequencies.
4. Separate reading from summary printing.
5. Document encoding assumptions.

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

- [ ] Works for empty and non-empty files.
- [ ] Read failures are reported.
- [ ] Counters use suitable types and do not overflow silently for supported inputs.
- [ ] Input path is not hard-coded.

Also:
- [ ] I can build and run it from the documented commands.
- [ ] I can explain the important functions without reading a tutorial aloud.
- [ ] I added one feature or variation of my own.
- [ ] I recorded one bug and how I diagnosed it in `NOTES.md`.

## Common stuck points

- **Text bytes are not the same as Unicode characters; describe your output as byte counts unless you implement decoding.:** Text bytes are not the same as Unicode characters; describe your output as byte counts unless you implement decoding.
- **Do not use feof as the loop condition; check the read result.:** Do not use feof as the loop condition; check the read result.
- **Large files require types appropriate for the file size.:** Large files require types appropriate for the file size.

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

Keep each counter's definition explicit so results can be tested.

## Completion log

- Started:
- Finished:
- Most useful concept:
- Hardest bug:
- What I can now do without help:
- Next project:
