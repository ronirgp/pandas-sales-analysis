# Business Analysis

## Exercise 1

Which product has the highest total revenue, and how many orders did that product have?

```python
# write your solution here

My solution:

df["total"] = df["quantity"] * df["price"]
df.groupby("product").agg({"total": "sum", "order_id": "count"}).sort_values("total", ascending=False)