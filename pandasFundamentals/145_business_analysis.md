# Business Analysis

## Exercise 1

For each category, find the total number of orders, average selling price, and total units sold.

```python
# write your solution here

My solution:

df["total"] = df["quantity"] * df["price"]
df.groupby("category").agg({"order_id": "count", "price": "mean", "quantity": "sum"})