# Business Analysis

## Exercise 1

Which product sold the most units?

```python
# write your solution here

My solution:

df["total"] = df["quantity"] * df["price"]
df.groupby("product")["total"].sum().sort(ascending=False)