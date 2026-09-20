# Filter, group, and sort

We can combine filtering, grouping, calculation, and sorting.

Example:

```python
df[df["category"] == "Electronics"].groupby("region")["quantity"].sum().sort_values(ascending=False)


**Exercise:** Filter `price > 100` → group by `region` → sum `quantity` → sort highest to lowest.

# My solution
df[df["price"] > "100"].groupby("region")[["quantity"].sum().sort_values(ascending=False)]