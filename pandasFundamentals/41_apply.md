# Apply a function

`apply()` applies a function to each value in a column.

Example:

```python
df["price"].apply(lambda x: x * 2)


**Exercise:** Use `.apply()` to multiply every value in `quantity` by 2.

# My solution
df["quantity"].apply()(lambda x: * 2)