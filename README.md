# LU Decomposition 

## AIM:
To write a program to find the LU Decomposition of a matrix.

## Equipments Required:
1. Hardware – PCs
2. Anaconda – Python 3.7 Installation / Moodle-Code Runner

## Algorithm
Step1 :Import the numpy module to use the built-in functions for calculation.
Step 2:Prepare the lists from each equations and assign in np.array()
Step 3:Using the np.linalg.eig(), we get two results (first is eigenvalue and second is eigenvector) of the given matrix.
Step 4:End the program

## Program:
(i) To find the L and U matrix
```Python
'''Program to find L and U matrix using LU decomposition.
Developed by: LOGU R
RegisterNumber: 212224230141 
'''
import numpy as np
from scipy.linalg import lu
A = np.array(eval(input()))
P,L,U = lu(A)
print(L)
print(U)
```
(ii) To find the LU Decomposition of a matrix
```Python
'''Program to solve a matrix using LU decomposition.
Developed by: LOGU R 
RegisterNumber: 212224230141
'''

# To print X matrix (solution to the equations)
import numpy as np
from scipy.linalg import lu_factor,lu_solve
A = np.array(eval(input()))
B = np.array(eval(input()))
lu,piv = lu_factor(A)
X = lu_solve((lu,piv),B)
print(X)
```

## Output:
<img width="1201" height="454" alt="image" src="https://github.com/user-attachments/assets/430e03d3-d232-437d-ae1c-306d3a8bd1f3" />
<img width="884" height="186" alt="image" src="https://github.com/user-attachments/assets/c16fd20d-9d5f-4011-b0a1-953d99023afe" />



## Result:
Thus the program to find the LU Decomposition of a matrix is written and verified using python programming.

