# Group by multiple columns and calculate average

We can group by multiple columns and calculate an average.

Example:

```python
df.groupby(["category", "region"])["price"].mean()

Find the average price for each category and region.


# write your solution here

Your turn: **group by `category` and `region`, then find the average price.**

My solution:
df.groupby(["category", "region"])["price"].mean()