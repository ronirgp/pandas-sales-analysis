# Multiple Conditions

Use `&` when we need two conditions to be true.

Example:

```python

df[(df["price"]> 50) & (df["region"] == "North")]