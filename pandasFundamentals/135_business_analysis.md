# Business Analysis

## Exercise 1

For each product, find the total revenue, number of orders, and total units sold.


```python
# write your solution here

My solution:


df["total"] = df["quantity"] * df["price"]
df.groupby("product").agg({"total": "sum", "order_id": "count", "quantity": "sum"})
 