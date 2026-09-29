# Business Analysis

## Exercise 1

For each customer, find their total revenue and total number of units purchased.


```python
# write your solution here

My solution:
 
df["total"] = df["quantity"] * df["price"]
df.groupby("customer").agg({"total": "sum", "quantity": "sum"})