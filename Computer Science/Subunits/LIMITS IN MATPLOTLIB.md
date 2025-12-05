bAssume y is the function and x is the list of numbers you're gonna run through that function.

Make a variable called y or whatever else you want to call it and write the function inside (you probably need numpy).

For Euler's number, use the .exp() function of numpy, and to raise something to a power, use .power().

For x, you can use the numpy .linspace(start, stop, num=50, endpoint=bool, dtype=None, axis = 0, device=None) function to generate an array of evenly spaced numbers. Here's what the parameters do:

start (type: *array_like*) is the starting value of the sequence.

stop (type: *array_like*) is the end value of the sequence, unless *endpoint* is *False*. In that case, the sequence excludes *stop*.

num (type: int, optional) the number of samples to generate. Default is 50. Must be positive.

endpoint (type: bool, optional) controls whether or not the value of *stop* is included in the sequence. Default is True.

retstep (type: bool, optional) if True, return (*samples*, *step*) where step is the spacing between samples.

dtype (type: *dtype*, optional) is the type of the array. If *dtype* is not given, the data type is inferred from *start* and *stop*. The data type cannot be an integer though, float will be chosen instead. 

device (type: str, optional) allows you to choose what device you want to put the array. Default is cpu, this is for like API stuff so it's not that important.

Then, you simply need to plot x and y, like this (lw controls the line width):

```
plt.plot(x, y_left_door, lw=1)
plt.plot(x, y_right_door, lw=1)
plt.xlabel('x')
plt.ylabel('y')
```

This is what the program for my Polybius task 2 looks like (try to understand what this actually does before you just copy and paste it like a lazy bum (this is for you JN)):
```
import numpy as np
import matplotlib.pyplot as plt

a = 8
x = np.linspace(-20, 20, 4000)

y_left_door = a + np.power(x + a, 100) * np.exp(-1.0/((x + a)**2))
y_right_door = np.exp(x + a) / x + np.exp(x + a)

plt.plot(x, y_left_door, lw=1)
plt.plot(x, y_right_door, lw=1)
plt.xlabel('x')
plt.ylabel('y')
plt.title('Doors')
plt.grid(True)
plt.ylim(-10000, 10000)
plt.show()
```
