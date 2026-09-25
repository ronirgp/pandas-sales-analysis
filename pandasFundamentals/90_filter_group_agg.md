# Filter, group, and multiple statistics

## Exercise 1

Using only rows where `price` is greater than 100, find the minimum, maximum, and average `quantity` for each `region`.

```python
# write your solution here

My solution:

df[df["price"] > 100 ].groupby("region")["quantity"].agg(["min", "max", "mean"])