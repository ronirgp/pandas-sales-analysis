# Filter, group, and multiple statistics

## Exercise 1

Using only rows where `price` is less than 100, find the minimum, maximum, and average `quantity` for each `region`.

# write your solution here

My solution:

# write your solution here

# My solution:
df[df["price"] < 100 ].groupby("region")["quantity"].agg(["min", "max", "mean"])