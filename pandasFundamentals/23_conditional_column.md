# Conditional column

We can create a new column based on a condition.

Example:

```python
df["large_order"] = df["quantity"] > 3


### Your task

Create **`high_price`** based on this rule:

> If `price` is greater than **100**, return `True`; otherwise `False`.

Don't copy the example—write the code yourself.
# My solution

df["hight_price"] = df["price"] >  100 