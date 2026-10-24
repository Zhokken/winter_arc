# Expression Evaluator

## Purpose

Parse and evaluate arithmetic such as `2 + 3 * 4`.

**Difficulty:** Intermediate–advanced  
**Main concepts:** tokenizer, operator precedence, recursive descent, errors

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

1. Tokenize numbers and operators.
2. Support parentheses.
3. Implement multiplication/division precedence over addition/subtraction.
4. Reject malformed expressions.
5. Detect division by zero.
6. Add unary minus as a later feature.

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

- [ ] `2 + 3 * 4` follows precedence.
- [ ] Parentheses change grouping.
- [ ] Trailing garbage is rejected.
- [ ] Division by zero and invalid syntax are handled.

Also:
- [ ] I can build and run it from the documented commands.
- [ ] I can explain the important functions without reading a tutorial aloud.
- [ ] I added one feature or variation of my own.
- [ ] I recorded one bug and how I diagnosed it in `NOTES.md`.

## Common stuck points

- **A left-to-right evaluator ignores precedence; use grammar levels or an operator stack.:** A left-to-right evaluator ignores precedence; use grammar levels or an operator stack.
- **Recursive descent must consume input or return an error to avoid infinite recursion.:** Recursive descent must consume input or return an error to avoid infinite recursion.
- **Integer division differs from floating-point division; choose and document behavior.:** Integer division differs from floating-point division; choose and document behavior.

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

Write a grammar in plain text before implementing the parser.

## Completion log

- Started:
- Finished:
- Most useful concept:
- Hardest bug:
- What I can now do without help:
- Next project:
