# Business Analysis

## Exercise 1

For each product, find the total number of units sold and the average selling price.


```python
# write your solution here

My solution:

df["total"] = df["quantity"] * df["price"]

df.groupby("product").agg({"quantity": "sum", "price": "mean" })