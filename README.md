# LU Decomposition 

## AIM:
To write a program to find the LU Decomposition of a matrix.

## Equipments Required:
1. Hardware – PCs
2. Anaconda – Python 3.7 Installation / Moodle-Code Runner

## Algorithm

Step 1: Import the required libraries such as NumPy and SciPy.

Step 2: Define the matrix using np.array() and store it in a variable.

Step 3: Use the scipy.linalg.lu() function to perform LU Decomposition and obtain the lower triangular matrix (L), upper triangular matrix (U), and permutation matrix (P).

Step 4: Display the matrices P, L, and U using the print() function.

## Program:
(i) To find the L and U matrix
```
Program to find the L and U matrix.
Developed by: SARANYA R
RegisterNumber:212225040384

import os
os.environ["OPENBLAS_NUM_THREADS"]="1"
import numpy as np
from scipy.linalg import lu
A=np.array(eval(input()))
P,L,U=lu(A)
print(L)
print(U)

```
(ii) To find the LU Decomposition of a matrix
```

Program to find the LU Decomposition of a matrix.
Developed by: SARANYA R
RegisterNumber: 212225040384

import os
os.environ["OPENBLAS_NUM_THREADS"]="1"
import numpy as np
from scipy.linalg import lu_factor,lu_solve
A=np.array(eval(input()),dtype='i')
B=np.array(eval(input()),dtype='i')
X=lu_factor(A)
solution=lu_solve(X,B)
print(solution)

```

## Output:
The L and U Matrix
<img width="1229" height="571" alt="image" src="https://github.com/user-attachments/assets/dc185d09-7bc3-4a53-8e00-26342efed4e3" />

The LU Decomposition of a matrix
<img width="1009" height="325" alt="image" src="https://github.com/user-attachments/assets/e07c88d6-f65f-4312-a888-9aa4d5515764" />


## Result:
Thus the program to find the LU Decomposition of a matrix is written and verified using python programming.

