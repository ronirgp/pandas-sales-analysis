# Business Analysis

## Exercise 1

For each category, find the number of orders, total units sold, and average price.

```python
# write your solution here

My solution:

df["total"] = df["quantity"] * df["price"]
df.groupby("category").agg({"order_id": "count", "quantity": "sum", "price": "mean"})