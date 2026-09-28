# Business Analysis

## Exercise 1

Which product has the highest average price, and how many units were sold for that product?


```python
# write your solution here

My solution:
df.groupby("product").agg({
    "price": "mean",
    "quantity": "sum"
})
