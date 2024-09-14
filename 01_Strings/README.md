# Strings - Working with Textual Data

## Introduction


In Python, textual data is represented by strings, and a simple print statement can display them:

```
print('Hello World')
```

**Key Methods:**
- `.lower()`
- `.upper()`
- `.count()`
- `.find()`
- `.replace()`
<br> <br>

---

## 1. Lower and Upper Case Methods

### Creating a Variable to Hold Text

You can store strings in variables to reuse them in your code:

```
message = 'Hello World'
print(message)
```

### Single vs. Double Quotes

- Use single (' ') or double quotes (" ") to define strings.
- To include a single quote in a string, either escape it with a backslash (\') or use double quotes around the string:

```
message = "Bobby's World"
print(message)
```

### Multi-line Strings

Multi-line strings can be created using triple quotes. This allows you to spread the text over multiple lines:

```
message = '''This is a multi-line
string example.'''

print(message)
```

---

## 2. String Methods

### `.lower()` and `.upper()`

These methods convert the string to lowercase or uppercase, respectively:

```
message = 'Hello World'
print(message.lower())  # Output: hello world
print(message.upper())  # Output: HELLO WORLD
```


### `.count()`

Use `.count()` to count occurrences of a specific substring in a string:

```
message = 'Hello World'
print(message.count('l')) 

# Output: 3
```


### `.find()`

The `.find()` method helps locate the first occurrence of a substring:

```
message = 'Hello World'
print(message.find('World'))

# Output: 6
```

If the substring isn't found, it returns `-1`.



### `.replace()`

The `.replace()` method allows you to replace part of a string with another substring:

```
message = 'Hello World'
message = message.replace('World', 'Universe')
print(message)  

# Output: Hello Universe
```

---

## 3. Accessing and Manipulating Strings

### String Length

The `len()` function returns the number of characters in a string:

```
message = 'Hello World'
print(len(message))

# Output: 11
```

### Accessing Individual Characters

You can access characters by their index using square brackets `([])`, starting at index 0:

```
message = 'Hello World'
print(message[0])

# Output: H
```


### Slicing Strings

Slicing allows you to extract a substring by specifying a range of indices.

```
message = 'Hello World'
print(message[0:5])

# Output: Hello
```

---

## 4. String Concatenation and Formatting

### String Concatenation

Strings can be concatenated using the `+` operator:

```
greeting = 'Hello'
name = 'Micheal'
message = greeting + ', ' + name
print(message)

# Output: Hello, Micheal
```

### String Formatting with `.format()`

You can use `.format()` to provide placeholders for string formatting:

```
message = '{}, {}. Welcome!'.format(greeting, name)
print(message)

# Output: Hello, Micheal. Welcome!
```

### F-strings

F-strings (Python 3.6+) offer a cleaner way to format strings by embedding expressions inside curly braces:

```
message = f'{greeting}, {name}. Welcome!'
print(message)

# Output: Hello, Micheal. Welcome!
```

---