# Business Analysis

## Exercise 1

For each region, find the average order sales value, average price, and total units sold.

```python
# write your solution here

My solution:

df["total"] = df["quantity"] * df["price"]
df.groupby("region").agg({"total": ,"mean", "price": , "mean", "quantity": "sum"})