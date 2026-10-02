# Business Analysis

## Exercise 1

For each product, find the number of orders, total revenue, and average order sales value.

```python
# write your solution here

My solution:

df["total"] = df["quantity"] * df["price"]
df.groupby("product").agg({"order_id": "count", "total": ["sum", "mean"]})