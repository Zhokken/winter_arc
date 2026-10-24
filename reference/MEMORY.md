# Pointers and Memory Reference

## Lifetime and ownership

Every pointer should have a clear meaning: which object does it point to, how long does that object live, and who is responsible for releasing it if it was dynamically allocated?

## Common mistakes

- Using a pointer before assigning a valid address.
- Dereferencing `NULL`.
- Reading or writing past an array's bounds.
- Returning a pointer to a local automatic variable.
- Using a pointer after `free`.
- Freeing the same allocation twice.
- Losing the only pointer to allocated memory.
- Forgetting space for the string's terminating `\\0`.
- Assuming `realloc` succeeded and overwrote the original pointer.

## Safer realloc pattern

```c
int *temporary = realloc(items, new_count * sizeof *items);
if (temporary == NULL) {
    /* items remains valid; handle the failure. */
} else {
    items = temporary;
}
```

For a general-purpose implementation, also validate `new_count * sizeof *items` for `size_t` overflow before calling allocation functions.

## Ownership contract example

A function that creates a buffer should document whether the caller owns the returned allocation and must call `free`. A function that merely borrows a pointer should not unexpectedly free it.

## Questions to ask when debugging

1. Is this pointer initialized?
2. Is the object still alive?
3. Is the index in range?
4. Is the buffer large enough?
5. Who frees this allocation?
6. Can the allocation fail?
7. Is the size calculation safe?
