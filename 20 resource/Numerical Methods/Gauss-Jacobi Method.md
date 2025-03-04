**Gauss-Jacobi Method** is an iterative method used to solve linear systems of equations. It is fairly simple and can be done in a few steps:

When no initial values are set, we are safe to assume it is zero.

1. **Rearrange the equations.** We must rearrange the equations in that we put the variable with the largest coefficient within the diagonal of all the equations. This is just for ease of use so we can ensure the unknown variables are already isolated.
2. **Obtaining the iterative Formula.** We must solve for the dominant variable by isolating that same variable on one side of the equation, then dividing the coefficient on the remaining terms on the other side of the equation. 
3. **Iterations.** You may now solve for every iteration, assuming zero is the initial value when no initial value is set. Here, you must simply substitute the unknowns with your initial value and do it iteratively till you reach the predefined absolute error.
