# C Project Roadmap

Progress is based on understanding, not calendar time. You can spend longer on any stage.

## Stage 1 — First principles
1. `01-hello-and-build.md` — source, compiler, executable, output
2. `02-purchase-calculator.md` — variables, types, arithmetic, input
3. `03-number-guessing-game.md` — conditions, loops, validation
4. `04-text-adventure.md` — functions, state, branching
5. `05-grade-tracker.md` — arrays, loops, simple summaries
6. `06-quiz-game.md` — arrays, strings, functions, score tracking

## Stage 2 — Practical command-line software
7. `07-cat-clone.md` — files, command-line arguments, errors
8. `08-word-line-counter.md` — character streams and counting rules
9. `09-file-analyzer.md` — file metadata/content analysis and modular code
10. `10-password-strength-checker.md` — string analysis and careful claims
11. `11-notes-app.md` — persistent data, parsing, CRUD operations

## Stage 3 — Games and graphics
12. `12-pong-raylib.md` — window, input, update/draw loop
13. `13-breakout-raylib.md` — arrays, collision, game states
14. `14-top-down-survival.md` — entity updates, spawning, game balance
15. `15-retro-horror-prototype.md` — atmosphere, scenes, interactions, assets

## Stage 4 — Data structures and memory
16. `16-dynamic-array-library.md` — `malloc`, `realloc`, ownership
17. `17-linked-list.md` — nodes, pointers, insertion and deletion
18. `18-hash-table.md` — hashing, collisions, resizing
19. `19-memory-tracker.md` — allocation wrappers and leak accounting
20. `20-custom-data-parser.md` — parsing, validation, error reporting

## Stage 5 — Linux systems programming
21. `21-mini-shell.md` — processes, `fork`, `exec`, `wait`
22. `22-file-search-tool.md` — directories, traversal, filtering
23. `23-process-monitor.md` — process information and safe parsing
24. `24-tcp-client-server.md` — sockets, protocol design, error handling

## Stage 6 — Developer tools
25. `25-expression-evaluator.md` — tokenization and precedence
26. `26-mini-language-interpreter.md` — lexer, parser, AST, evaluation
27. `27-bytecode-vm.md` — instructions, stack, execution
28. `28-terminal-text-editor.md` — terminal input, text buffer, redraw

## Stage 7 — Advanced choices
29. `29-raycaster.md` — vectors, grid maps, ray intersections
30. `30-simple-software-renderer.md` — pixels, transforms, depth
31. `31-simple-memory-allocator.md` — alignment, blocks, fragmentation
32. `32-own-project-capstone.md` — independently scope and deliver a project

## Suggested sequence

Do projects 1–6 before the file tools. Start game projects as soon as you can write functions and loops; do not wait until the whole roadmap is complete. For the mini-shell, TCP server, interpreter, allocator, and renderer, expect to revisit earlier concepts.

## Advancement gates

- Before file tools: can write loops, functions, and basic string code.
- Before raylib: can compile C and use functions, structs, and arrays.
- Before dynamic data structures: understand addresses, pointers, and `sizeof`.
- Before processes/sockets: comfortable with command-line tools and error handling.
- Before interpreter/VM: comfortable with structs, enums, arrays, and parsing input.
- Before allocator/renderer: can debug carefully and test small components independently.
