# Business Analysis

## Exercise 1

Which customer has the highest total revenue, and how many orders did that customer place?


```python
# write your solution here

My solution:

df["total"] = df["quantity"] * df["price"]

df.groupby("customer").agg({"total": "sum", "order_id": "count"}).sort_values("total", ascending=False)