# Learning-ML

This project is designed for students learning the basics of data visualization and linear regression using Python. The code helps you understand how to create scatterplots, draw regression lines, and analyze relationships between variables.

---

## **Installation and Setup**

### 1. Lib
Ensure you have the following libraries installed in your Python environment: pandas, matplotlib, statsmodels

### 2. Install Package 
You can install them using:
```plaintext
pip install pandas matplotlib statsmodels
```

## **Code Overview**

### 1. Scatterplot with Data Points
Create a scatterplot to see how two variables (SAT and GPA) are related:
```plaintext
plt.scatter(x, y)
plt.xlabel('SAT', fontsize=20)
plt.ylabel('GPA', fontsize=20)
plt.show()
```

### 2. Run a Simple Linear Regression
Use statsmodels to calculate the regression equation and get a summary:
```plaintext
x1 = sm.add_constant(x)
results = sm.OLS(y, x1).fit()
print(results.summary())
```

### 3. Adding Regression Lines
We’ll add different types of regression lines to understand their effects:
```python
plt.scatter(x, y)
yhat = 0.0017 * x + 0.275  # Regression equation
plt.plot(x, yhat, lw=4, c='orange', label='Regression Line')
plt.xlabel('SAT', fontsize=20)
plt.ylabel('GPA', fontsize=20)
plt.show()
```
