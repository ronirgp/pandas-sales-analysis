# Business Analysis

## Exercise 1

For each category, find the total revenue and identify how many units were sold.

```python
# write your solution here

My solution:

df["total"] = df["quantity"] * df["price"]
df.groupby("category").agg({"total": "sum", "quantity": "count"})