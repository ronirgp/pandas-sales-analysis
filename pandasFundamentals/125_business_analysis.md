# Business Analysis

## Exercise 1

For each customer, find the average order sales value and total number of orders.


```python
# write your solution here

My solution:

f["total"] = df["quantity"] * df["price"]
df.groupby("customer").agg({"total": "mean", "order_id": "count" })