# Business Analysis

## Exercise 1

For each product, find the number of orders, total units sold, and average order sales value.

```python
# write your solution here

My solution:
df["total"] = df["quantity"] * df["price"]
df.groupby("product").agg({"order_id": "count", "quantity": "sum", "total": "mean" })