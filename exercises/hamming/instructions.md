# Instructions

The program will take two sequences of answers:
- The answer key (the sequence of correct answers).
- A sequence representing a single student's answers.

The result of the program is the number of mistakes the student has made.

So a score of 0 means that the student did everything right.
A score of 4 means that the student got four questions wrong.

The program can work internationally, using different scoring systems.
For example, in Thailand you might use ก.ข.ค.ง., whereas in Canada you might use A.B.C.D.

Due to a historical accident, the test data for your program uses A.C.G.T.

~~~~exercism/note
Comparing two sequences and counting the mistakes between them is called the Hamming Distance.

The Hamming Distance can only be used to compare two sequences that are of equal length.

In a later version of your program you might allow a student to skip an answer, encoding it with '-' or 'X'.
But for now, assume that the student must answer every question.
~~~~
