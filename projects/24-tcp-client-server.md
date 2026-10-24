# TCP Client and Server

## Purpose

Send a simple message over a local TCP connection.

**Difficulty:** Advanced  
**Main concepts:** socket, bind, listen, accept, connect, send/recv, byte streams

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

1. Write a server that listens on localhost.
2. Accept one client.
3. Exchange a short greeting.
4. Define how messages end or how long they are.
5. Handle partial reads/writes and disconnects.
6. Add a client and test locally.

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

- [ ] Client and server agree on message framing.
- [ ] Connection errors are reported.
- [ ] Buffers are bounded and terminated safely when treated as strings.
- [ ] Server handles client disconnect.

Also:
- [ ] I can build and run it from the documented commands.
- [ ] I can explain the important functions without reading a tutorial aloud.
- [ ] I added one feature or variation of my own.
- [ ] I recorded one bug and how I diagnosed it in `NOTES.md`.

## Common stuck points

- **TCP is a byte stream; one recv is not guaranteed to equal one send.:** TCP is a byte stream; one recv is not guaranteed to equal one send.
- **Check return values and loop for partial writes/reads.:** Check return values and loop for partial writes/reads.
- **Start on 127.0.0.1, not a public interface, while learning.:** Start on 127.0.0.1, not a public interface, while learning.
- **Do not run an unauthenticated experimental server on a public network.:** Do not run an unauthenticated experimental server on a public network.

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

Read Beej's Guide to Network Programming and keep the first protocol local and tiny.

## Completion log

- Started:
- Finished:
- Most useful concept:
- Hardest bug:
- What I can now do without help:
- Next project:
