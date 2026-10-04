# Business Analysis

## Exercise 1

Which product has the highest total revenue, and what is its average selling price?

```python
# write your solution here

My solution:

df["total"] = df["quantity"] * df["price"]
df.groupby("product").agg({"total": "sum", "price": "mean"}).sort_values("total", ascending=False)