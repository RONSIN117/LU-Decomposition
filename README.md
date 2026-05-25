# LU Decomposition 

## AIM:
To write a program to find the LU Decomposition of a matrix.

## Equipments Required:
1. Hardware – PCs
2. Anaconda – Python 3.7 Installation / Moodle-Code Runner

## Algorithm
1. Start the program
2. Import the necessary libraries(numpy,scipy.linalg)
3. Define the matrix using numpy
4. Use lu(),lu_solve(),lu_factor() to get the solutions
5. End the program
## Program:
(i) To find the L and U matrix
'''Program to find L and U matrix using LU decomposition.
Developed by: RONIT SINHA
RegisterNumber: 212225100040
'''
import os
os.environ["OPENBLAS_NUM_THREADS"]="1"
import numpy as np
from scipy.linalg import lu
A = np.array(eval(input()))
P,L,U=lu(A)
print(L)
print(U)


(ii) To find the LU Decomposition of a matrix

'''Program to solve a matrix using LU decomposition.
Developed by: RONIT SINHA
RegisterNumber: 212225100040
'''

import os
os.environ["OPENBLAS_NUM_THREADS"]="1"


import numpy as np
from scipy.linalg import lu_factor, lu_solve
A = np.array(eval(input()))
b = np.array(eval(input()))
lu, piv = lu_factor(A)
X = lu_solve((lu , piv),b)
print(X)



## Output:

<img width="1469" height="939" alt="image" src="https://github.com/user-attachments/assets/72b6caf4-1e65-401a-a04f-41bc1471fc5a" />
<img width="1137" height="923" alt="image" src="https://github.com/user-attachments/assets/adfebb9f-00f1-4f5d-91c8-d9f6483baa55" />



## Result:
Thus the program to find the LU Decomposition of a matrix is written and verified using python programming.

