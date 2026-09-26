# Business Analysis

## Exercise 1

Which product generated the highest total sales?


```python
# write your solution here

My solution:

df["total"] = df["quantity"] * df["price"]

df.groupby("product")["total"].sum().sort_values(ascending=False)
