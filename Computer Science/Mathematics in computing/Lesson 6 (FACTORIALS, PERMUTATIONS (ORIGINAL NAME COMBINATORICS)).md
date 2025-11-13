==WHEN THE ORDER DOESN'T MATTER, IT IS A **COMBINATION**.
WHEN THE ORDER DOES MATTER, IT IS A **PERMUTATION**.

A combination can be any set of items where order doesn't really matter. Like S = {apples, bananas, oranges.}. It doesn't matter how you order the fruits.

A permutation is a set of items where they have to be in a specific order to be used for their purpose, like a combination lock (I know, conflicting). Think S = {4,7,2}. The set has to be ordered that way, because that is the code to the combination lock. 

There are two types of permutations:

==Repetition is Allowed: allows multiple of the same item in the same set. Example: a combination lock with the code being '333' or '448'.

These are the easiest to calculate. Take the combination lock S = {0, 1, 2, 3, 4, 5, 6, 7, 8, 9}.

When a thing has **r** things, we have **n** choices each time.

For example, choosing **3** items out of the **10** item list:

$$n*n*n\ (n\ multiplied\ r\ times) = 10*10*10\ (10\ multiplied\ 3\ times)$$

For example, in the lock above, there are 10 numbers to choose from. If we choose 6 of them:

$$\begin{aligned}
&\\10*10*10*10*10*10 = 10^6 = 1000000 \ permutations
\end{aligned}$$

The formula being n^r
Where **n** is the number of things to choose from, and we choose **r** of them.


==No Repetition: a set cannot have a repeat item. Think about it like the first 3 people winning a race. You can't be first and second.

To calculate a no repetition permutation, you need to reduce the number of available choices every time you choose an item. 

For example, what order can 16 pool balls go in?
If we put ball number 14 first, we cannot choose it again. So for the next choice, we have 15 choices left. Overall, it comes out to:

$$16*15*14*13*12*11*10*9*8*7*6*5*4*3*2*1 = 20,922,789,888,000\ permutations$$
You might see where this is going. But if you don't need to choose a space for all 16 balls, and want to order 3 of them, for example, all you have to do is:
$$16*15*14 = 3360\ permutations$$
In other words, there are 3,360 balls can be arranged out of 16 balls.

How do we write this mathematically though? I'm getting carpel tunnel from writing all this stuff.

The answer is:
==THE FACTORIAL FUNCTION==

If you have a set, say like S  = {1,5,4,3}

How many combinations does it have?
You find this out with the factorial function, the rule being n! = n x (n-1)!

Say you need to calculate 3!
All you need to do is:

3 x 2 x 1 = 6

or:

3! = 3 x (3-1)!

3! = 3 x 2!

3! = 3 x 2 x (2-1)!

3! = 3 x 2 x 1

3! = 6

Interestingly, 0! is actually equal to one. Let me explain by working my way back from 4!.

4! = 24  (/4)
3! = 6 (/3)
2! = 2 (/3)
1! = 1 (/2)
0! = 1 (/1)

==fun cool awesome hack for dividing factorials working 2026 no virus

If you divide 2 factorials, e.g.
$$\frac{100!}{98!}$$
In reality, this looks like:
$$\frac{100*99*98*97*96*95...}{98*97*96*95...}$$
If you look closely, you would notice that 100! contains all terms in 98!, so you can simplify the fraction:
$$\frac{100*99*98*97....}{98*97...} = 100*98 = 9800$$
