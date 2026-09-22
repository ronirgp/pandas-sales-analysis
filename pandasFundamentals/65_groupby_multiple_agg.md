# Group by multiple columns and statistics

We can group by multiple columns and calculate more than one statistic.

Example:

```python
df.groupby(["category", "region"])["quantity"].agg(["sum", "mean"])

Find the total and average quantity for each category and region.

# write your solution here

Your turn: **group by `category` and `region`, then find the sum and mean of `quantity`.**

My solution:


df.groupby(["category", "region"])["quantity"].agg(["sum", "mean"])