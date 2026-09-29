# Business Analysis

## Exercise 1

Which region has the most orders, and what is the total revenue for that region?

```python
# write your solution here

My solution:

f["total"] = df["quantity"] * df["price"]

df.groupby("region").agg({"order_id": "count", "total": "sum"})