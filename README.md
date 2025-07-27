# Remove Stars From a String

## Problem Description

You are given a string `s` that contains lowercase English letters and asterisks (`*`).

**In one operation**, you can:
- Choose a `*` in `s`
- Remove the **closest non-star character to its left**, and also **remove the `*` itself**

Your task is to **return the final string after performing all such operations**.

### Notes:
- The input is always valid (every `*` has a character to its left to remove).
- The result will always be **unique**.

---

## Examples

### Example 1:

**Input:**  
`s = "leet**cod*e"`

**Output:**  
`"lecoe"`

**Explanation:**
- `"leet**cod*e"`
- First `*` removes `'t'` → `"lee*cod*e"`
- Second `*` removes `'e'` → `"lecod*e"`
- Third `*` removes `'d'` → `"lecoe"`

✅ Final output: `"lecoe"`

---

### Example 2:

**Input:**  
`s = "erase*****"`

**Output:**  
`""` (empty string)

**Explanation:**
- Each `*` removes one character to the left.
- All characters are eventually removed.

---

## Constraints

- `1 <= s.length <= 10⁵`
- `s` contains only **lowercase English letters** and **asterisks (`*`)**
- The operation can **always be performed** on the input string
