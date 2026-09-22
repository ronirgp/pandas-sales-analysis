# Group and calculate different statistics

We can calculate different statistics for different columns.

Example:

```python
df.groupby("region").agg({
    "quantity": "sum",
    "price": "mean"
})

For each category, find:

total quantity
average price

# write your solution here

Your turn: **group by `category` and calculate total quantity + average price.**

My solution:
df.groupby("category").agg({"quantity": "sum", "price": "mean"})