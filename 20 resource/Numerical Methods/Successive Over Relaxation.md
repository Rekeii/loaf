**Successive Over Relaxation Method** is an iterative method that is an extension of [[Gauss-Seidel Method]]. The difference between the two is the introduction of the relaxation factor, $\omega$. This aims to speed up the update rate of the variables, leading us to need less time to arrive at the convergence. The formula is as follows:
$$

x_i^{(k+1)} = (1 - \omega)x_i^{(k)} + \frac{\omega}{a_{ii}}\left(b_i - \sum_{j=1}^{i-1} a_{ij}x_j^{(k+1)} - \sum_{j=i+1}^{n} a_{ij}x_j^{(k)}\right)

$$
OR:

$$
x^k_{i} = \omega \cdot [eqn] + (1-\omega ) (x^{(k-1)}_{i})
$$
where, $(x^{(k-1)}_{i})$ is simply the value of $x_{i}$ at the preceding iteration. Then continue solving iteratively until the desired $E_{A}$ is reached.
$$
E_{A} = |present - past|
$$
