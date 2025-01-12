# Uncommon CSS Flexbox Issue: space-between with Overflowing Items

This repository demonstrates an unusual behavior in CSS flexbox when using `justify-content: space-between` with items whose total width exceeds the container's width.  The expected behavior of evenly distributing items is not always met in such cases.  The `bug.css` file contains the problematic code, while `bugSolution.css` offers a solution.

## Problem
The problem arises from the interaction between `justify-content: space-between` and the total width of flex items exceeding the container's width.  In some browsers, this leads to unexpected item positioning and potentially overlapping elements.

## Solution
The solution involves using `flex-shrink` to allow items to shrink and fit within the container when the total width exceeds the container's available space.  This ensures a more predictable layout even when items overflow.