# filter and groupby

We can filter rows first and then group the remaining data.

Example:

```python
df[df["category"] == "Electronics"].groupby("region")["quantity"].sum()


### Your task

> **Find the total quantity sold for each region, but only for Electronics.**

Write it yourself and send me the code.


#my solution
df[df["category"] == "Electronics"].groupby("region")["quantity"].sum()