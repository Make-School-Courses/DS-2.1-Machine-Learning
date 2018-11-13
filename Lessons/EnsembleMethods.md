# Ensemble methods

- Ensemble Methods are machine learning algorithms that rely on the "Wisdom of the Crowd"

- Many weak algorithms working together do better than 1 big, monolithic algorithm

- They are two major groups for ensemble methods: ***Random Forests*** and ***Gradient Boosted Trees***

```python
from sklearn.tree import DecisionTreeRegressor
import numpy as np
from sklearn.tree import export_graphviz
import pydotplus

X = np.array([5, 7, 12, 23, 25, 28, 29, 34, 35, 40])

Y = np.array([-52, -54, -31, -16, 38, -7, 70, 55, -35, 32])

regre = DecisionTreeRegressor(max_depth=1)
print(X.reshape(-1, 1))
print([[i, j] for (i, j) in zip(X, Y)])
regre.fit(X.reshape(-1, 1), Y.reshape(-1, 1))

dot_data = export_graphviz(regre, out_file=None)

# Draw graph
graph = pydotplus.graph_from_dot_data(dot_data)
graph.write_png('reg_tree.png')
```
![](../Notebooks/Images/reg_tree.png){.center}
