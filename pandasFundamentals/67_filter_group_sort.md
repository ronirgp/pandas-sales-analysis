# Filter, group, and sort

We can combine several operations to answer a business question.

Example:

```python
df[df["price"] > 100].groupby("region")["quantity"].sum().sort_values(ascending=False)

Using only rows where quantity is greater than 2, find the total price for each category, sorted from highest to lowest.

# write your solution here

Your turn: **filter → group → sum → sort.**


My solution:


df[df["quantity"] > 2].groupby("category")["price"].sum().sort_values(ascending=False)