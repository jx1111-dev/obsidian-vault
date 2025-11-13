==WHEN THE ORDER DOESN'T MATTER, IT IS A **COMBINATION**.
WHEN THE ORDER DOES MATTER, IT IS A **PERMUTATION**.

A combination can be any set of items where order doesn't really matter. Like S = {apples, bananas, oranges.}. It doesn't matter how you order the fruits.

A permutation is a set of items where they have to be in a specific order to be used for their purpose, like a combination lock (I know, conflicting). Think S = {4,7,2}. The set has to be ordered that way, because that is the code to the combination lock. 

There are two types of permutations:

Repetition is Allowed: allows multiple of the same item in the same set. Example: a combination lock with the code being '333' or '448'.

These are the easiest to calculate. Take the set S = {3,3,3,3,3,3,3,3,3}.
To calculate the maximum combinations, just multiply each number in the list, or to make it easier, bunch all repeated items in the list together:

$$\begin{aligned}
&\\3*3*3*3*3*3*3*3*3  =3^9 = 19683 \ combinations
\end{aligned}$$
n is the item.
r is the amount of times it shows up.
The formula being n^r

No Repetition: a set cannot have a repeat item. Think about it like the first 3 people winning a race. You can't be first and second.

==FACTORIALS==


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