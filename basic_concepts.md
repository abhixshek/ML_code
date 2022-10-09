# Basic ML concepts every DS should know
## BAD DATA
### Insufficient quantity of data
### Non representative data
It is crucial to use a training set that is representative of the cases you
want to generalize to. This is often harder than it sounds: if the sample is
too small, you will have **sampling noise** (i.e., nonrepresentative data as a
result of chance), but even very large samples can be nonrepresentative if
the sampling method is flawed. This is called **sampling bias**.

### Poor quality data
It is often well worth the effort to spend time cleaning up your training data.
If some instances are missing a few features (e.g., 5% of your customers did not specify their age), you must decide whether you want to ignore this attribute altogether, ignore these instances, fill in the missing values (e.g., with the median age), or train one
model with the feature and one model without it.
### Irrelevant features
Do feature engineering


## BAD ALGORITHMS
### Overfitting the training data
Overfitting happens when the model is **too complex relative to the amount and noisiness of the training data.** Here are possible solutions:
1. Simplify the model by selecting one with fewer parameters (e.g., a linear model rather than a high-degree polynomial model), by reducing the number of attributes in the training data, or by constraining the model.
2. Gather more training data.
3. Reduce the noise in the training data (e.g., fix data errors and remove outliers).

### Underfitting the training data
Here are the main options for fixing this problem:
1. Select a more powerful model, with more parameters.
2. Feed better features to the learning algorithm (feature engineering).
3. Reduce the constraints on the model (e.g., reduce the regularization hyperparameter).

## Frame the problem
The first question to ask your boss is what exactly the business objective is.
The next question to ask your boss is what the current solution looks like (if
any)

**NOTE:** when you have only 1 output in a regression task, its called a **univariate regression** problem. 
when you have multiple outputs, its called a **multivariate regression** problem.
When multiple input features are used for a regression task, it is called a **multiple regression** problem



