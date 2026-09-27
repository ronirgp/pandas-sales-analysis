# Business Analysis

## Exercise 1

For each product, find the total units sold and total revenue.

```python
# write your solution here


My solution:

df["total"] = df["quantity"] * df["price"]
df.groupby("product").agg({"quantity": "sum", "total": "sum" })