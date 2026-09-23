# Filter, group, and multiple statistics

We can filter the data, group it, and calculate multiple statistics.

Example:

```python
df[df["price"] > 50].groupby("region")["quantity"].agg(["sum", "mean"])

Using only rows where quantity is greater than 3, find the minimum, maximum, and average price for each region.

# write your solution here

Your turn: **filter → groupby → min + max + mean.**

My solution:

df[df["quantity"] > 3].groupby("region")["price"].agg(["min", "max", "mean"])

