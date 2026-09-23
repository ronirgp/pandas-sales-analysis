# Filter, group, and multiple statistics

We can filter the data, group it, and calculate multiple statistics.

## Exercise 1

# Using only rows where `price` is greater than 100, find the minimum, maximum, and average `quantity` for each `category`.

```python
# write your solution here

My solution:
df[df["price"] > 100].grpupby("category")["quantity"].agg(["min", "max", "mean"])

