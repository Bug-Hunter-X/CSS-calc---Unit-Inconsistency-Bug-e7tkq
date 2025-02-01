# CSS calc() Unit Inconsistency Bug

This repository demonstrates a common error when using the CSS `calc()` function: inconsistent units within the calculation.  The bug arises when combining percentage units with other units (like pixels or ems) without ensuring proper unit compatibility. This can lead to unexpected layout behavior in different browsers.

## How to Reproduce

1.  Open `bug.css` and examine the problematic `width` calculation in `.container`.
2.  Open `bugSolution.css` to see how to fix the problem.

## Bug Solution

The solution lies in ensuring all units within the `calc()` expression are consistent or easily convertible. The provided fix shows how to handle the issue by converting all units to a compatible base unit (in this case, pixels) before using them in the calculation. 