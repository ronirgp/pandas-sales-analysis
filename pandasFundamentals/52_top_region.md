# Find the top region

We can use `groupby()`, `sum()`, and `sort_values()` together to compare totals.

## Exercise 1

Find the region with the highest total quantity sold.

My solution:

df.groupby("region")["quantity"].sum().sort_values(ascending=False)