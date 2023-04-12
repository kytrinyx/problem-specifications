# Instructions

Make sure that your time machine handles leap years correctly.

**A leap year is a year that has an extra day in it.**

Normally, a year has 365 days, but the Earth takes about 365.25 days to orbit the sun, so we get out of sync.
To make up for this, every four years we add an extra day (a leap day) on February 29th.

The problem is that Earth doesn't take exactly 365.25 days to orbit the sun.
Adding a leap day every four years helps, but we still get a bit out of sync.

To make up for that, we skip a leap day every century, which gets us **mostly** back into sync.
To get us all the way back into sync, every 400 years we don't skip the leap day after all.

So to sum up the rules:

- Add a leap day if the year is divisible by 4.
- If the year is divisible by 100, don't add the leap day.
- If the year is divisible by 400, add the leap day after all.

So 1997 was not a leap year, but 1996 was.
The years 1700, 1800, and 1900 were not leap years, even though they are divisible by 4.
However, the year 2000 was a leap year because it is divisible by 400.

~~~~exercism/note
Leap years are more interesting than most people realize.
For a delightful introduction, watch the four minute video [What is a Leap Year?][video] by CGP Grey.

[video]: https://www.youtube.com/watch?v=xX96xng7sAE
~~~~
