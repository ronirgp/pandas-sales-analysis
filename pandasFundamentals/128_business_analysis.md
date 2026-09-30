# Business Analysis

## Exercise 1

For each customer, find the number of orders, average price, and total revenue.


```python
# write your solution here

My solution:

df["total"] = df["quantity"] * df["price"]

df.groupby("customer").agg({"order_id": "count", "price": "mean", "total": "sum"})