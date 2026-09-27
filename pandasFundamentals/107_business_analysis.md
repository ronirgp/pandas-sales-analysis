# Business Analysis

## Exercise 1

Which category generated the most revenue, and how much revenue did it generate?

```python
# write your solution here

My solution:

df["total"] = df["quantity"] * df["price"]
df.groupby("category")["total"].sum().sort_values(ascending=False)