# Business Analysis

## Exercise 1

Which customer has the highest average order sales value, and what is their total revenue?

```python
# write your solution here

My solution:

df["total"] = df["quantity"] * df["price"]

df.groupby("customer").agg({
    "total": ["mean", "sum"]
})