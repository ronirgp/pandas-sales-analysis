# Filter, group, and multiple statistics

## Exercise 1

Using only rows where `price` is greater than 200, find the minimum, maximum, and average `quantity` for each `region`.

```python
# write your solution here

My solution:

df[df["price"] > 200].groupby("region")["quantity"].agg(["min", "max", "mean"])