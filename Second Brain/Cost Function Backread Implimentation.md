# Ghist
Perhaps it is possible to discourage [[The Averaging Problem]] from becoming an issue in our [[Stock Analization and Prediction Platform]] work. Specifically, including a previous weight in the network and punishing the network for comforming to that previous weight, via modifying the [[Cost Function]]

Part of a series in #machine_learning. Definitly a #batshit_insane_idea.

# Mathematics
Normally, for [[Classification Problems]], we use the [[Mean Squared Error]]:$$C_i=\dfrac{1}{n}\sum(y_i-y_n)^2$$and $$C=\dfrac{1}{n}\sum(C_n)$$A way to punish the network would be to take the difference of this iteration's outputs and last iteration's, stating that:$$C^L=\dfrac{1}{n}\sum[(y^L_e-y^L_n)^2+(y^{L-1}_n-y^L_n)^2]$$Where we use $L$ to denote the current index of the training data. This tends to push the graph away form relying on previous values as input [^1]

```desmos-graph
left=-0; right=1;
bottom=0; top=2;
---
C(a,b,c)=(a-b)^2+(b-c)^2

C(1,0.9,x)
```

# Implimentation
In simple [[Python]] this would read
```python
def loss(y_actual, y_expected, prev_y):
	# Simple single imput implimentation
	l = (y_expected - y_actual) ** 2
	loss += (prev_y - y_actual) ** 2
	return loss
```
Implimentation varies by library however.

[^1]: Theoretically