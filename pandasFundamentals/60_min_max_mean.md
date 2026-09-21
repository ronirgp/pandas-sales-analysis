# Multiple statistics

We can calculate several statistics from the same column.

Example:

```python
df["quantity"].agg(["min", "max", "mean"])

Find the minimum, maximum, and average price.

# write your solution here

Your turn: **find min, max, and mean for `price`.**

My solution:

df["price"].agg(["min", "max", "mean"])