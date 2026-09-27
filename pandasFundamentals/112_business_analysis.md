# Business Analysis

## Exercise 1

Which region generated the highest total revenue, and how many orders did that region have?

```python
# write your solution here

My solution:

df["total"] = df["quantity"] * df["price"]

df.groupby("region").agg({"order_id": "count", "total": "sum"})