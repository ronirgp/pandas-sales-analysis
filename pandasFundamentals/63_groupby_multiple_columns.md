# Group by multiple columns

We can group by more than one column.

Example:

```python
df.groupby(["category", "region"])["quantity"].sum()

Find the total quantity for each category and region.

# write your solution here

Your turn: **group by both `category` and `region`, then find total quantity.**

My solution:

df.groupby(["category", "region"])["quantity"].sum()