**Linear Regression** is a type of curve fitting where the curve depicted is a straight line (hence why it is linear). This method utilizes the *least-squares method*.  This method is used to model the relationship between a dependent variable (y) and one or more independent variables (x). Through this method, we should be able to find the straight line that best fits the data points and is represented as such:
$$y=mx+b \qquad OR \qquad  y = a_{0}+a_{1}x  $$

When doing Linear Regression you need the following values:
- $x$
- $y=f(x)$
- $xy$
- $x^2$
- $y^2$
- $y_{(model)}$
- $e=y-y_{(model)}$
- $\sum x$, $\sum y$, $\sum xy$, $\sum x^2$, $\sum y^2$

To find $m$ or $a_{1}$:
$$
a_1 = \frac{n \sum x_i y_i - \sum x_i \sum y_i}{n \sum x_i^2 - (\sum x_i)^2}
$$

To find $b$ or $a_{0}$:
$$
a_{0} = \bar{y} - a_{1}\bar{x}
$$

The correlation coefficient is calculated as follows:
$$
r = \frac{n \sum xy - (\sum x)(\sum y)} {\sqrt{n \sum x^2 - (\sum x)^2} \sqrt{n \sum y^2 - (\sum y)^2}}
$$


