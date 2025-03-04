**Polynomial Regression** is a type of curve fitting where it can take various shapes depending on the equation. This is because Polynomial Regression can also be utilized with nonlinear equations, compared to Linear Regression which is strictly limited to linear equations. It models the relationship between the dependent variable $y$ and one or more independent variables $x$ using a polynomial equation.
$$
y = a_{0}+a_{1}x + a_{2}x^2
$$
When doing Polynomial Regression you need the following values. Note that this is subjective on your polynomial:
- $x$
- $y=f(x)$
- $xy$
- $x^2$
- $y^2$
- $y_{(model)}$
- $e=y-y_{(model)}$
- $\sum x$, $\sum y$, $\sum x^2$, $\sum x^3$, $\sum y^4$, $\sum xy$, $\sum x^2 y$  

Afterwards, construct your equation, here we are tackling a 2nd order polynomial regression hence the equations are as follows:
$$
\begin{align}
\sum y_{i} &= na_{0}+ \sum x_{1}a_{1}+\sum x^2_{i} a_{2} \\ 
\sum x_{i}y_{i} &= \sum x_{1}a_{0}+\sum x^2_{i} a_{1} + \sum x^3_{i} a_{2}\\ 
\sum x^2_{i}y_{i} &= \sum x^2_{i} a_{0} + \sum x^3_{i} a_{1} + \sum x^4_{i} a_{2}\\
\end{align}
$$
Now use matrices to obtain your unknown values. This is just $Ax=b$ 