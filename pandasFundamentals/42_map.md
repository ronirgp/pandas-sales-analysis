# Map values

`map()` replaces values in a column according to a mapping.

Example:

```python
df["region"].map({
    "North": "N",
    "South": "S"
})


**Exercise:** Use `.map()` to change `"North"` to `"N"`.

# My solution
df["region"].map({
    "North": "N"

})