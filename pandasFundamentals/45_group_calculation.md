# Group and calculate

We can group data and then calculate a result for each group.

Example:

```python
df.groupby("region")["quantity"].sum()

**Exercise:** Find the average `quantity` for each `category`.

# My solution
df.groupby("category")["quantity"].mean()