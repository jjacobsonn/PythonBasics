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

### 3. `find()` Method

The `find()` method returns the index of the first occurrence of a substring. If the substring is not found, it returns `-1`:
```
message = 'Hello World'
print(message.find('World'))
# Output: 6

print(message.find('Universe'))
# Output: -1
```

### 4. `replace()` Method

The replace() method replaces a substring with another substring. It doesn’t modify the original string but returns a new string with the specified replacements.

```
message = 'Hello World'
new_message = message.replace('World', 'Universe')
print(new_message)

# Output: Hello Universe
```

To permanently replace the original string, assign the result back to the variable:

```
message = 'Hello World'
message = message.replace('World', 'Universe')
print(message)

# Output: Hello Universe
```

---

## 6. String Concatenation

You can concatenate (combine) strings using the `+` operator. Be sure to include spaces where necessary:

```
greeting = 'Hello'
name = 'Micheal'
message = greeting + ' ' + name

print(message)

# Output: Hello Micheal
```
---

## 7. Formatted Strings
For cleaner string concatenation, Python provides `formatted strings` or `f-strings` (introduced in Python 3.6+). These allow variables to be embedded directly into a string.

### Formatted String using `.format()`:
```
greeting = 'Hello'
name = 'Micheal'
message = '{}, {}. Welcome!'.format(greeting, name)
print(message)

#Output: Hello, Micheal. Welcome!
```

### Using f-strings (Python 3.6+)
F-strings are more concise and allow embedding of variables directly into curly braces:

```
greeting = 'Hello'
name = 'Micheal'
message = f'{greeting}, {name}. Welcome!'
print(message)

# Output: Hello, Micheal. Welcome!
```
You can even use expressions inside f-strings:
```
message = f'{greeting}, {name.upper()}. Welcome!'
print(message)

# Output: Hello, MICHEAL. Welcome!
```

---

## 8. String Literals
When concatenating strings, it's easy to forget to add spaces. String literals can help avoid such errors:

```
greeting = 'Hello'
name = 'Micheal'
message = greeting + ', ' + name
print(message)

# Output: Hello, Micheal
```
For more complex cases, it’s better to use formatted strings or f-strings to avoid errors and improve readability.

---