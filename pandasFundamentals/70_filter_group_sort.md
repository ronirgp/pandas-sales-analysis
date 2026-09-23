# Filter, group, and sort

We can combine filtering, grouping, calculation, and sorting.

Example:

```python
df[df["quantity"] > 2].groupby("region")["price"].mean().sort_values(ascending=False)

Using only rows where price is greater than 100, find the total quantity for each category, sorted from highest to lowest.


# write your solution here

Your turn: **filter → group → sum → sort.**

My solution:

df[df["price"] > 100].groupby("category")["quantity"].sum().sort_values(ascending=False)