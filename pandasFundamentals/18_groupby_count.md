# groupby count

`count()` counts the number of non-empty values in a column for each group.

Example:

```python
df.groupby("category")["product"].count()


### Your task

> **Count the number of orders for each region using `groupby()`.**

Write the code and send it to me.
# My solution
df.groupby("region")["order_id"].count()