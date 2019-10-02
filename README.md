# Python Hackathon Entry Task <br>

Hackaton intro task: **Birth number generator & verifier** 

Program **birthnumber.py** will run in 2 modes - it will either generate a new birth number (no argument) or verify the number provided from command line (1 argument).

The conditions for generating and verifying the birth number are as follows:
  * number must contain 10 digits (for people born after 1954)
  * or must contain 9 digits (for people born before 1953)
  * number has 2 parts - date of birth and check sum (CCCC) in the form YYMMDD / CCCC
  * the integer must be divisible by 11
  * women have an added value of 50 in the month of birth

### Example: 
**861107/2239** is a valid birth number for a man born on 7.11.1986. <br> **025226/1306** is a valid birth number for a woman born on 26.02.2002.
To run a program and verify birth number, use the following command:

     $ birthnumber.py YYMMDD/CCCC
     
where `YYMMDD/CCCC` is specific birth number we want to verify.

The expected output in case of incorrect birth number is a message with errors that occurred during validation. <br>Example:

     Provided birth number is INVALID.
     <reason>
     <another-reason>

In case of generating new birth number, it will be an interactive process:
     
     $ birthnumber.py

output:

    Day of the birth [YYYY-MM-DD]: <user input>
    Sex [M/F]: <user input>
    Generated birth number: YYMMDD/CCCC

Use **Python 3** for implementation. It is not necessary to send us your solution, it is for your judgment whether you could handle similar and more challenging types of hackathon tasks. <br> For further information, please contact us at tech@engeto.com.
