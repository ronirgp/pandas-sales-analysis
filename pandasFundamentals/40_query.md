# Query rows

`query()` filters rows using a condition written as a string.

Example:

```python
df.query("price > 100")


**Exercise:** Use `query()` to find rows where `quantity > 3`.

# My solution
df.query("quantity > 3")