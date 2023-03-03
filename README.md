# test



**Sigmoid Function (Logistic Function)**

Logistic regression algorithm also uses a linear equation with independent predictors to predict a value. The predicted value can be anywhere between negative infinity to positive infinity. We need the output of the algorithm to be class variable, i.e 0-no, 1-yes. Therefore, we are squashing the output of the linear equation into a range of [0,1]. To squash the predicted value between 0 and 1, we use the sigmoid function.





We take the output(z) of the linear equation and give to the function g(x) which returns a squashed value h, the value h will lie in the range of 0 to 1. To understand how sigmoid function squashes the values within the range, let’s visualize the graph of the sigmoid function.


As you can see from the graph, the sigmoid function becomes asymptote to y=1 for positive values of x and becomes asymptote to y=0 for negative values of x.

![image](https://user-images.githubusercontent.com/89921883/222824767-a82f2052-6efe-46fa-9c21-c001fc89e476.png)

---



**Cost Function**
Since we are trying to predict class values, we cannot use the same cost function used in linear regression algorithm. Therefore, we use a logarithmic loss function to calculate the cost for misclassifying.

![image](https://user-images.githubusercontent.com/89921883/222825691-a3695da9-6cfa-4305-b38a-38a38c564b86.png)

---


**Calculating Gradients**
We take partial derivatives of the cost function with respect to each parameter(theta_0, theta_1, …) to obtain the gradients. with the help of these gradients, we can update the values of theta_0, theta_1, … To understand the equations below you would need some calculus.

![image](https://user-images.githubusercontent.com/89921883/222826236-eb01297b-4943-4b9e-b7e1-ebac1d4eac34.png)
