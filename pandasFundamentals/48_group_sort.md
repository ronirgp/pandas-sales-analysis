# Group and sort

We can group data, calculate a result, and then sort that result.

Example:

```python
df.groupby("category")["quantity"].sum().sort_values(ascending=False)


**Exercise:** Group by `region`, calculate the average `price`, then sort from **lowest to highest**.

# My solution
df.groupby("region")["price"].mean().sort_value(ascemding=True)