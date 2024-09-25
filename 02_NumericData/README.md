
# Integers and Floats - Working with Numeric Data

## Introduction

In Python, numbers are represented by two main types: integers and floats. Integers (`int`) are whole numbers, and floats (`float`) are numbers with decimal points. Understanding how to work with these data types is fundamental in Python.

### Integers vs. Floats

An integer is a whole number, whereas a float is a decimal number.

Example of creating an integer and checking its type:

```python
num = 3
print(type(num))  # Output: <class 'int'>
```

If you assign a decimal value, the type becomes float:

```python
num = 3.14
print(type(num))  # Output: <class 'float'>
```

The output shows how the data type changes from `int` to `float` when you assign a decimal.

---

## 1. Arithmetic Operators

Python supports standard arithmetic operations, such as addition, subtraction, multiplication, and division.

### Addition

We are all familiar with addition. For example:

```python
print(3 + 2)  # Output: 5
```

### Subtraction

```python
print(3 - 2)  # Output: 1
```

### Multiplication

```python
print(3 * 2)  # Output: 6
```

### Division

Division returns a float:

```python
print(3 / 2)  # Output: 1.5
```

### Floor Division

Floor division discards the decimal part:

```python
print(3 // 2)  # Output: 1
```

### Exponentiation

Use `**` for powers:

```python
print(3 ** 2)  # Output: 9
```

### Modulus

The modulus operator returns the remainder of division:

```python
print(3 % 2)  # Output: 1
```

#### Common Use of Modulus

The modulus operator can be used to determine if a number is even or odd:

```python
print(4 % 2)  # Output: 0  # Even
print(5 % 2)  # Output: 1  # Odd
```

---

## 2. Order of Operations

Python respects the order of operations (PEMDAS). Parentheses can be used to change the default order:

```python
print(3 * (2 + 1))  # Output: 9
```

Without parentheses:

```python
print(3 * 2 + 1)  # Output: 7
```

---

## 3. Incrementing a Variable

### Standard Incrementing

One way to increment a variable is as follows:

```python
num = 1
num = num + 1
print(num)  # Output: 2
```

### Shorthand Increment

You can also use the shorthand operator `+=`:

```python
num = 1
num += 1
print(num)  # Output: 2
```

This shorthand applies to other operations, such as multiplication:

```python
num *= 10
print(num)  # Output: 10
```

---

## 4. Built-in Functions for Working with Numbers

### abs()

The `abs()` function returns the absolute value:

```python
print(abs(-3))  # Output: 3
```

### round()

The `round()` function rounds a number to the nearest integer:

```python
print(round(3.75))  # Output: 4
```

You can also specify the number of decimal places:

```python
print(round(3.75, 1))  # Output: 3.8
```

---

## 5. Comparisons and Casting

### Comparison Operators

Comparison operators in Python return boolean values (`True` or `False`):

```python
# Comparisons:
# Equal:                3 == 2
# Not Equal:            3 != 2
# Greater Than:         3 > 2
# Less Than:            3 < 2
# Greater or Equal:     3 >= 2
# Less or Equal:        3 <= 2

print(3 == 2)  # Output: False
print(3 != 2)  # Output: True
print(3 > 2)   # Output: True
print(3 < 2)   # Output: False
```

### Casting

If you have numbers stored as strings, you can cast them to integers using the `int()` function:

```python
num_1 = '100'
num_2 = '200'
num_1 = int(num_1)
num_2 = int(num_2)
print(num_1 + num_2)  # Output: 300
```

In this example, casting converts the string representations of numbers into integers.

