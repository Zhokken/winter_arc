# C Quick Reference

## Compile

```bash
gcc -std=c17 -Wall -Wextra -Wpedantic -g main.c -o app
./app
```

## Common types

```c
int count = 3;
double distance = 12.5;
char letter = 'A';
char name[] = "Ada";
```

Use `%d` for `int`, `%f` for `double` in `printf` (the `printf` argument is promoted appropriately), `%c` for `char`, and `%s` for a null-terminated string. `printf("%f", value)` is valid for a `double`.

## Conditions and loops

```c
if (count > 0) {
    puts("positive");
} else {
    puts("zero or negative");
}

for (int i = 0; i < 5; i++) {
    printf("%d\\n", i);
}

while (count > 0) {
    count--;
}
```

## Functions

```c
int add(int a, int b)
{
    return a + b;
}
```

A function declaration/prototype lets the compiler know a function's type before its definition:

```c
int add(int a, int b);
```

## Arrays and strings

```c
int values[3] = { 2, 4, 6 };
char text[64] = "hello";
```

C arrays do not automatically know their length when passed to a function. Pass the length separately. A C string ends with `\\0`. Ensure the destination buffer is large enough before writing to it.

## Pointers

```c
int value = 10;
int *ptr = &value;
*ptr = 20;
```

- `&value` means address of `value`.
- `int *ptr` declares a pointer to an integer.
- `*ptr` accesses the object pointed to, when the pointer is valid.

Never dereference an uninitialized, null, dangling, or otherwise invalid pointer.

## Structs and enums

```c
typedef struct {
    int x;
    int y;
} Point;

typedef enum {
    STATE_MENU,
    STATE_PLAYING,
    STATE_GAME_OVER
} GameState;
```

## File I/O

```c
FILE *file = fopen("input.txt", "r");
if (file == NULL) {
    perror("fopen");
    return 1;
}
/* Read and check errors here. */
if (fclose(file) != 0) {
    perror("fclose");
}
```

## Dynamic memory

```c
int *items = malloc(count * sizeof *items);
if (items == NULL) {
    /* Handle allocation failure. */
}
/* Use items only if allocation succeeded. */
free(items);
items = NULL;
```

Include `<stdlib.h>` for allocation functions. Check multiplication overflow before calculating large allocation sizes. Never use memory after freeing it.

## Errors

- Compiler error: code cannot be compiled as written.
- Warning: compiler sees a suspicious pattern; investigate it.
- Runtime error: program fails while running.
- Logic bug: program runs but behaves incorrectly.
- Undefined behavior: C does not define what the program does; it may appear to work and still be wrong.
