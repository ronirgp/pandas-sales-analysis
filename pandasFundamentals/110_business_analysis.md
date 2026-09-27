# Business Analysis

## Exercise 1

Which customer placed the most orders, and what was their total revenue?

```python
# write your solution here

My solution:

df["total"] = df["quantity"] * df["price"]
df.groupby("customer").agg({"order_id": "count", "total": "sum"})