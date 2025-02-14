---
title: "Python Refreshers"
parent: "Home"
nav_order: 2
---

# Python Refreshers

## List Comprehension (For Beginners or Those Who Forgot)
List comprehension is a shortcut for creating lists in Python. Instead of writing a for loop to build a list step by step, you can do it all in one line.

### Let's Break It Down, Step-by-Step
The basic structure of list comprehension is:

`[do something for each item in a list]`

Let’s build one together for example:
1. What's your list? A list of words.
`words = ["hello", "world", "python"]`
2. What do you want to do to each word in the list? Make it uppercase.
`{variable}.upper()`
3. Okay so what do you want to do (in english)? For every word in my list of words make it uppercase.
```python
uppercase_words = [word.upper() for word in words]
print(uppercase_words)  # Output: ['HELLO', 'WORLD', 'PYTHON']
```

