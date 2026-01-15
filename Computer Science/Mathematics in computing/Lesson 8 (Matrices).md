**Tensors**: Matrices stacked on top of matrices

There are many types of matrices. I should probably start with that.

A matrix is an array of numbers:
![[Pasted image 20260115104212.png]]

It has a __main diagonal__ running down the "middle":
![[Pasted image 20260115104233.png]]
That stays the same even when transposed (and when the matrix isn't square, read on):
![[Pasted image 20260115104249.png]]

A transpose is where we flip the rows and columns of the matrix (notice the main diagonal stays the same):
![[Pasted image 20260115104341.png]]

The types are:

Square matrices, that have the same number of rows and columns:
![[Pasted image 20260115104432.png]]
![[Pasted image 20260115104436.png]]

Identity matrices, noted as I, are square matrices, and only consist of 1 on the main diagonal and 0 everywhere else:
![[Pasted image 20260115104545.png]]
Thus, if we multiply a matrix by an identity matrix, the result stays the same.

Diagonal matrices, as the name implies, have values only on the main diagonal but 0 everywhere else:
![[Pasted image 20260115104650.png]]

A scalar matrix (you might remember this from vectors) has the same value along its main diagonal, but 0 everywhere else:
![[Pasted image 20260115104720.png]]

Triangular matrices have 2 types: __lower__ and __upper__. Lower, when all the values above the main diagonal are 0. Upper when all the values below the main diagonal are 0.
![[Pasted image 20260115104859.png]]
![[Pasted image 20260115104906.png]]

A zero matrix is a matrix with the value of 0 everywhere:
![[Pasted image 20260115104929.png]]

A symmetric matrix is where both sides of the main diagonal mirror each other:
![[Pasted image 20260115105026.png]]
It has to be square, and is equal to its own transpose. 

This one is hard, but a hermitian matrix is a __symmetric matrix, except for its imaginary numbers, which swap signs across the main diagonal__:

![[Pasted image 20260115105211.png]]

==OPERATIONS WITH MATRICES==

Adding is simple. 2 matrices must have the same number of rows and columns to add together. Then, just add each number together one by one:
![[Pasted image 20260115105440.png]]
The same goes with negatives. 
![[Pasted image 20260115105504.png]]

Subtracting also works the same:
![[Pasted image 20260115105530.png]]
Multiplying by a constant is also relatively easy, just multiply all the numbers in the matrix by that number:
![[Pasted image 20260115105656.png]]


To multiply 2 matrices together you need to find the __cross product__ of both matrices. To do this, you take each row of the first matrix, and multiply it by each column of the second matrix.
![[Pasted image 20260115110110.png]]
![[Pasted image 20260115110123.png]]