# Filter and calculate

We can combine operations to answer business questions.

Example:

```python
df[df["region"] == "North"]["quantity"].sum()


**Exercise:** Filter `Electronics` and calculate the total `price`.

# My solution
df[df["category"] == "electronics"] ["price"].sum()