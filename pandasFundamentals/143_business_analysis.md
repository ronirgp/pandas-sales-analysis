# Business Analysis

## Exercise 1

For each region, find the total units sold, total revenue, and number of orders.

```python
# write your solution here

My solution:

df["total"] = df["quantity"] * df["price"]

df.groupby("region").agg({"quantity": "sum", "total": "sum", "order_id": "count"})