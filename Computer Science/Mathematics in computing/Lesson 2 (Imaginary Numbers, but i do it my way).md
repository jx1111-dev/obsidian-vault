You were like 10 mins late but so far he's been speaking about real and rational and irrational numbers (you know these)

It's impossible to get an irrational number from a rational number.

Mean is that weird backwards sort of Z character that keeps showing up. (Called sigma) Think of it like the range function in python. 
![[Pasted image 20251009092155.png]]

==COMPLEX NUMBERS

![[Pasted image 20251009092639.png]]
![[Pasted image 20251009093344.png]]
Complex numbers are a combination of real numbers and imaginary numbers.

Complex numbers can be represented on a graph.

Magnitude is represented by z with 2 lines on each side.
![[Pasted image 20251009093704.png]]
If you multiply them its like multiplying two brackets? I guess?

==COMPLEX NUMBER SUBUNITS==

Complex conjugates are briefly covered in [[Lesson 3 (Limits)]]

if letters have a line above them it means they are negative or something???

V line z
z = a-b * i

V normal z
z = a+b * i

==HOW TO ACTUALLY MAKE SENSE OF ANY OF THIS

Real numbers (in case you forget): 1, 12.38, -0.8625, 3/4, square root of 2, 1998 etc.

Imaginary numbers are numbers that, when squared, give a negative result. This is impossible because when we square a positive number, the result HAS to be positive. This is true even if the number is negative. (e.g. -2^2 = 4)

The "unit" imaginary number is the square root of -1, which is represented by i. When we square it, we get -1.

i^2 = -1

Imaginary numbers are just numbers that have i in them. Like: 3i, 1.04i, -2.8i, 3i/4, square root of 2 * i, 1998i

Complex numbers are just a combination of real and imaginary numbers. They are LITERALLY just real and imaginary numbers added/subtracted together. **All real and imaginary numbers are complex numbers.

a (real) + b(imaginary) * i
examples: 3+i, 39+3i, 0.8 -2.2i, >-2 + 

Either part of a complex number can be a zero, meaning that it can either be purely real, or purely imaginary. So you could have 1+4i, which is complex. You can also have 0+4i, which is purely imaginary, or 1+0i, which is purely real. (because 0 * i = 0)

Now, before I move on to visual explanations (Graphs. Yes, I know you haven't seen a graph in 2 years.) you need to rack your brain and remember **polar** and **cartesian** coordinates.

Cartesian coordinates are simple. It's (x,y). It's the simple type of coordinate. e.g. (12,5). You know this. You had like a whole other set of GCSEs about this.  
![[Pasted image 20251009105045.png]]

Polar coordinates mark a point by **how far away it is**, and **what angle it has** from **0**.
![[Pasted image 20251009105104.png]]

If  you want to convert from polar to cartesian, you do so like this:
Firstly, make a triangle with points on the center (0), the point, and the intersection of the point and the center. Make sure it's a right angle triangle.
![[Pasted image 20251009105154.png]]

If you are converting from **cartesian to polar**, use pythagoras theorem to calculate r (because you should have x and y)
![[Pasted image 20251009105348.png]]
$$
\begin{align}
&r^2 = 12^2 + 5^2\\
&r^2 = 144 + 25\\
&r^2 = 169\\
&r = 13
\end{align}
$$
Then, you need to use tan to find the angle 
$$
\begin{align}
&tan(θ) = 5 / 12\\
&θ = tan-1 ( 5 / 12 ) = 22.6° 
\end{align}
$$
And boom. You got a distance of 13, and an angle of  22.6 (goes on for a while but its shortened to 1 decimal.)

To convert from **polar to cartesian**, basically just do the opposite. You have the distance and the angle, and you apply either cos or sin depending on if you have x or y, respectively.
![[Pasted image 20251009112821.png]]
Solving for x:
$$
\begin{align}
&cos( 22.6° ) = x / 13\\
&x = 13 × cos( 22.6°)\\
&x = 13 × 0.923\\
&x = 12.002\\
&x = 12
\end{align}
$$
Solving for y:
$$
\begin{align}
&sin( 22.6° ) = y / 13\\
&y = 13 × cos( 22.6°)\\
&y = 13 × 0.391\\
&y = 4.996\\
&y = 5
\end{align}
$$
These give you almost exactly the coordinates (12,5). This is stupid and dumb, but good enough. 

**If x and y are negative, things get more complicated.**
The graph you had gains 3 more "Quadrants." These are numbered I-IV, counter-clockwise. (This is explained later)
![[Pasted image 20251009113342.png]]
Now, when converting from Polar to Cartesian, it all works out fine. 
$$
\begin{aligned}
&For\ example,\ what\ is\ (12,195\degree)\ in\ cartesian\ coordinates?
\\&r=12\ and\ \theta=195\degree\\
\\&Solving\ x:
\\&x = 12 \times cos(195\degree)
\\&x = 12 \times -0.9659...
\\&x = -11.59\ to\ 2\ decimal\ places\\
\\&Solving\ y:
\\&y = 12 \times sin(195\degree)
\\&y = 12 \times -0.2588...
\\&y = -3.11\ to\ 2\ decimal\ places

\end{aligned}
$$ 
But when you try Cartesian to Polar, your calculator can give the wrong value of tan^-1

However, it depends on what quadrant the point is in. Here is what you do:


| Quadrant | Value of tan^-1                  |
| -------- | -------------------------------- |
| I        | Use the calculator value         |
| II       | Add 180° to the calculator value |
| III      | Add 180° to the calculator value |
| IV       | Add 360° to the calculator value |
(Yes, both quadrant II and III are "Add 180")

Example:
![[Pasted image 20251030104350.png]]
P is in Quadrant II
$$\begin{aligned}
&r = \sqrt((-3)^2+10^2)
\\&r = \sqrt109 = 10.4\ to\ 2\ decimal\ place
\\&\theta = tan^{-1}(10/-3)
\\&\theta = tan^{-1}(-3.33...)
\\&The\ calculator\ value\ for\ tan^{-1}(-3.33...)\ is\ -73.3\degree\ (not\ good)
\\&\to The\ rule\ for\ Quadrant\ II\ is:\ Add\ 180\degree \ to\ the\ calculator\ value
\\&\to \theta = -73.3\degree + 180\degree = 106.7\degree
\end{aligned}$$
So the polar coordinates for the point (-3,10) are (10.4, 106.7°)

Now that we got conversions out of the way,

# ==THE COMPLEX PLANE==
![[Pasted image 20251030105949.png]]
When you imagine real numbers, you probably imagine them in a line that goes negative (to the left) and positive (to the right). Imaginary numbers basically go up (positive) and down (negative), creating a **complex plane.** 

We can now show complex numbers as points:
![[Pasted image 20251030110302.png]]
==Properties==
The letter z is usually the designation we use for a complex number.
$$
z = a + bi
$$
- **z** is a Complex Number
- **a** and **b** are Real Numbers
- **i** is the unit imaginary number = $$\sqrt{-1}$$
We refer to the real part and imaginary part using **Re** and **Im** like this:

Re(z) = a
Im(z) = b



TO FINISH
#LessonDefinedUnderstandingTBD😂😂😎😎 