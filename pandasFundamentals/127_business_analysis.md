# Business Analysis

## Exercise 1

For each product, find the total units sold, average price, and total revenue.

My solution:

```python
# write your solution here

df["total"] = df["quantity"] * df["price"]

df.groupby("product").agg({"quantity": "sum", "price": "mean", "total": "sum"})