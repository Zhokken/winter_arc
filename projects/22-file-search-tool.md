# File Search Tool

## Purpose

Search files for a text pattern or filename match.

**Difficulty:** Intermediate  
**Main concepts:** directory traversal, paths, file I/O, filtering, errors

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

1. Accept a starting directory and search term.
2. Search file contents or filenames—choose one first.
3. Print matching path and line number where applicable.
4. Handle unreadable files and directories.
5. Add case-sensitive/case-insensitive mode if desired.

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

- [ ] Search works in nested folders if recursion is implemented.
- [ ] Unreadable files do not crash the tool.
- [ ] Paths with spaces are handled as paths, not shell commands.
- [ ] Search results identify the source file.

Also:
- [ ] I can build and run it from the documented commands.
- [ ] I can explain the important functions without reading a tutorial aloud.
- [ ] I added one feature or variation of my own.
- [ ] I recorded one bug and how I diagnosed it in `NOTES.md`.

## Common stuck points

- **Do not build shell command strings from user input and pass them to system(); use filesystem APIs.:** Do not build shell command strings from user input and pass them to system(); use filesystem APIs.
- **Recursive traversal can loop if symlinks are followed carelessly; define symlink policy.:** Recursive traversal can loop if symlinks are followed carelessly; define symlink policy.
- **Large files need streaming rather than loading everything into memory.:** Large files need streaming rather than loading everything into memory.

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

Build filename search first, then content search, then recursive traversal.

## Completion log

- Started:
- Finished:
- Most useful concept:
- Hardest bug:
- What I can now do without help:
- Next project:
