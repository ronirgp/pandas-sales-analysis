# groupby

`groupby()` groups rows based on a column.

Example:

```python
df.groupby("category")["quantity"].sum()

### Your task

> **Find the total quantity sold for each region.**

Write the code yourself and send it to me.
# My solution
df.groupby("region")["quantity"].sum()

