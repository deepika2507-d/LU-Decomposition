# LU Decomposition 

## AIM:
To write a program to find the LU Decomposition of a matrix.

## Equipments Required:
1. Hardware – PCs
2. Anaconda – Python 3.7 Installation / Moodle-Code Runner

## Algorithm
1. Import Library: Import the NumPy library as np.

2.Define Matrix: Create a 2D NumPy array a with the given elements.

3.Compute Eigenvalues and Eigenvectors: Use np.linalg.eig(a) to calculate the eigenvalues and eigenvectors.

4.Display Result: Print the eigenvalues and eigenvectors.
 

## Program:
(i) To find the L and U matrix

'''Program to find L and U matrix using LU decomposition.
Developed by: Deepika.V
RegisterNumber: 24000724
'''
import numpy as np

from scipy.linalg import lu

A = np.array(eval(input()))

P,L,U = lu(A)

print(L)

print(U)
```
(ii) To find the LU Decomposition of a matrix
```
/*
Program to find the LU Decomposition of a matrix.
'''Program to solve a matrix using LU decomposition.
Developed by: Deepika.V
RegisterNumber: 24000724

import numpy as np

from scipy.linalg import lu_factor, lu_solve

a = np.array(eval(input()))

b = np.array(eval(input()))

lu, piv = lu_factor(a)

x = lu_solve((lu, piv), b)

print(x)

## Output:
'''Program to solve a matrix using LU decomposition.
Developed by: Deepika.V
RegisterNumber: 24000724
'''
# To print X matrix (solution to the equations)

import numpy as np

from scipy.linalg import lu_factor, lu_solve

a = np.array(eval(input()))

b = np.array(eval(input()))

lu, piv = lu_factor(a)

x = lu_solve((lu, piv), b)

print(x)


## Result:
Thus the program to find the LU Decomposition of a matrix is written and verified using python programming.

