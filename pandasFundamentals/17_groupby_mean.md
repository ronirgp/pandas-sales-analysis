# groupby mean

`groupby()` can also calculate averages.

Example:

```python
df.groupby("region")["price"].mean()


### Your task

> **Find the average price for each category.**

Write the code yourself and send it to me.

# My solution
df.groupby("category")["price"].mean()