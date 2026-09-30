# Business Analysis

## Exercise 1

For each region, find the total units sold, number of orders, and average order sales value.

```python
# write your solution here

My solution:

df["total"] = df["quantity"] * df["price"]
df.groupby("region").agg({"quantity": "sum", "order_id": "count", "total": "mean"})