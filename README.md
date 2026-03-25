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
```
/*
Program to find the L and U matrix.
Developed by: kirupasagar.s
RegisterNumber: 212224230126
*/
import numpy as np
from scipy.linalg import lu
A = np.array(eval(input()))
P,L,U=lu(A)
print(L)
print(U)
```
###
(ii) To find the LU Decomposition of a matrix
```
/*
Program to find the LU Decomposition of a matrix.
Developed by:  kirupasagar.s
RegisterNumber:  212224230126
*/
import numpy as np
from scipy.linalg import lu, lu_solve, lu_factor
A = np.array(eval(input()))
b = np.array([4,5,7], dtype=float)
lu_, piv = lu_factor(A)
x = lu_solve((lu_, piv), b)
print(x)
```
###
## Output:
<img width="1449" height="904" alt="Screenshot 2026-03-25 111231" src="https://github.com/user-attachments/assets/235b5e87-8ce5-4a2c-a60d-1dbbe53fb354" />
<img width="1344" height="702" alt="Screenshot 2026-03-25 111300" src="https://github.com/user-attachments/assets/cf370264-6519-4ed9-bdac-6c51c2135dd4" />
<img width="1422" height="899" alt="Screenshot 2026-03-25 111324" src="https://github.com/user-attachments/assets/c2d7862e-97de-4f3a-baee-ba78f808f8fa" />
<img width="1289" height="399" alt="Screenshot 2026-03-25 111342" src="https://github.com/user-attachments/assets/f641cf09-4092-4530-8950-123941a8d565" />


## Result:
Thus the program to find the LU Decomposition of a matrix is written and verified using python programming.

