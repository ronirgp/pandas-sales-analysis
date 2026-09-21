# Find the top product

We can combine `groupby()` and `sum()` to compare totals between groups.

Example:

```python
df.groupby("product")["quantity"].sum().sort_values(ascending=False)


**Exercise:** Find the product with the highest total quantity sold.

Exercise 1

Find the product with the highest total quantity sold.

# My solution
df.groupby("product")["quantity"].sum().sort_values(ascending=False)