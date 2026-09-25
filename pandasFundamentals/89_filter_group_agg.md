# Filter, group, and multiple statistics

## Exercise 1

Using only rows where `quantity` is less than 3, find the minimum, maximum, and average `price` for each `category`.


```python
# write your solution here
My solution:

df[df["quantity"] < 3 ].groupby("category")["price"].agg(["min", "max", "mean"])