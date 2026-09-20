# Pivot table

`pivot_table()` summarizes data by groups.

Example:

```python
df.pivot_table(
    values="quantity",
    index="region",
    aggfunc="sum"
)


**Exercise:** Use `pivot_table()` to find the average `price` for each `category`.

# My solution
df.pivot_table( values="price",
index="category",
aggfunc="mean"

)