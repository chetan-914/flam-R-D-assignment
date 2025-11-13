Flam R&D — AI Assignment

This project focuses on fitting a parametric curve defined by nonlinear equations using numerical optimization methods from SciPy.

📌 Parametric Model

Given parametric equations are:

$x = \left( t\cos\theta \;-\; e^{M\lvert t\rvert}\,\sin(0.3t)\,\sin\theta \;+\; X \right)$

$y = \left( 42 + t\sin\theta \;+\; e^{M\lvert t\rvert}\,\sin(0.3t)\,\cos\theta \right)$

Unknowns are: $\theta, M, X$
Given range for unknown params is : 

$ \\
0 \deg<\theta<50 \deg \\
-0.05<M<0.05 \\
0<X<100\\
$

parameter t has range: $ 6<t<60 $
🧠 Optimization Approach

Initial attempts were made using:

scipy.optimize.minimize

A general-purpose optimization algorithm that minimizes a scalar function of one or more variables.
The BFGS method is widely used and frequently applied in machine-learning optimization, such as logistic regression.

Given that we have measured data points and adjustable model parameters—similar to fitting logistic regression—this method is suitable for the task.

📚 Sources

https://www.geeksforgeeks.org/python/optimization-in-scipy/

https://www.geeksforgeeks.org/machine-learning/scipy-curve-fitting/

✅ Results

After optimization, the best-fit parameters obtained were:

𝜃=30∘
M=0.03
X=55
