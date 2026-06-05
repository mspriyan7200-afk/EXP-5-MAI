# LU Decomposition 

## AIM:
To write a program to find the LU Decomposition of a matrix.

## Equipments Required:
1. Hardware – PCs
2. Anaconda – Python 3.7 Installation / Moodle-Code Runner

## Algorithm 
## FINDING L AND U MATRIX
1.Start the program.

2.Import the required libraries (NumPy and SciPy).

3.Read the input matrix A from the user.

4.Convert the input into a NumPy array.

5.Apply the LU decomposition using the lu() function.

6.Obtain the matrices P (Permutation Matrix), L (Lower Triangular Matrix), and U (Upper Triangular Matrix).

7.Display the L matrix.

8.Display the U matrix.

9.Stop the program.

## FINDING LU DECOMPOSITION OF MATRIX

1.Import the required libraries (NumPy and SciPy).

2.Read the coefficient matrix A from the user.

3.Read the constant matrix/vector B from the user.

4.Convert both inputs into NumPy arrays.

5.Perform LU factorization of matrix A using the lu_factor() function.

6.Obtain the LU-factored matrix and pivot indices.

7.Use the lu_solve() function with the LU factors and constant matrix B.

8.Compute the solution vector X.

9.Display the solution vector X.



## Program:
(i) To find the L and U matrix
```
/*
Program to find the L and U matrix.
Developed by: M PRIYAN
RegisterNumber: 212225040320
*/
import os
os.environ["OPENBLAS_NUM_THREADS"]="1"
import numpy as np
from scipy.linalg import lu
matrix = np.array(eval(input()))
P,L,U=lu(matrix)
print(L)
print(U)

```
(ii) To find the LU Decomposition of a matrix
```
/*
Program to find the LU Decomposition of a matrix.
Developed by: M PRIYAN
RegisterNumber: 212225040320
*/

# To print X matrix (solution to the equations)
import os
os.environ["OPENBLAS_NUM_THREADS"]="1"
import numpy as np
from scipy.linalg import lu_factor,lu_solve
matrix=np.array(eval(input()))
constant=np.array(eval(input()))
piv,lu=lu_factor(matrix)
result=lu_solve((piv,lu),constant)
print(result)
```

## Output:
![lu decomposition]()
![alt text](EXP5(A).png)
![alt text](EXP5(B).png)

## Result:
Thus the program to find the LU Decomposition of a matrix is written and verified using python programming.

