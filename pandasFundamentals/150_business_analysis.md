# Business Analysis

## Exercise 1

For each customer, find the average order sales value, total units purchased, and number of orders.

```python
# write your solution here

My solution:

df["total"] = df["quantity"] * df["price"]
df.groupby("customer").agg({"total": "mean", "quantity": "sum", "order_id": "count" })