# LU Decomposition 

## AIM:
To write a program to find the LU Decomposition of a matrix.

## Equipments Required:
1. Hardware – PCs
2. Anaconda – Python 3.7 Installation / Moodle-Code Runner
## Algorithm
### Step 1:  
Import required libraries `numpy` and `scipy.linalg`.  

### Step 2:  
Input the matrix/matrices using `eval(input())`.  

### Step 3:  
Perform LU decomposition using `lu()` or solve equations using `lu_factor()` and `lu_solve()`.  

### Step 4:  
Print the results `L` and `U` matrices or solution `X` matrix. 

## Program:
(i) To find the L and U matrix
```python
import numpy as np
from scipy.linalg import lu
A = np.array(eval(input()))
P,L,U = lu(A)
print(L)
print(U)
```
(ii) To find the LU Decomposition of a matrix
```python
import numpy as np
import scipy.linalg 

A = np.array([[3, 2, 7], [2, 3, 1], [3, 4, 1]],dtype = float)
b = np.array([4, 5, 7],dtype = float)
P,L,U = scipy.linalg.lu(A)
pb = np.dot(P,b)
y = scipy.linalg.solve(L,pb)
x = scipy.linalg.solve(U,y)

print(x)
```

## Output:
(i) To find the L and U matrix
![Screenshot 2025-04-26 085301](https://github.com/user-attachments/assets/fdd59256-4b02-48dd-ba40-980c806b448c)


(ii) To find the LU Decomposition of a matrix
![Screenshot 2025-04-26 085324](https://github.com/user-attachments/assets/a73b9e59-464f-4da6-a5f3-fad39193a999)



## Result:
Thus the program to find the LU Decomposition of a matrix is written and verified using python programming.
