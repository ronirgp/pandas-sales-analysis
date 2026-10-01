# Business Analysis

## Exercise 1

Which region has the highest average order sales value, and what is the total number of units sold in that region?

```python
# write your solution here

My solution:

df["total"] = df["price"] * df["quantity"]
df.groupby("region").agg({"total": "mean", "quantity": "sum"})