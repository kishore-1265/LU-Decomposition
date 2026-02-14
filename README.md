# LU Decomposition 

## AIM:
To write a program to find the LU Decomposition of a matrix.

## Equipments Required:
1. Hardware – PCs
2. Anaconda – Python 3.7 Installation / Moodle-Code Runner

## Algorithm
### Step 1: 
Import the numpy module to use the built-in functions for calculation
### Step 2: 
Prepare the lists from each linear equations and assign in np.array()
### Step 3:
Using the functions lu(), lu_factor(), lu_solve() we can find the rank of the given matrix.
### Step 4: 
End the program

## Program:
(i) To find the L and U matrix
```
/*
Program to find the L and U matrix.
Developed by: Kishore R
RegisterNumber: 25011776
*/

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
Developed by: Kishore R
RegisterNumber: 25011776
*/

import numpy as np
from scipy.linalg import lu_factor, lu_solve
A = np.array(eval(input()))
B = np.array(eval(input()))
lu, pivot = lu_factor(A)
X = lu_solve((lu, pivot),B)
print(X)
```

## Output:
(i)
<img width="737" height="728" alt="Screenshot 2026-02-14 175053" src="https://github.com/user-attachments/assets/67bcb1af-a8ba-440f-bec9-bc9e9ecb0d4d" />
(ii)
<img width="593" height="565" alt="Screenshot 2026-02-14 175103" src="https://github.com/user-attachments/assets/b4aa31e6-bb5b-4c13-9bb6-ddf6dd0fa949" />




## Result:
Thus the program to find the LU Decomposition of a matrix is written and verified using python programming.

