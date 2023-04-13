# Instructions

Your task is to convert a random number into sounds.

There are three possible sounds.
Each sound is represented by a prime number.

- **Pling**: 3
- **Plang**: 5
- **Plong**: 7

The sound should be played if the random number can be divided by the prime number, leaving no remainder.
If it can, we say that the prime number is a **factor** of the random number.

To convert the random number into sounds, use these rules:

- If the number has 3 as a factor, add 'Pling' to the result.
- If the number has 5 as a factor, add 'Plang' to the result.
- If the number has 7 as a factor, add 'Plong' to the result.
- If the number _does not_ have any of 3, 5, or 7 as a factor, the result should be the digits of the number.

For example:

- 28 has 7 as a factor, but not 3 or 5, so the result would be "Plong".
- 30 has both 3 and 5 as factors, but not 7, so the result would be "PlingPlang".
- 34 is not factored by 3, 5, or 7, so the result would be "34".

~~~~exercim/note
The simplest way to test if one number is a factor of another is to use the [modulo operation][modulo].

[modulo]: https://en.wikipedia.org/wiki/Modulo_operation
~~~~
