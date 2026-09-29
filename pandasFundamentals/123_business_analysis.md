# Business Analysis

## Exercise 1

For each region, find the average price, total units sold, and total revenue.

```python
# write your solution here

My solution:

df["total"] = df["quantity"] * df["price"]
df.groupby("region").agg({"price": "mean", "quantity": "sum", "total": "sum"})