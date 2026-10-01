# Business Analysis

## Exercise 1

For each customer, find the total revenue, number of orders, and average order sales value.


```python
# write your solution here

My solution:

df["total"] = df["quantity"] * df["price"]

df.groupby("customer").agg({
    "total": ["sum", "mean"],
    "order_id": "count"
})