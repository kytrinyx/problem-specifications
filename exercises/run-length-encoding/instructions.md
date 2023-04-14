# Instructions

You need to create a program that can encode and decode the knitting patterns.

Since knitting patterns often have long sequences of identical colors, you've decided to use Run-length encoding (RLE) to compress the knitting patterns.
This is a simple form of data compression, where runs (consecutive data elements) are replaced by just one data value and count.

For example, in this excerpt from a black and white knitting pattern, we can represent the original 53 characters with only 13.

```text
"WWWWWWWWWWWWBWWWWWWWWWWWWBBBWWWWWWWWWWWWWWWWWWWWWWWWB"  ->  "12WB12W3B24WB"
```

RLE allows the original data to be perfectly reconstructed from the compressed data, which makes it a lossless data compression.

```text
"AABCCCDEEEE"  ->  "2AB3CD4E"  ->  "AABCCCDEEEE"
```

The knitting patterns use the letters A through Z to encode colors.
They use upper and lower-case letters to represent different types of stitches (e.g. a pattern might use upper case for 'knit' and lower-case for 'purl').
