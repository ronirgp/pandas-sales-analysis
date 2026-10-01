# Business Analysis

## Exercise 1

For each region, find the average order sales value, total units sold, and number of orders.

```python
# write your solution here

My solution:

df["total"] = df["quantity"] * df["price"]
df.groupby("region").agg({"total": "mean", "quantity": "sum", "order_id": "count" })