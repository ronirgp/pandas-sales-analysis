# Filter, group, and multiple statistics

## Exercise 1

Using only rows where `price` is greater than 50, find the minimum, maximum, and average `quantity` for each `category`.

```python
# write your solution here

My solution:

df[df["price"] > 50].groupby("category")["quantity"].agg(["min", "max", "mean"])