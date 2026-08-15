# OR Conditions

Use `|` when either condition can be true.

Example:

```python
df[(df["region"] == "North") | (df["region"] == "South")]

df[(df["category"] == "Electronics") | (df["category"] == "Furniture")]