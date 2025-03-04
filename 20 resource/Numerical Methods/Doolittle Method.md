**Doolittle Method** is similar to [[Crout’s or Cholesky’s Method]] except with a few minor changes to how its decomposition is structured. Matrix $A$ is decomposed into $[L][U]$ as follows:

$$
\begin{align}

\begin{bmatrix} 
a_{11} & a_{12} & a_{13} \\ 
a_{21} & a_{22} & a_{23} \\ 
a_{31} & a_{32} & a_{33} 
\end{bmatrix} &= 
\begin{bmatrix} 
1 & 0 & 0 \\ 
L_{21} & 1 & 0 \\ 
L_{31} & L_{32} & 1
\end{bmatrix} 
\begin{bmatrix} 
U_{11} & U_{12} & U_{13} \\ 
0 & U_{22} & U_{23} \\ 
0 & 0 & U_{33} 
\end{bmatrix}

\\

\begin{bmatrix} 
a_{11} & a_{12} & a_{13} \\ 
a_{21} & a_{22} & a_{23} \\ 
a_{31} & a_{32} & a_{33} 
\end{bmatrix} &=
\begin{bmatrix} 
1(U_{11}) + 0(0) + 0(0) & 1(U_{12}) + 0(U_{22}) + 0(0) & 1(U_{13}) + 0(U_{23}) + 0(U_{33}) \\ 
L_{21}(U_{11}) + 1(0) + 0(0) & L_{21}(U_{12}) + 1(U_{22}) + 0(0) & L_{21}(U_{13}) + 1(U_{23}) + 0(U_{33}) \\ 
L_{31}(U_{11}) + L_{32}(0) + 1(0) & L_{31}(U_{12}) + L_{32}(U_{22}) + 1(0) & L_{31}(U_{13}) + L_{32}(U_{23}) + 1(U_{33}) 
\end{bmatrix}

\end{align}
$$

