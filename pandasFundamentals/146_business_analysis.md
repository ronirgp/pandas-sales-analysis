# Business Analysis

## Exercise 1

For each customer, find the number of orders, total revenue, and total units purchased.

```python
# write your solution here

My solution:

df["total"] = df["quantity"] * df["price"] 
df.groupby("customer").agg({"order_id": "count", "total": "sum", "quantity": "sum"})