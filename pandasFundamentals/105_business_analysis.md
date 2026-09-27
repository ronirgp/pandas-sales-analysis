# Business Analysis

## Exercise 1

Which customer generated the highest total sales?

```python
# write your solution here

My solution:

df["total"] = df["quantity"] * df["price"]

df.groupby("customer")["total"].sum().sort_values(ascending=False)