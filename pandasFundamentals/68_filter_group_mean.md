# Filter, group, and calculate average

We can filter rows first, then group the remaining data and calculate an average.

Example:

```python
df[df["quantity"] > 2].groupby("region")["price"].mean()

Using only rows where price is greater than 50, find the average quantity for each region.


# write your solution here

Your turn: **filter → group → mean.**

My solution:

df[df["price"] > 50].groupby("region")["quantity"].mean()