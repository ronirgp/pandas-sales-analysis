\# isin()



Use `isin()` when we want to filter for several values in one column.



Example:



```python

df\[df\["region"].isin(\["North", "South"])]


### 🎯 Your exercise

> **Show me all orders where the category is `"Electronics"` OR `"Furniture"` using `isin()`.**

Don't use `|` this time. We're specifically practicing `isin()`.

Build the solution yourself and send me the code.


df[df["category"].isin(["Electronics", "Furniture"])]