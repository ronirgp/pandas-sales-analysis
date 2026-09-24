# Filter, group, and multiple statistics

## Exercise 1

Using only rows where `quantity` is greater than 1, find the minimum, maximum, and average `price` for each `category`

```python
# write your solution here

My solution:
df[df["quantity"] > 1].groupby("category")["price"].agg(["min", "max", "mean"])

