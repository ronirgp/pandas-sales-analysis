# Group and calculate multiple statistics

We can group data and calculate several statistics at the same time.

Example:

```python
df.groupby("region")["quantity"].agg(["min", "max", "mean"])

Find the minimum, maximum, and average price for each category.

# write your solution here

Your turn: **group by `category` and find min, max, and mean price.**

My solution:

df.groupby("category")["price"].agg(["min", "max", "mean"])