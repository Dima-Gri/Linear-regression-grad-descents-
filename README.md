# Linear-regression-grad-descents-
Realization of Linear regression with implemented gradient descents such as GD, SGD, Momentum, Adam, Nadam and their regularized versions

For using my custom Linear Regression it's nessesary to build `descent_config` such as

```
descent_config = {
    'descent_name': '',  # descent name
    'regularized': True  # if we use regularization
    'kwargs': {          # kwargs for building choosen descent
        'dimension': X_train_transformed.shape[1],
    }
}
```
Criterion of finish descent:
1. The rate of change in scales does not change much (less than `self.tolerance`)
2. Reached maximum number of iteraions (default `300`)
