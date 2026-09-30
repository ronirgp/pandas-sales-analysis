# Business Analysis

## Exercise 1

Which category has the highest total revenue, and how many units were sold in that category?


```python
# write your solution here

My solution:

df["total"] = df["quantity"] * df["price"]
df.groupby("category").agg({"total": "sum", "quantity": "sum"}).sort_values("total", ascending=False)