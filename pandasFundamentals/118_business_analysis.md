# Business Analysis

## Exercise 1

Which customer bought the most units, and what was the average price they paid?


```python
# write your solution here

My solution:

df.groupby("customer").agg({"quantity": "sum", "price": "mean"

})