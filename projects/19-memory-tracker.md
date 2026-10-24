# Memory Tracking Utility

## Purpose

Wrap allocations to count active allocations and bytes.

**Difficulty:** Intermediate  
**Main concepts:** allocation wrappers, metadata, cleanup, limits of leak tracking

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

1. Create wrapper functions around malloc/free.
2. Track allocation count and requested bytes.
3. Track frees and active allocations.
4. Report outstanding allocations at program exit.
5. Test successful and failed allocations.
6. Document limitations.

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

- [ ] Counters do not underflow.
- [ ] Freeing NULL follows documented behavior.
- [ ] The tracker itself does not recursively track its own bookkeeping unintentionally.
- [ ] Test cases demonstrate expected counts.

Also:
- [ ] I can build and run it from the documented commands.
- [ ] I can explain the important functions without reading a tutorial aloud.
- [ ] I added one feature or variation of my own.
- [ ] I recorded one bug and how I diagnosed it in `NOTES.md`.

## Common stuck points

- **Tracking metadata can itself allocate memory; avoid recursive tracking or use a simple fixed registry for a learning version.:** Tracking metadata can itself allocate memory; avoid recursive tracking or use a simple fixed registry for a learning version.
- **A wrapper cannot safely know the size of an arbitrary pointer unless it records that information.:** A wrapper cannot safely know the size of an arbitrary pointer unless it records that information.
- **This tool is educational, not a replacement for sanitizers or Valgrind.:** This tool is educational, not a replacement for sanitizers or Valgrind.

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

Use it only in your own test programs; do not redefine global allocation behavior prematurely.

## Completion log

- Started:
- Finished:
- Most useful concept:
- Hardest bug:
- What I can now do without help:
- Next project:
