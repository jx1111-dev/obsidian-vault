
For plotting stuff related to this in matplotlib, go here: [[LIMITS IN MATPLOTLIB]]

==THIS SHIT MAKES NO SENSE, IMMA DO MY OWN THING==
Limits are used to sort of approximate what an impossible calculation would equal.

Let's say you have this calculation: 
$$
\begin{align}
&\frac{(x^2-1)}{(x-1)}
\end{align}
$$
If you work it out for x = 1:
$$
\begin{align}
&\frac{(1^2-1)}{(1-1)} = \frac{(1-1)}{(1-1)} = \frac{0}{0}
\end{align}
$$
And you can't go any further than this. What ever could we POSSIBLY do??????????????????
This is where limits come in. You can't divide 0 by 0, but you CAN divide 0.25 by 0.5.
Here's what I mean:

| x       | $$\frac{(x^2-1)}{(x-1)}$$ |
| ------- | ------------------------- |
| 0.5     | 1.50000                   |
| 0.9     | 1.90000                   |
| 0.99    | 1.99000                   |
| 0.999   | 1.99900                   |
| 0.9999  | 1.99990                   |
| 0.99999 | 1.99999                   |
| ...     | ...                       |
As you can see, making x a value very close to 1 instead of 1 gives us an approximate value of what the result of 0/0 is, namely: 2. 

So when x=1, we don't know the answer. It is __indeterminate__.

But we can see it's __going__ to be 2.

We can't just say it's 2 however. Instead, the math way of saying this is: $$The \space limit \space of \space \frac{(x^2-1)}{(x-1)}\space as \space x \space approaches \space 1 \space is \space 2$$

Written in symbols as:
$$\lim_{x \to 1} \frac{x^2-1}{x-1} = 2
$$

So you are basically ignoring what happens when you get to x=1, but as you get closer the answer gets closer to 2. 

This is what a graph of the limit above looks like:
![[Pasted image 20251016101658.png]]
x=1 is a hole in the line. 

It's also good practice to check from the "other side", as in assigning 0 values above 1.
Example:

| x       | $$\frac{(x^2-1)}{(x-1)}$$ |
| ------- | ------------------------- |
| 1.5     | 2.50000                   |
| 1.1     | 2.10000                   |
| 1.01    | 2.01000                   |
| 1.001   | 2.00100                   |
| 1.0001  | 2.00010                   |
| 1.00001 | 2.00001                   |
| ...     | ...                       |

So now you're double sure 0/0 is 2.

### ==APPROACHING INFINITY==

Infinity is an idea, not a number. So if you pull some bullshit like $$\frac{1}{\infty}$$

That's like dividing 1 by a word. You're doing $$\frac{1}{tall}$$
###### Idiot. 
In fact, 1 divided by infinity is **undefined**. 

But just like earlier, we can approach it. Replace infinity with x, and keep making it a larger and larger value. 

| x     | $$\frac{1}{x}$$ |
| ----- | --------------- |
| 1     | 1.00000         |
| 2     | 0.50000         |
| 4     | 0.25000         |
| 10    | 0.10000         |
| 100   | 0.01000         |
| 1000  | 0.00100         |
| 10000 | 0.00010         |
As we can see, as x gets larger, $$\frac{1}{x}$$
gets closer and closer to 0.

So the limit of 1/x as x approaches infinity is 0. Trippy stuff. I know.
$$\lim_{x \to \infty} \frac{1}{x} = 0$$
==When you think limit, think approaching.==


### ==EVALUATING LIMITS==
Just saying that the result of 1 divided by infinity looks like it equals 0 isn't enough. You still need to evaluate it. What does that mean though?

In this case, it means to find the value of (e-**"value"**-ating).

If you're just dealing with a normal number and not some imaginary black magic, it's actually pretty easy. You just ***substitute*** x for the limit. Just put the value in.
$$\lim_{x \to 10} \frac{x}{2} \to \frac{10}{2} = 5 👍$$
But...
$$\lim_{x \to 1} \frac{x}{1} \to \frac{(1-1)}{(1-1)} = \frac{0}{0} 👎$$
To evaluate these types of limits, you use 
#### ==FACTORS==
I'm not gonna go into what factoring is because I assume the person reading this knows some degree of GCSE math. If you don't just let me know I guess. I'll try teaching you.

This is how it would go using factoring:
$$\lim_{x \to 1} \frac{(x^2-1)}{(x-1)} = \lim_{x \to 1} \frac{(x-1)(x+1)}{(x-1)} = \lim_{x \to 1} (x+1)$$
Then, just substitute x=1 to get the limit:
$$\lim_{x \to 1} (x+1) = 1+1 = 2$$

For some fractions, you may need to use 
#### ==CONJUGATES==
If you don't remember, a conjugate is when you change the sign in the middle of 2 terms to their opposite. Like this:
$$3x+1 \to 3x-1$$
Here's an example of how to use conjugates in limits:
$$\lim_{x \to 4} \frac{2-\sqrt{x}}{4-x}$$
This gives you 0/0. That's no good.
So instead, let's **rearrange** it:

First, Multiply the top and bottom by the conjugate of the top (2+sqrt(x))

$$\frac{2-\sqrt{x}}{4-x} * \frac{2+\sqrt{x}}{2+\sqrt{x}}$$
Simplify it using (a+b)(a-b) = a^2 - b^2 and simplify it further:

$$\frac{2^2 - (\sqrt{x})^2}{(4-x)(2+\sqrt{x})} = \frac{4-x}{(4-x)(2+\sqrt{x})}$$
And then cancel (4-x) from the top:
$$\frac{1}{2+\sqrt{x}}$$
Which gives us:
$$\lim_{x \to 4}\frac{2-\sqrt{x}}{4-x} = \lim_{x \to 4} \frac{1}{2+\sqrt{x}} = \frac{1}{2+\sqrt{4}} = \frac{1}{4}$$
Done!

Want to get more nerdy?

#### ==INFINITE LIMITS AND RATIONAL FUNCTIONS

Polynomials are just a bunch of terms together. Like $$4xy^2 + 2x + 5$$
A rational function is a ratio of 2 polynomials:
$$f(x) = \frac{P(x)}{Q(x)}$$
Example:
$$
\begin{align}
&P(x) = x^3 + 2x -1
&Q(x) = 6x^2
\end{align}
$$
$$
\frac{x^3+2x-1}{6x^2}
$$
TO FINISH. ADD THE L'HOPITAL RULE AND THE FORMAL METHOD

#LessonDefinedUnderstandingTBD😂😂😎😎