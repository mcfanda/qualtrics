# Qualtrics Hacks
## Some qualtrics small projects

These are a few tests implemented in qualtrics. You just need to import the qsf file in your library and then include the survey in your project.
The surveys are simple exemplifications of what can be done in qualtrics, they are not meant to reflect the exact behavior of the original tests
or the scores one obtains with the code. For that, it is your responsability to test that the code is valid and results reliable.

I hope this code can give you a good start in implementing your own project.

## Digit Span

The digit span test shows a series of sequences of digits of increasing length. The participant should look at the digits sequence and type it in
when the last digit of the sequence disappear. 

In this implementation, each digit is shown for T milliseconf (T=1000 by default but can be changed). 
The first sequence shows K (K=3 by default but can be changed) digits. If the participants gets it right, the next sequence is of K+1 digits. 
If the participants gets it wrong, another sequence of length K is shown. The task ends and so the memory span is defined when the participant 
makes three consecutive errors for a given sequence length or when the span is 9 (this also can be changed easily). 

The same task is duplicated asking the participant to type the digit sequence in reverse order.

In the data produced one finds the time needed to respond to each sequence (usually not important) and two variable, named `span` and `spanr` that
contains the resulting memory span of the participant.

The test is implemented with a minimum of javascript code. It does not require any JS library and does not depend on the format of the survey it is included.

### Disclaimer of Liability:

The code and any accompanying documentation provided in this repository are offered "as is" without warranty or liability of any kind. The author(s) and contributors to this repository disclaim any liability for damages, including but not limited to direct, indirect, incidental, special, exemplary, or consequential damages, arising from the use or misuse of the code or any information contained herein.

Use of the code is entirely at your own risk. The author(s) and contributors disclaim any responsibility for any harm or loss of data that may occur from using or modifying the code. It is your responsibility to review and test the code thoroughly before using it in any production environment.

The code shared in this repository is provided under the CC BY-NC license. By using, distributing, or modifying the code, you agree to abide by the terms and conditions set forth in the license.

