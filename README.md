# Happy Number

## Problem Description

A **happy number** is a number defined by the following process: Starting with any positive integer, replace the number by the sum of the squares of its digits, and repeat the process until the number equals 1 (where it will stay), or it loops endlessly in a cycle which does not include 1. Those numbers for which this process ends in 1 are happy numbers.

Write a function to determine if a given number `n` is happy.

### Input

- An integer `n` (1 ≤ n ≤ 2<sup>31</sup> - 1).

### Output

- Returns `True` if `n` is a happy number, `False` otherwise.

## Example

```python
assert is_happy(19) == True
assert is_happy(2) == False
```

## Explanation

- **Example 1:** 19 is a happy number.

    1² + 9² = 82

    8² + 2² = 68

    6² + 8² = 100

    1² + 0² + 0² = 1 (Happy number)

- **Example 2:** 2 is not a happy number.

    2² = 4

    4² = 16

    1² + 6² = 37

    3² + 7² = 58

    5² + 8² = 89

    8² + 9² = 145

    1² + 4² + 5² = 42

    4² + 2² = 20

    2² + 0² = 4 (Cycle starts, not a happy number)

## Constraints

- The input integer `n` is a positive integer.
