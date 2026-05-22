# LU Decomposition 

## AIM:
To write a program to find the LU Decomposition of a matrix.

## Equipments Required:
1. Hardware – PCs
2. Anaconda – Python 3.7 Installation / Moodle-Code Runner

## Algorithm
1. 
2. 
3. 
4. 

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

Program to find the LU Decomposition of a matrix.
'''Program to solve a matrix using LU decomposition.
Developed by: Kalpesh C
RegisterNumber: 212225230121
'''
```
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

