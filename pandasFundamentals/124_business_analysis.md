# Business Analysis

## Exercise 1

Which product has the highest total revenue, and what is its total number of units sold?

```python
# write your solution here


My solution:

df["total"] = df["quantity"] * df["price"]

df.groupby("product").agg({
    "total": "sum",
    "quantity": "sum"
}).sort_values("total", ascending=False)