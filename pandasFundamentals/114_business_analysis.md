# Business Analysis

## Exercise 1

For each customer, find the number of orders, total units purchased, and total revenue.


```python
# write your solution here

My solution:

df["total"] = df["quantity"] * df["price"]

df.groupby("customer").agg({
    "order_id": "count",
    "quantity": "sum",
    "total": "sum"
})