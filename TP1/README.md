In this colab, we will study basic linear and non-linear regression algorithms. Regression is another name for function approximation,
it consists in fitting a function to a set of points.

The colab is meant to study elements presented in lessons available in video here https://www.youtube.com/playlist?list=PLe5mY-Da-ksURGcelU-egwtWZXxVgZ76a

The objective of regression or function approximation is to create a model from observed data.
The model has a fixed structure with parameters (like the coefficients of a polynomial for instance),  and regression consists in adjusting these parameters to fit the data. In machine learning, it is a very important technique since having a good model enables better predictions and performance.

Generally speaking, given some data $\{ ({\bf x}^{(i)}, {\bf y}^{(i)}) \}$, the goal is to adjust a model ${\bf y} = f({\bf x})$ so that the *learned* function $f$ accounts for datapoints and generalize well to other unseen points. 

The simplest case is linear regression, which assumes a relation of type ${\bf y} = {\bf A}{\bf x} + {\bf b}$ between the data ${\bf x}$ and ${\bf y}$.

Several methods exist to adjust the parameters ${\bf A}$ and ${\bf b}$, the most well-known being the least squares method (or least norm in the multivariate case).

In this lab, we assume that ${\bf y}$ is of dimension 1 (and write $y$ instead of ${\bf y}$ in what follows). This is a very common assumption.

Furthermore, in the code ${\bf x}$ is also of dimension 1, this is more restrictive as regression is often used from multidimensional input data.
