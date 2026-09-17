# groupby multiple aggregations

We can calculate more than one value for each group.

Example:

```python
df.groupby("category")["quantity"].agg(["sum", "mean"])


### Your task

> **Find the total and average quantity for each region.**

Write the code yourself and send it to me. 
#  My solution
df.groupby("region")["quantity"].agg(["sum", "mean"])