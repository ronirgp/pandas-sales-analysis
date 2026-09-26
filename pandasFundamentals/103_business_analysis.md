# Business Analysis

## Exercise 1

Which region generated the highest number of orders?

```python
# write your solution here

My solution:

df.groupby("region")["order_id"].count().sort_values(ascending=False)

