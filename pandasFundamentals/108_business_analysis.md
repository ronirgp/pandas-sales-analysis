# Business Analysis

## Exercise 1

Which region sold the most units, and what was the average price of those units?

```python
# write your solution here

My solution:

df["total"] = df["quantity"] * df["price"]
df.groupby("region").agg({
    "quantity": "sum",
    "price": "mean"
})