# Learn C by Building Real Projects

A project-first C curriculum for a beginner who wants to build their own software, games, and eventually lower-level systems.

## How to use this repository

1. Start with `00_START_HERE.md`.
2. Work through projects in the order in `ROADMAP.md`. Do not jump straight to the advanced projects just because they look exciting.
3. Read each project's `README.md` before coding. Treat it as a specification, not a solution.
4. Keep a `NOTES.md` in each project. Record bugs, fixes, concepts learned, and questions.
5. Build a small version first. Add optional features only after the core version works.
6. Use `REFERENCE.md` when stuck before searching for a complete solution.
7. Ask AI for explanations, debugging help, or hints—not a complete project to paste.

## Suggested repo layout

```text
c-learning/
├── README.md
├── ROADMAP.md
├── 00_START_HERE.md
├── reference/
│   ├── C_CHEATSHEET.md
│   ├── DEBUGGING.md
│   ├── MEMORY.md
│   └── TESTING.md
└── projects/
    ├── 01-hello-and-build/
    ├── 02-purchase-calculator/
    └── ...
```

Each project guide in this pack is standalone. You can place its Markdown file in a folder with the same project name.

## Definition of done

A project is done when:
- It compiles with useful warnings enabled.
- The normal use case works.
- You have tested invalid, empty, and boundary inputs where relevant.
- You can explain the important functions and data structures.
- You can make one small change without following a tutorial line by line.
- The README explains how to build and run it.

## Standard compile command

For a single-file program:

```bash
gcc -std=c17 -Wall -Wextra -Wpedantic -g main.c -o app
./app
```

For multi-file programs, compile all required `.c` files or use the project's Makefile. `-g` includes debug information; `-Wall -Wextra -Wpedantic` enable useful diagnostics. Warnings are information—read them rather than hiding them.
