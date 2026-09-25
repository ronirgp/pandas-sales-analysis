# Filter, group, and multiple statistics

## Exercise 1

Using only rows where `quantity` is less than 4, find the minimum, maximum, and average `price` for each `region`.

```python
# write your solution here

My solution:

df[df["quantity"] < 4 ].groupby("region") ["price"].agg(["min", "max", "mean"])