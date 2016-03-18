# Machine Learning Notes - Linear Regression

https://en.wikipedia.org/wiki/Linear_regression
https://en.wikipedia.org/wiki/Least_squares
https://en.wikipedia.org/wiki/Linear_least_squares_%28mathematics%29#Derivation_of_the_normal_equations

I used [this site](http://www.sciweavers.org/free-online-latex-equation-editor) to convert the math equations to images that I can embed in markdown.

### The hypothesis function
```latex
    h_\theta(x) = \theta_0 + \theta_1x
```
![hypothesis function](images/hypothesis_function.png)


### The cost function (or MSE)
```latex
    J(\theta_0, \theta_1) = \frac{1}{2m} \sum_{i=1}^m (h_\theta(x^{(i)}) - y^{(i)})^2
```
![cost function](images/mse_cost_function.png)


### The gradient descent algorithm
    Repeat until convergence:

```latex
    \theta_j := \theta_j -  \alpha  \frac{\partial}{\partial \theta_j} J(\theta_0, \theta_1)
    for j = 0 and j = 1
```
![gradient descent algorithm](images/gradient_descent_algorithm.png)

### Gradient descent for linear regression
```latex
    \theta_0 = \theta_0 - \alpha \frac{1}{m} \sum_{i=1}^m (h_\theta(x^{(i)}) - y^{(i)})
    \theta_1 = \theta_1 - \alpha \frac{1}{m} \sum_{i=1}^m ((h_\theta(x^{(i)}) - y^{(i)}) x^{(i)})
```
![gradient descent for linear regression theta 0](images/gd_linear_theta0.png)

![gradient descent for linear regression theta 1](images/gd_linear_theta1.png)

I got the idea to use GPs to evolve the hypothesis function and then use gradient descent to get the dependent variables, and then minimise using the mean_squared_error cost function; this will help select the best hypothesis that fits the data correctly

### Handwritten Notes:
<img src="images/my_notes_1.jpg" alt="My Notes 1" style="width: 800px;"/>

<img src="images/my_notes_2.jpg" alt="My Notes 2" style="width: 800px;"/>

<img src="images/my_notes_3.jpg" alt="My Notes 3" style="width: 800px;"/>
