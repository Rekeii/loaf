**Crout's Method** utilizes [[LU Decomposition]] wherein we break down a matrix into two simpler matrices: : a lower triangular matrix $L$ and an upper triangular matrix 
$U$. Hence, it is represented mathematically as:

$$
|A| = [L][U]
$$
- $|A|$ - represents matrix A or our original matrix.
- $[L]$ - represents the *lower* triangular matrix derived from A.
- $[U]$ - represents the *upper* triangular matrix derived from A.

Since per properties of matrices, matrix A is equivalent to the two triangular matrices, lower and upper. This decomposition allows us to now solve linear equations by substituting the decomposition of matrix A in a typical linear equation with:
$$
\begin{align}
Ax&=b\\
LUx&=b 
\end{align}
$$
Thus, we can now solve for the equation as follows:
$$
\begin{align}
Ly&=b \\
Ux&=y
\end{align}
$$

> [!faq] Why does it work?
> Recall that in Linear Algebra, $Ax=b,$ is the standard form when we want to represent systems of linear equations where,
> - $A$ is the coefficient matrix.
> - $x$ is the vector of unknown variables.
> - $b$ is the result vector.
> 
> After which, as per the properties of matrices, we can now employ substitution. 
> 
> **Solving** $Ly = b$,  Since $L$ is a lower triangular matrix, you can start solving for $y$ from the top row down, using forward substitution.
> **Solving** $Ux = y$, Since we now have $y$, we can now solve for $x$ using the upper triangular matrix $U$. This uses backward substitution.

Now Crout's method does the aforementioned steps, matrix decomposition, however what differs is that the **diagonal of the upper triangular matrix $[U]$ are all 1s**.

$$
\begin{align}

\begin{bmatrix} 
a_{11} & a_{12} & a_{13} \\ 
a_{21} & a_{22} & a_{23} \\ 
a_{31} & a_{32} & a_{33} 
\end{bmatrix} &= 
\begin{bmatrix} 
L_{11} & 0 & 0 \\ 
L_{21} & L_{22} & 0 \\ 
L_{31} & L_{32} & L_{33} 
\end{bmatrix} 
\begin{bmatrix} 
1 & U_{12} & U_{13} \\ 
0 & 1 & U_{23} \\ 
0 & 0 & 1 
\end{bmatrix}

\\

\begin{bmatrix} 
a_{11} & a_{12} & a_{13} \\ 
a_{21} & a_{22} & a_{23} \\ 
a_{31} & a_{32} & a_{33} 
\end{bmatrix} &=
\begin{bmatrix} 
L_{11}(1) + 0(0) + 0(0) & L_{11}(U_{12}) + 0(1) + 0(0) & L_{11}(U_{13}) + 0(U_{23}) + 0(1) \\ 
L_{21}(1) + L_{22}(0) + 0(0) & L_{21}(U_{12}) + L_{22}(1) + 0(0) & L_{21}(U_{13}) + L_{22}(U_{23}) + 0(1) \\ 
L_{31}(1) + L_{32}(0) + L_{33}(0) & L_{31}(U_{12}) + L_{32}(1) + L_{33}(0) & L_{31}(U_{13}) + L_{32}(U_{23}) + L_{33}(1) 
\end{bmatrix}

\end{align}
$$

That looks complicated! But it's actually just matrix multiplication and the dot product. Every element is calculated as:
$$ 
[ c_{ij} = a_{i1}b_{1j} + a_{i2}b_{2j} + a_{i3}b_{3j} ]
$$
Where visually, if we want to calculate for $a_{11}$, we can obtain its formula as such:
$$
\begin{bmatrix} 
L_{11} & 0 & 0 \\ 
\end{bmatrix}

\cdot
\begin{bmatrix} 
1  \\ 
0 \\ 
0 
\end{bmatrix}
= L_{11} \cdot 1 + 0\cdot 0 + 0\cdot 0 = L_{11} 
$$




