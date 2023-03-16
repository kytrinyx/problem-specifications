# Instructions

Your task is to look for patterns in the long sequence of digits in the encrypted signal.

The technique you're going to use here is called the largest series product.

Let's define a few terms, first.

- **input** - the long sequence of digits that you need to analyze
- **series** - a sequence of adjacent digits that is contained within the input
- **span** - how many digits long the series is

To form a series, take digits that are next to each other in the original input.

Given the input `"1234"`, if you are working with a span of `3`, there will be two possible series:

- `"123"`
- `"234"`

The **product** is what you get when you multiply numbers together.
The product of `2` and `3` is `6` (`2 × 3 = 6`).

So the product of a series is the result of multiplying all the digits in a series together.

- The product of the series `"123"` is 6 (`1 × 2 × 3 = 6`).
- The product of the series `"234"` is 24 (`2 × 3 × 4 = 24`).

For a series of zero digits, you need to return the empty product (the result of multiplying no numbers), which is 1.

~~~~exercism/advanced
You do not need to understand why the empty product is 1 to solve this problem.

In case you're interested, here is an informal argument:

It doesn't matter which order you multiply things in.
`2 × 3` is the same as `3 × 2`.

If we split a list of numbers `A` into two new lists `B` and `C`, then we expect `product(A) == product(B) * product(C)`.

If we split a list containing only the number 3 into the empty list and a list containing the number 3 then the product of the empty list has to be 1 for `product([3]) == product([]) * product([3])` to be true.

The same kind of argument justifies why the sum of no numbers is 0.
~~~~

Let's take the input `"63915"` as an example.

There will be three series of span `3`:

- `"639"`
- `"391"`
- `"915"`

Then we need to calculate the product of each series:

- The product of the series `"639"` is 162 (`6 × 3 × 9 = 162`)
- The product of the series `"391"` is 27 (`3 × 9 × 1 = 27`)
- The product of the series `"915"` is 45 (`9 × 1 × 5 = 45`)

162 is bigger than both 27 and 45, so the largest series product of `"63915"` is 162.
