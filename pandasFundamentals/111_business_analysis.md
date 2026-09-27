# Business Analysis

## Exercise 1

Which category has the highest average order sales value?


```python
# write your solution here

My solution:

df["total"] = df["quantity"] * df["price"]

df.groupby("category")["total"].mean()