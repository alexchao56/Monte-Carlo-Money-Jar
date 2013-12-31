Monte-Carlo-Money-Jar
=====================

Program to see how fast loose change piles up over a one year period.

To run the program (Using Python 2.7):

from command line:

`>> python CookieJar.py`

Once within python, from the folder containing this file:

`>> from CookieJar.py import CookieJar, simulate`

`>> simulate()`

Answers the following questions

**a**: What is the average total amount of change accumulated each year (assume X=5)? What is the 1-sigma scatter about this quantity?

Ans: mean = $181.71
     std   = $5.99

**b**: What coin (quarter, dime, nickel, penny) are you most likely to accumulate over time? Second most likely? Does it depend on X?

Ans: Pennies always come first, quarters areusually second (and sometimes dimes). No it doesn't depend on X
    

**c**: Let's say you need 8 quarters per week to do laundry. How many quarters do you have at the end of the year? (if you do not have enough quarters at the end of each week, use only what you have).

Ans: 31
