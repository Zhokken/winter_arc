# Word and Line Counter

## Purpose

Count bytes, lines, and whitespace-separated words.

**Difficulty:** Beginner–intermediate  
**Main concepts:** character streams, EOF, ctype.h, counting rules

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

1. Read a file character by character.
2. Count bytes or characters as defined by your implementation.
3. Count newline characters.
4. Define a word as a run of non-whitespace characters and count transitions into words.
5. Support multiple files if desired.

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

- [ ] Empty file reports zero.
- [ ] A final line without a newline is handled according to your documented line-count rule.
- [ ] Repeated spaces do not create extra words.
- [ ] EOF is not confused with an ordinary character.

Also:
- [ ] I can build and run it from the documented commands.
- [ ] I can explain the important functions without reading a tutorial aloud.
- [ ] I added one feature or variation of my own.
- [ ] I recorded one bug and how I diagnosed it in `NOTES.md`.

## Common stuck points

- **Use int for the result of fgetc so EOF can be represented.:** Use int for the result of fgetc so EOF can be represented.
- **Pass character values safely to isspace:** cast to unsigned char unless the value is EOF.
- **State your counting convention; different tools may define line counts differently.:** State your counting convention; different tools may define line counts differently.

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

Write the rules in plain language before writing the loop.

## Completion log

- Started:
- Finished:
- Most useful concept:
- Hardest bug:
- What I can now do without help:
- Next project:
