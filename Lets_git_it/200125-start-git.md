# Today I Learend..

## Mathmatics

1. Review

   - Greek alphabet : alpha ~ omega
   - Linear algebra : 
      - scalar, vector, matrix, tensor 's character
      - scalar, vector, matrix, tensor 's operation
      - special vector & matrix
      - transpose, broadcasting, linear combination, inner product, weighted sum & average
      - cosine similarity, linear regression model, sum of squares, error(residual)
      - quadratic form, submatrix

2. Practise Numpy
   
   - greek alphabet 
   ```
   display : $$\alpha$$ ,  inline ; $\beta$
   ```
   - vector code
   ```
   A = np.array([[1,2,3],[4,5,6]])
   ```
   - transpose
   ```
   A.T, A.T.T
   ```
   - special vetor & matrix
   ```
   np.zeros((3,1)), np.ones((4,1)), np.diag([1,2,3,4]), np.identity(3), np.eye(4) 
   np.arange(1,10).reshape(3,3) 
   ```
   - inner product
   ```
   X @ A
   ```
   - weighted average
   ```
   x = np.aragne(10)
   N = len(x)
   np.ones(N) @ x / N

   or

   x.mean()
   ```
   - quadratic form
   ```
   x = np.array([1,2,3])
   A = np.arange(0,10).reshape(3,3)
   x.T @ A @ x
   ```
## Git 

1. git process and command review
   - workspace -> index -> local repository -> remote repository
   - add -> commit -> push
