# Qualtrics
## Some qualtrics small projects

These are a few tests implemented in qualitrics. You just need to import the qsf file in your library and then include the survey in your project.
The surveys are simple exemplification of what can be done in qualtrics, they are not meant to reflect the exact behavior of the original tests
or the scores one obtain with the code. For that, it is your responsability to test that the code is valid and results reliable.

I hope this code can give you a good start in implementing your own project.

## Digit Span

The digit span test shows a series of sequences of digits of increasing length. The participant should look at the digits sequence and type it in
when the last digit of the sequence disappear. 

In this implementation, each digit is shown for T milliseconf (T=1000 by default but can be changed). 
The first sequence shows K (K=3 by default but can be changed) digits. If the participants gets it right, the next sequence is of K+1 digits. 
If the participants gets it wrong, another sequence of length K is shown. The task ends and so the memory span is defined when the participant 
makes three consecutive errors for a given sequence length or when the span is 9 (this also can be changed easely). 

The same task is duplicated asking the participant to type the digit sequence in reverse order.

In the data produced one finds the time needed to respond to each sequence (usually not important) and two variable, named `span` and `spanr` that
contains the resulting memory span of the participant.
