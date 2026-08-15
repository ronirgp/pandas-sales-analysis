\# Exercise 2.3.2 — Filter South Region



\## Business Question



Show me all orders from the South region.



\## Solution



The column we need is `region`.



The condition is `== "South"`.



```python

df\[df\["region"] == "South"]

