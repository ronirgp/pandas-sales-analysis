# Business Analysis

## Exercise 1

What is the average sales value of an order in each region?

```python
# write your solution here

My solution:

df["total"] = df["quantity"] * df["price"]
df.groupby("region")["total"].mean()