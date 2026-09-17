# sort and groupby

We can group data, calculate a value, and then sort the result.

Example:

```python
df.groupby("region")["quantity"].sum().sort_values(ascending=False)


### Your task

> **Find the total quantity sold for each category and sort it from highest to lowest.**

Send me your code.

# My solution
df.group("category")["quantity"].sum().sort_values(ascending=False)