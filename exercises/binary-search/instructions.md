# Instructions

Your task is to implement a binary search algorithm.

A binary search algorithm works by dividing the sorted list in half and comparing the middle element with the item we're looking for.
If the middle element is our item, then we're done.
If not, then there are two options.
Either the middle element is greater than our item, or it is less than our item.

If the middle element is greater than our item, we can eliminate that number and all the numbers after it.
If the middle element is less than our item, we can eliminate that number and all the numbers before it.
Then we can repeat the process on the other half of the list.

By dividing the list in half each time, we can quickly narrow down the possible locations of our item until we find it, or until we've eliminated all possible locations.

Here's an example:

Let's say we're looking for the number 23 in the following sorted list: `[4, 8, 12, 16, 23, 28, 32]`.

We start by comparing 23 with the middle element, 16.
Since 23 is greater than 16, we can eliminate the left half of the list, leaving us with `[23, 28, 32]`.
We then compare 23 with the new middle element, 28.
Since 23 is less than 28, we can eliminate the right half of the list: `[23]`.
We've found our item.
