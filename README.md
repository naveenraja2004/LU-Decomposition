# LU Decomposition 

## AIM:
To write a program to find the LU Decomposition of a matrix.

## Equipments Required:
1. Hardware – PCs
2. Anaconda – Python 3.7 Installation / Moodle-Code Runner

## Algorithm : 
1.Read the elements of augmented matrix into arrays a and b.
2.Calculate elements of L and U.
3.Print elements of L and U.
4.Find V by solving LV = B by forward substitution.
5.Find X by solving UX = V by backward substitution.
6.Print Array X as the solution. 

## Program:
(i) To find the L and U matrix
```
'''Program to find L and U matrix using LU decomposition.
Developed by: Naveen Raja N.R
RegisterNumber: 212222230093
'''
import numpy as np
from scipy.linalg import lu
arr=np.array(eval(input()))
P,L,U=lu(arr)
print(L)
print(U)
```
(ii) To find the LU Decomposition of a matrix
```
'''Program to solve a matrix using LU decomposition.
Developed by: naveen raja 
RegisterNumber: 212222230093
'''

# To print X matrix (solution to the equations)
import numpy as np
from scipy.linalg import lu_factor,lu_solve
arr=np.array([[3, 2, 7],[2, 3, 1],[3, 4, 1]])
B=np.array([4, 5, 7])
LU,P=lu_factor(arr)
res=lu_solve((LU,P),B)
print(res)
```

## Output:
1)
![naveen exp 5 cr](https://github.com/naveenraja2004/LU-Decomposition/assets/118707204/eeffafc0-650d-4d51-a391-cc84272b3e1d)
2)
![naveen exp 5cr 2](https://github.com/naveenraja2004/LU-Decomposition/assets/118707204/7dd7736c-577a-41d8-bed1-6d2101379640)


## Result:
Thus the program to find the LU Decomposition of a matrix is written and verified using python programming.

