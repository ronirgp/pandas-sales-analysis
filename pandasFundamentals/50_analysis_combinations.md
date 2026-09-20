# Pandas combinations

The important part of Pandas is combining operations to answer questions.

Common patterns:

```python
# Filter + calculation
df[df["price"] > 100]["quantity"].sum()

# Group + calculation
df.groupby("region")["quantity"].sum()

# Group + sort
df.groupby("category")["quantity"].sum().sort_values(ascending=False)

# Filter + group + calculation
df[df["category"] == "Electronics"].groupby("region")["quantity"].sum()


**Exercise:** Combine **filter → group → sum**.
Find the total quantity sold for each region, but only for orders where price > 50.

# My solution
df[df["price"] > 50].groupby("region")["quantity"].sum()
