# Debugging Checklist

## When compilation fails

1. Re-run the exact compile command.
2. Read the first error and note the file and line.
3. Check the previous line for a missing semicolon or brace.
4. Confirm declarations and includes.
5. Check capitalization—C is case-sensitive.
6. Fix one issue, then compile again.

## When the program crashes or behaves strangely

1. Reproduce the problem with the smallest input.
2. State what you expected and what actually happened.
3. Add temporary diagnostic output to inspect values.
4. Use a debugger if needed:

```bash
gdb ./app
```

Useful GDB commands:
- `break main` — stop at the beginning of `main`
- `run` — start the program
- `next` — execute the next source line without stepping into a function
- `step` — step into a function
- `print variable_name` — inspect a variable
- `backtrace` — show the call stack after a crash
- `continue` — resume execution
- `quit` — exit GDB

## Sanitizers

For many small programs, compile with AddressSanitizer and UndefinedBehaviorSanitizer:

```bash
gcc -std=c17 -Wall -Wextra -Wpedantic -g \
    -fsanitize=address,undefined -fno-omit-frame-pointer \
    main.c -o app
./app
```

Sanitizers help detect certain memory and undefined-behavior bugs. They do not prove that a program is correct.

## The bug report template

```text
Goal:
Expected behavior:
Actual behavior:
Steps to reproduce:
Input used:
Exact compile command:
Full error/output:
Smallest relevant code:
What I already tried:
```

## If you are stuck for 20 minutes

- Reduce the feature to one function.
- Print or inspect the variables involved.
- Check assumptions about input and array bounds.
- Write down what each step should do.
- Search the documentation for the exact function or error.
- Ask for a hint that preserves the problem-solving work.
