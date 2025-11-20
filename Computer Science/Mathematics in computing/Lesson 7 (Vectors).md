Matrix and vector multiplication are behind machine/deep learning and computer graphics. What does the GPU do in these actions?

It calculates simple computations, like multiply and sum, where the cpu is not needed.

It does each step independently, which leads to trivial parallelisation.

General purpose GPUs: Computer graphics, Deep Learning, LLMs impossible otherwise.

GPU libraries: Torch, TensorFlow, Open CV...

Matrices are a 2D arrangement of data and variables. 
![[Pasted image 20251120092331.png]]

==What actually are they?==

This is a vector:
![[Pasted image 20251120093942.png]]

It has **magnitude** (size) and **direction**.
![[Pasted image 20251120094153.png]]

The length of the line shows the magnitude and the arrow points towards the direction.

You can add 2 vectors together by joining them tail to tail:
![[Pasted image 20251120094252.png]]
In addition, the order does not matter.

As an example, think of a plane flying north. There is a wind coming from the North-West.
![[Pasted image 20251120094535.png]]
The **propeller** and the **wind** are working against each other. This means that by subtracting the **wind** from the **propeller**, we get the direction the plane is going in.

Speaking of which, in order to subtract:
![[Pasted image 20251120094735.png]]
First, you reverse the direction of the vector you want to subtract. 
Then, you add them together like usual.

==NOTATION==
Vectors are written in **bold**, like **a** or **b**.

It's also written with an arrow above it, like this:
![[Pasted image 20251120095039.png]]

==CALCULATIONS==

To actually calculate them, you need to separate them into x and y values.
![[Pasted image 20251120095156.png]]
You break the vector **a** into the vectors **ax** and **ay**.

So to add 2 vectors, it would look like this:
![[Pasted image 20251120095342.png]]
When you break up a vector, each part is called a **component**.

Subtracting them is pretty much the same:
$$\begin{aligned}
&a = v + -k \\&a = (12,2) + -(4,5) = (12-4, 2-5) = (8, -3)
\end{aligned}$$ 
==MAGNITUDE==

The magnitude of a vector is shown by two vertical bars on each side:
$$\vert{a}\vert$$
Or it can also be written with 2 lines to differentiate from absolute values:
$$\vert\vert{a}\vert\vert$$
We calculate the magnitude vector using Pythagoras' theorem: 
$$\vert\vert{a}\vert\vert = \sqrt{6^2 + 8^2} = \sqrt{36+64} = \sqrt{100} = 10$$
A vector with magnitude 1 is called a **unit vector**. Their notation is a lowercase letter with a "hat", like this:
![[Pasted image 20251120102004.png]]
(Pronounced "a-hat")

==UNIT VECTORS==

A vector can be scaled off of a **unit vector**. 

In this example, vector **a**  is shown being 2.5 times the size of the magnitude of the unit vector. The direction remains unchanged. 
![[Pasted image 20251120102130.png]]

They can be used in 2 dimensions:
![vector a <em>=</em> 2x + 1.3y](https://www.mathsisfun.com/algebra/images/vector-unit-2d.svg)
Here, we show that the vector **a** is made up of 2 "x" units and 1.3 "y" unit vectors.

They can also be used in 3 (or even more!) dimensions:
![[Pasted image 20251120102433.png]]
