Monte-Carlo-Money-Jar
=====================

A monte carlo program to simulate the growth of coins in a cookie jar over a 1 year period. The following are assumed:

1. you make X purchases each day with petty cash, starting out with only bills in your pocket (i.e., no change)
    
2. Each purchase has a random chance of costing some dollar amount plus YY cents (where YY goes from 0-99). You always get change in the smallest number of coins possible. For instance, if you have a purchase of $2.34, then you assume you acquire 66 cents in change (2 quarters, 1 dime, 1 nickel, 1 penny). 
        
3. If you have enough change to cover the YY cents of the current transaction, you use it. Otherwise, you accumulate more change. For example, if you have $1.02 in loose change, and you have a purchase of $10.34, then you use 34 cents (or as close to it as possible) in coins leaving you with 68 cents.
        
4. At the end of each day you dump all your coins collected for the day in a Money Jar.

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
