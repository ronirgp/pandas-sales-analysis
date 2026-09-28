# Business Analysis

## Exercise 1

For each region, find the total units sold, total revenue, and average price.


```python
# write your solution here

My solution:

df.groupby("region")ag({"quantity":"sum", "total": "sum",
"price": "mean"})