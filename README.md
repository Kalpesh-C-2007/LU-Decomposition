# LU Decomposition 

## AIM:
To write a program to find the LU Decomposition of a matrix.

## Equipments Required:
1. Hardware – PCs
2. Anaconda – Python 3.7 Installation / Moodle-Code Runner

## Algorithm
### (i) To find the L and U matrix
1. Import required libraries and set environment variable
Import os, numpy, and lu function from scipy.linalg. Set OPENBLAS_NUM_THREADS = 1 to control thread usage.
2. Read the matrix input
Accept a matrix from the user and convert it into a NumPy array.
3. Perform LU decomposition
Apply the lu() function to decompose the matrix into:
P → Permutation matrix
L → Lower triangular matrix
U → Upper triangular matrix
4. Display the results
Print the Lower triangular matrix (L) and Upper triangular matrix (U).

### (ii) Program to find the LU Decomposition of a matrix

1. Import required libraries such as os, numpy, and functions lu_factor and lu_solve from scipy.linalg. Set OPENBLAS_NUM_THREADS = 1.

2. Read the coefficient matrix and constant matrix from the user and convert them into NumPy arrays.

3. Apply LU factorization to the coefficient matrix using lu_factor(), and solve the system of equations using lu_solve().

4. Display the solution vector obtained after solving the equations.


## Program:
```
(i) To find the L and U matrix
'''
Program to find L and U matrix using LU decomposition.
Developed by:Kalpesh C 
RegisterNumber: 212225230121
'''
import os
os.environ["OPENBLAS_NUM_THREADS"]="1"
import numpy as np
from scipy.linalg import lu
matrix = np.array(eval(input()))
P,L,U = lu(matrix)
print(L)
print(U)
```
```
Program to find the LU Decomposition of a matrix.
'''Program to solve a matrix using LU decomposition.
Developed by: Kalpesh C
RegisterNumber: 212225230121
'''
import os
os.environ["OPENBLAS_NUM_THREADS"]="1"
import numpy as np
from scipy.linalg import lu_factor, lu_solve
matrix = np.array(eval(input()))
constant = np.array(eval(input()))
piv,lu = lu_factor(matrix)
result = lu_solve((piv,lu), constant)
print(result)
```

## Output:
![alt text](<5(1)(1).png>)
![alt text](<5(1)(2).png>)
![alt text](5(2)(1).png)
![alt text](5(2)(2).png)


## Result:
Thus the program to find the LU Decomposition of a matrix is written and verified using python programming.

