# Create column and group

We can create a new column and then use it in a groupby analysis.

Example:

```python
df["total"] = df["quantity"] * df["price"]


**Exercise:** Create `total`, then group by `region` and calculate the sum of `total`.

# My solution
df["total"] = df["quantity"] * df["price"]
df.groupby("region")["total"].sum()