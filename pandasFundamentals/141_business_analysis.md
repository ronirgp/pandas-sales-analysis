# Business Analysis

## Exercise 1

For each customer, find the total units purchased, average price, and total revenue.

```python
# write your solution here

My solution:
df["total"] = df["quantity"] * df["price"]

df.groupby("customer").agg({
    "quantity": "sum",
    "price": "mean",
    "total": "sum"
})