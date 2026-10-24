# Start Here: Your First Week with C

## Goal

Become comfortable editing, compiling, running, and changing a tiny C program. Do not try to memorize the language.

## Before you start

On Linux, check:

```bash
gcc --version
make --version
gdb --version
```

If GCC is missing on Arch Linux, install the base development tools:

```bash
sudo pacman -S --needed base-devel gdb
```

Use your normal user account for compiling and running projects. Do not run your own programs as root unless there is a specific, understood reason.

## First program

Create `main.c`:

```c
#include <stdio.h>

int main(void)
{
    printf("Hello, world!\\n");
    return 0;
}
```

Compile and run:

```bash
gcc -std=c17 -Wall -Wextra -Wpedantic -g main.c -o hello
./hello
```

## Understand each part

- `#include <stdio.h>` makes declarations for standard input/output functions available.
- `int main(void)` defines the program's entry point.
- `{ ... }` groups statements into a function body.
- `printf` prints formatted text.
- `\\n` moves output to a new line.
- `return 0;` indicates successful completion to the operating system.
- `;` ends most C statements.

## Tiny experiments

Do these one at a time:
1. Change the message.
2. Print two separate lines.
3. Store an integer in a variable and print it with `%d`.
4. Create a second variable and print their sum.
5. Intentionally remove a semicolon, compile, and read the error. Then fix it.
6. Compile with `-Wall -Wextra -Wpedantic` and resolve every warning you introduced.

## How to get unstuck

Use this order:
1. Read the **first compiler error**, not only the final line.
2. Check the line mentioned and the line immediately above it.
3. Check spelling, semicolons, braces, parentheses, and format specifiers.
4. Recompile after making one change.
5. If it still fails, save the exact command, full error, and smallest relevant code snippet in your notes.
6. Ask for an explanation of the error and one hint before requesting a rewritten solution.

## Learning rule

Do not move on because the code ran once. Move on when you can change it, predict the result, and explain the main lines.
