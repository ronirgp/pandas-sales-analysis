# Business Analysis

## Exercise 1

For each category, find the total revenue, average order sales value, and total number of units sold.

```python
# write your solution here

My solution:

df["total"] = df["quantity"] * df["price"]
df.groupby("category").agg({"total": ["sum", "mean"], "quantity": "sum"})