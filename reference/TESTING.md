# Testing Small C Projects

## Minimum test categories

For every project, test:
- Normal input.
- Smallest allowed input.
- Largest supported input.
- Empty input where possible.
- Invalid input.
- Repeated operations.
- Failure to open a file or allocate memory, where practical.
- Cleanup after errors.

## Example: number guessing game

| Test | Expected result |
|---|---|
| Guess equals target | Win message |
| Guess below target | Hint says higher |
| Guess above target | Hint says lower |
| Non-number input | Clear error or safe retry |
| Quit command | Clean exit |
| Target at minimum | Boundary case works |

## Manual test log

```text
Test:
Input/actions:
Expected:
Actual:
Pass/fail:
Follow-up:
```

## Regression testing

When fixing a bug, add a test or repeatable manual case so it does not return after later changes.
