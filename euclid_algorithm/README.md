# Euclid Algorithm #

The problem at hand is: given two numbers, m and n, find their *greatest common divisor* which is the largest positive number that evenly divides both m and n.

## How to solve ##

The algorithm is quite simple:
1. Divide m by n and let r be the remainder.
2. If r is zero then we have finished: n is the result.
3. Else let m be n and n be r. Repeat from step 1 until r is zero.

## Implementation in Algol60 ##

I implemented the algorithm with a procedure called `Euclid`, which is, basically, a function with two variables (namely, m and n).
Also i introduced a condition: if m is lesser than n, then swap the arguments (this is useful in order to achieve efficiency in code).  
I subsequently introduced two labels inside the procedure (`LOOP` and `EXIT`): the first (`LOOP`) is used to iterate until the result has been reached, while `EXIT` is used as exit from the precedent loop.
The procedure returns the greatest common divisor, which is then displayed as output in console.



