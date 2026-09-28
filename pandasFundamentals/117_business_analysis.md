# Business Analysis

## Exercise 1

For each category, find the number of orders and the total revenue.

```python
# write your solution here


My solution:

groupby("category").agg({"order_id": "count", "total": "sum"})