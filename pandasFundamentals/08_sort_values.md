# sort_values()

Use `sort_values()` to sort the data.

Example:

```python
df.sort_values("price", ascending=False)



### 🎯 Your exercise

> **Show me all orders sorted by `quantity` from highest to lowest.**

Think:

**sort → `sort_values()`**

**quantity → column**

**highest to lowest → `ascending=False`**

Write the code yourself and send it to me.

# write solution here
df.sort_values("quantity", ascending=False)