# Instructions

Your task is to find the saddle points in a matrix representing distances between cities.

A saddle point is a point where the surface curves up in one direction and down in another direction.
The saddle point isn't the lowest point overall, nor is it the highest point overall.
It represents a point where there is no good solution.

In a matrix, a saddle point is an element that the largest in its row, while being the smallest in its column.

~~~~exercism/note
You may find other definitions of matrix saddle points online.
The tests for this exercise follow the above unambiguous definition.
~~~~

A matrix might not have any saddle points at all.
Or it might have one, or even several.

Here is a matrix that has exactly one saddle point.

    1  2  3  4
  |-----------
1 | 9  8  7  8
2 | 5  3  2  4  <--- saddle point at row 2, column 1, with value 5
3 | 6  6  7  1

- Row 2 has values 5, 3, and 1. The largest value is 5.
- Column 1 has values 9, 5, and 6. The smallest value is 5.

So the point at `[2, 1]` (row: 2, column: 1) is a saddle point with value 5.
