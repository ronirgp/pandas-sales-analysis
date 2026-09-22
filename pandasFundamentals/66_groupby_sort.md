# Group, calculate, and sort

We can group data, calculate a value, and then sort the result.

Example:

```python
df.groupby("region")["quantity"].sum().sort_values(ascending=False)

Find the average price for each category, sorted from highest to lowest.

# write your solution here

Your turn: **group by `category`, calculate average `price`, and sort from highest to lowest.**

My solution:

df.groupby(["category"])["price"].mean().sort_values(ascending=False)