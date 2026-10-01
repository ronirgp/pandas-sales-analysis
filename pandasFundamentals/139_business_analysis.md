# Business Analysis

## Exercise 1

For each region, find the total revenue, number of orders, and average price.

```python
# write your solution here

My solution:

df["total"] = df["quantity"] * df["price"]
df.groupby("region").agg({"total": "sum", "order_id": "count", "price": "mean"})