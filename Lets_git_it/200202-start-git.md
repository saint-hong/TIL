# Today I Learend..

## Mathmatics

1. Review
   - PCA : Principal Componet Analysis
      - concept : dimension reduction
      - details : latent variable, low-rank approximation
      - mathematical definition
      ```
      $$
      \begin{align}
      \ \hat{\hat{x}} = W U \hat{x} = \hat{x}
      \end{align}
      $$
      
      $$
      \begin{align}
      WU = I
      \end{align}
      $$

      $$
      \begin{align}
      \arg\min_{\hat{x}} || x - U \hat{x} ||^2
      \end{align}
      $$

      $$
      \begin{align}
      \arg\min_{W} \sum_{i=1}^N || x_i - W^{T} W x_i ||^2
      \end{align}
      $$  
      ```
      - scikit-learn code
      ```
      from sklearn.decomposition import PCA

      pca1 = PCA(n_comonents=1)
      X_low = pca1.fit_transform(X)
      X2 = pca1.inverse_transform(X_low)
      ...
      ```
   - Function
      - sign function, Heaviside step function, indicator function, inverse function
      ```
      def f(x):
          return 2*x
      x = 10
      y = f(x)
      ```
      ```
      1)sign function..
      np.sign()
      
      2)Heaviside step function..
      def heaviside_step(x):
      if isinstance(x, np.ndarray):
        return np.where(x >= 0, 1, 0)
      else:
      return 1.0 if x >= 0 else 0.0
      ```
      - A function that is used well in data analysis
      ```
      1)polynomial
      
      2)ReLU
      plt.plot(xx, np.maximum(xx,0))
      
      3)exponetial function
      np.exp()

      4)logistic function
      def logistic(x):
         return 1 / (1+np.exp(-x)

      5)log
      np.log()

      6)softplus
      def softplus(x):
         return np.log(1+np.exp(x))
      ```
    - Differentiation
       - optmization, slpe, derivative, partial differentiation
       - Schwarz's theorem
       - Taylor expansion
       - SymPy...
      ``` 
      import sympy
      sympy.init_printing(use_latex='mathjax')
      x = sympy.symbols('x')

      sympy.diff(f)

      sympy.diff(f,x)

      sympy.diff(f,x,x)
      ```
   - Integral : indefinite integral, definite integral
      - Fundamental Theorem of Calculus
      - SymPy
      ```
      sympy.integrate(f)
      sympy.integrate(f,x)

      (F.subs(x,2)-F.subs(x,0)).evalf()

      수치적분
      sp.integrate.quad(f, 0, 2)
      
      다변수 정적분
      dblquad(func, a, b, gfun, hfun)
      or
      dblquad(func, 1, 10, lambda x:0, lambda x:10)

2. Read and studied
   - grid search, steepest gradient, Newton method
   - Lp : Linear Programming
   - QP : Quadratic Programming
   - Lagrange multiplier, KKT







