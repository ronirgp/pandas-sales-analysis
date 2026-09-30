# Business Analysis

## Exercise 1

For each customer, find the total revenue, average price, and total number of units purchased.

```python
# write your solution here

My solution:

df["total"] = df["quantity"] * df["price"]
df.groupby("customer").agg({"total": "sum", "price": "mean", "quantity": "count"})