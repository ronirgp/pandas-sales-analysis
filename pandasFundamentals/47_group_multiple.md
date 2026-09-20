# Group with multiple calculations

`agg()` lets us perform multiple calculations on the same column.

Example:

```python
df.groupby("region")["quantity"].agg(["sum", "mean"])


**Exercise:** Group by `category` and find the **minimum and maximum price** for each category.

# My solution
df.groupby("category")["price"].agg(["min", "max"])