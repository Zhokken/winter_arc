# Password Strength Checker

## Purpose

Practice string analysis and rule-based feedback.

**Difficulty:** Beginner–intermediate  
**Main concepts:** string length, character classes, functions, honest security limitations

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

1. Read a password without echoing it if you know how to do so safely; otherwise use non-sensitive test inputs.
2. Check length and character variety.
3. Explain which rules passed and failed.
4. Avoid storing or printing the submitted password.
5. Write a clear note that rule-based scoring is not a proof of security.

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

- [ ] Empty input is handled.
- [ ] Input length is bounded safely.
- [ ] Feedback explains its reasoning.
- [ ] The program never claims to guarantee that a password is uncrackable.

Also:
- [ ] I can build and run it from the documented commands.
- [ ] I can explain the important functions without reading a tutorial aloud.
- [ ] I added one feature or variation of my own.
- [ ] I recorded one bug and how I diagnosed it in `NOTES.md`.

## Common stuck points

- **strlen counts bytes, not Unicode characters.:** strlen counts bytes, not Unicode characters.
- **Do not print the secret back in debug output.:** Do not print the secret back in debug output.
- **Character-class rules are only rough heuristics; length and known compromised passwords matter too.:** Character-class rules are only rough heuristics; length and known compromised passwords matter too.

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

Use made-up test strings only. Do not submit real passwords to your own experimental tools.

## Completion log

- Started:
- Finished:
- Most useful concept:
- Hardest bug:
- What I can now do without help:
- Next project:
