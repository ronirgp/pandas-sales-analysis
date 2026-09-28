# Business Analysis

## Exercise 1

For each region, find the total revenue and average order sales value.


```python
# write your solution here

My solution:

df["total"] = df["quantity"] * df["price"]

df.groupby("region").agg({
    "total": ["sum", "mean"]
})