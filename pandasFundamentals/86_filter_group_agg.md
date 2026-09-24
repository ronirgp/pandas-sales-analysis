# Filter, group, and multiple statistics

## Exercise 1

Using only rows where `price` is less than 300, find the minimum, maximum, and average `quantity` for each `region`.

```python
# write your solution here
My solution:

df[df["price"] < 300 ].groupby("region")["quantity"].agg(["min", "max", "mean"])