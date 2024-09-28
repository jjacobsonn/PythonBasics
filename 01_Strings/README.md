# Strings - Working with Textual Data

## Introduction

Textual data in Python is represented using strings. Below is the most basic example of printing a string:


```
print('Hello World')

# Outputs: Hello World
```

**Key Methods:**
- `.lower()` and `.upper()`
- `.count()`
- `.find()`
- `.replace()`
<br> <br>

---

## 1. Creating a Variable to Hold a Text Value

In Python, variables are typically named using lowercase letters. If a variable name has multiple words, underscores (`_`) are used to separate them (e.g., `my_message`). Variable names should be descriptive to clarify the data they hold.

Example:

```
message = 'Hello World'
print(message)

# Outputs: Hello World
```

## 2. Single vs Double Quotes

Python strings can be defined using single (`'`) or double quotes (`"`). The choice depends on the content of the string. If the string contains an apostrophe, it’s better to use double quotes to avoid syntax errors.

### Example of an Error Using Single Quotes

```
message = 'Bobby's World'

# Output: SyntaxError: unterminated string literal
```

### Fix 1: Escaping the Apostrophe

```
message = 'Bobby\'s World'
print(message)

# Output: Bobby's World
```

### Fix 2: Using Double Quotes

```
message = "Bobby's World"
print(message)

# Output: Bobby's World
```

---

## 3. Multi-line Strings

To create multi-line strings, use triple quotes (''' or """). This allows the string to span multiple lines:
```
message = """Bobby's World was a good
cartoon in the 1990's"""
print(message)

# Output:
# Bobby's World was a good
# cartoon in the 1990's
```

---

## 4. String Length and Indexing

### Finding the Length of a String

Use the `len()` function to determine the number of characters in a string, including spaces:

```
message = 'Hello World'
print(len(message))

# Output: 11
```
### Accessing Individual Characters

Strings in Python are zero-indexed, meaning the first character is at index 0. Use square brackets (`[]`) to access individual characters:
```
message = 'Hello World'
print(message[0])

# Output: H
```
### Indexing Errors

If you attempt to access an index that is out of range, Python will raise an `IndexError`:
```
message = 'Hello World'
print(message[11])

# Output: IndexError: string index out of range
```
### Slicing Strings

To access a substring, use slicing (`[start:end]`). The `start` index is inclusive, while the `end` index is exclusive:
```
message = 'Hello World'
print(message[0:5])

# Output: Hello
```

You can also omit the start or end index for default values:
```
print(message[:5])  # From start to index 5
# Output: Hello

print(message[6:])  # From index 6 to the end
# Output: World
```
---

## 5. String Methods

### 1. `lower()` and `upper()` Methods
The `lower()` method converts all characters in a string to lowercase, while `upper()` converts them to uppercase:
```
message = 'Hello World'
print(message.lower())
# Output: hello world

print(message.upper())
# Output: HELLO WORLD
```

### 2. `count()` Method
The `count()` method counts how many times a substring appears within a string:
```
message = 'Hello World'
print(message.count('Hello'))
# Output: 1

print(message.count('l'))
# Output: 3
```
