# Fill missing values

`fillna()` replaces missing values with another value.

Example:

```python
df["price"].fillna(0)


**Exercise:** Use `fillna()` on the `customer` column and replace missing values with `"Unknown"`.

# My solution
df["customer"].fillna("unknown")