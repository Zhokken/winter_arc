# Mini Language Interpreter

## Purpose

Build a tiny language with variables and print statements.

**Difficulty:** Advanced  
**Main concepts:** lexer, parser, AST, environment, evaluation, errors

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

1. Define a tiny grammar: numbers, arithmetic, variable assignment, print.
2. Write a lexer that creates tokens.
3. Parse expressions and statements.
4. Represent syntax with structs/enums or evaluate directly for a first tiny version.
5. Store variables in a simple environment.
6. Report line/column for errors.

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

- [ ] Example programs parse and execute predictably.
- [ ] Undefined variables produce clear errors.
- [ ] Malformed syntax does not crash the interpreter.
- [ ] Operator precedence is consistent.

Also:
- [ ] I can build and run it from the documented commands.
- [ ] I can explain the important functions without reading a tutorial aloud.
- [ ] I added one feature or variation of my own.
- [ ] I recorded one bug and how I diagnosed it in `NOTES.md`.

## Common stuck points

- **Do not mix tokenization, parsing, and evaluation into one giant function.:** Do not mix tokenization, parsing, and evaluation into one giant function.
- **AST node ownership must be explicit and recursively freed.:** AST node ownership must be explicit and recursively freed.
- **Keep the language small; functions and loops are later extensions.:** Keep the language small; functions and loops are later extensions.

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

Start with arithmetic only; reuse the expression evaluator from project 25.

## Completion log

- Started:
- Finished:
- Most useful concept:
- Hardest bug:
- What I can now do without help:
- Next project:
