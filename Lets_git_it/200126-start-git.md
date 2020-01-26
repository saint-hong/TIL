# Today I Learend..

## Mathmatics

1. Review
   - matrix & vector scale character :
      - positive definite, positive semi definite
      - notion of norm, trace, determinent and character
      - especially, determinent was the most difficult to understand.
      - but, it was good to know function of cofactor expansion, minor. 
   - system of linear equations & inverse matrix
   - least square problem
   - pseudo inverse
   - residure sum of squares

2. Practise Numpy
   - norm code
   ```
   import nmpy as np
   A = np.arange(9).reshape(3,3)

   np.linalg.norm(A)
   ```
   - trace code
   ```
   np.trace(np.eye(3))
   ```
   - determinent code
   ```
   A = np.array([[1,2,3],[4,5,6],[7,8,9]])

   np.linalg.det(A)
   ```
   - inverse matrix code
   ```
   import numpy as np

   A = np.array([[1,1,0],[0,1,1],[1,1,1]])

   Ainv = np.linalg.inv(A)
   ```
   - lstsq code
   ```
   b = np.array([[1],[2],[3]])
   x, np.linalg.lstsq(A, b)
   ```
   - pseudo inverse code
   ```
   !!! especially, if matrix A is not square matrix, A's inverse matrix = pseudo inverse
   Ainv = np.linalg.inv(A.T @ A) @ A.T
   ```
## Python..

1. Review
   - map, filter, reduce
   - decorator

