# Business Analysis

## Exercise 1

For each category, find the total units sold, average order sales value, and number of orders.


```python
# write your solution here

My solution:

df["total"] = df["quantity"] * df["price"]

df.groupby("category").agg({"quantity": "sum", "total": "mean", "order_id": "count"})