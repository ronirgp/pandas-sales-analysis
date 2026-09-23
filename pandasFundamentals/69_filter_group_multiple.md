# Filter, group, and calculate multiple statistics

We can filter the data, group it, and calculate more than one statistic.

Example:

```python
df[df["price"] > 50].groupby("region")["quantity"].agg(["sum", "mean"])

Using only rows where quantity is greater than 2, find the minimum and maximum price for each category.


# write your solution here

Your turn: **filter → group → min + max.**

My solution:
df[df["quantity"] > 2].groupby("category")["price"].agg(["min", "max"])

