# LU Decomposition 

## AIM:
To write a program to find the LU Decomposition of a matrix.

## Equipments Required:
1. Hardware – PCs
2. Anaconda – Python 3.7 Installation / Moodle-Code Runner

## Algorithm
(i)
1.Start

2.Read the input matrix A.

3.Call the LU decomposition function:
   P, L, U = lu(A)

   P is the permutation matrix (used internally)

   L is the lower triangular matrix

   U is the upper triangular matrix

   Print the matrices L and U.

4.End
(ii)
1.Start

2.Read the coefficient matrix A and the right-hand side vector b.

3.Compute LU decomposition using:
   lu, piv = lu_factor(A)

   lu contains the combined LU matrix

   piv stores pivoting information

   Solve the system using:
   x = lu_solve((lu, piv), b)

   Print the solution vector x.

4.End
 

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
(ii) To find the LU Decomposition of a matrix
``

import numpy as np

from scipy.linalg import lu_factor, lu_solve

a = np.array(eval(input()))

b = np.array(eval(input()))

lu, piv = lu_factor(a)

x = lu_solve((lu, piv), b)

print(x)

output:

![Screenshot 2025-04-26 220311](https://github.com/user-attachments/assets/5c817175-1f19-49d0-98aa-cd1371f16c51)

![Screenshot 2025-04-26 220410](https://github.com/user-attachments/assets/c4c5e13f-69bf-435c-9cf9-d6be0f614292)


## Result:
Thus the program to find the LU Decomposition of a matrix is written and verified using python programming.


```
