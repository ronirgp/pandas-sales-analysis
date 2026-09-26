# Business Analysis

## Exercise 1

Which category has the highest total sales value?

```python
# write your solution here

My solution:
df["total"] = df["quantity"] * df["price"]

df.groupby("category")["total"].sum().sort_values(ascending=False)