# Mini Shell

## Purpose

Build a restricted shell to understand process creation and execution.

**Difficulty:** Advanced  
**Main concepts:** fork, execvp, waitpid, signals, pipes as optional extension

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

1. Read a command line safely.
2. Split a simple command into argv tokens.
3. Run a program using fork and execvp.
4. Wait for the child and report its exit status.
5. Handle command-not-found and EOF.
6. Optional: implement one pipe, then redirection.

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

- [ ] External commands run and the shell returns to the prompt.
- [ ] Child processes are reaped.
- [ ] EOF exits cleanly.
- [ ] Failed exec is reported in the child process.
- [ ] Limitations are documented.

Also:
- [ ] I can build and run it from the documented commands.
- [ ] I can explain the important functions without reading a tutorial aloud.
- [ ] I added one feature or variation of my own.
- [ ] I recorded one bug and how I diagnosed it in `NOTES.md`.

## Common stuck points

- **Do not call exec in the parent; fork first.:** Do not call exec in the parent; fork first.
- **After failed exec, the child should report the error and exit.:** After failed exec, the child should report the error and exit.
- **Naive whitespace splitting does not support shell quotes or expansions; state this limitation rather than pretending it is a full shell.:** Naive whitespace splitting does not support shell quotes or expansions; state this limitation rather than pretending it is a full shell.
- **Avoid signal-handling complexity until the basic loop works.:** Avoid signal-handling complexity until the basic loop works.

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

Use the operating-system manual pages for fork, execvp, waitpid, and pipe. Test only commands you understand.

## Completion log

- Started:
- Finished:
- Most useful concept:
- Hardest bug:
- What I can now do without help:
- Next project:
