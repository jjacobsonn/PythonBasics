# Integers and Floats - Working with Numeric Data


## 1. Introduction to Numeric Data Types

In Python, numeric data can be divided into two main types:
- **Integers**: Whole numbers without decimal points.
- **Floats**: Numbers with decimal points.

### Example

```
num = 3
print(type(num))  # Output: <class 'int'>

num = 3.14
print(type(num))  # Output: <class 'float'>
```

- The first example returns `<class 'int'>` because num is an integer.
- The second example returns `<class 'float'>` because num is now a decimal.

### Summary

- Use **integers** when you don't need decimals.
- Use **floats** when you do need decimals.

---

## 2. Arithmetic Operators

Python provides a variety of operators that allow you to perform basic arithmetic operations on numbers. These operators work on integers and floats and are essential for performing calculations in programming. Let's go over each operator in detail with examples and practical uses.

**Overview of Python's Arithmetic Operators**
| Operator   | Name          | Example      | Result       |
|------------|---------------|--------------|--------------|
| `+`        | Addition      | `3 + 2`      | `5`          |
| `-`        | Subtraction   | `3 - 2`      | `1`          |
| `*`        | Multiplication| `3 * 2`      | `6`          |
| `/`        | Division      | `3 / 2`      | `1.5`        |
| `//`       | Floor Division| `3 // 2`     | `1`          |
| `**`       | Exponentiation| `3 ** 2`     | `9`          |
| `%`        | Modulus       | `3 % 2`      | `1`          |

## 2.1 Addition (`+`)

Addition is used to add two numbers together. This is one of the most basic math operations you'll use in Python.

### Example

```
print(3 + 2)

# Output: 5
```

#### What's Happening:

- Python adds the two numbers `3` and `2` and returns `5`.

#### Key Use Case:

- **Adding values**: This is commonly used when calculating totals, such as summing up prices in a shopping cart or counting items in a list.


### 2.2 Subtraction (`-`)

Subtracts the second number from the first.

### Example
```
print(3 - 2)

# Output: 1
```



#### What's Happening:
- Python subtracts `2` from `3` and returns `1`.

#### Key Use Case:
- **Calculating differences**: Useful when determining how much something has decreased, such as when calculating the difference between two measurements or finding the balance in a bank account after a withdrawal.

### 2.3 Multiplication (`*`)

Multiplies two numbers.

```
print(3 * 2)# 

Output: 6
```

### 2.4 Division (`/`)

Divides the first number by the second. **Always returns a float**, even when dividing integers.

```
print(3 / 2)

# Output: 1.5
```

### 2.5 Floor Division (`//`)

Divides the first number by the second, but drops any decimals (**rounds down**).

```
print(3 // 2)

# Output: 1
```

### 2.6 Exponentiation (`**`)

Raises the first number to the power of the second.

```
print(3 ** 2)

# Output: 9  (3 squared)
```

### 2.7 Modulus (`%`)

The modulus operator `%` gives the remainder of the division.

**Key Use Case**
- The modulus operator is often used to check whether a number is even or odd. 
- If `num % 2 == 0`, the number is even. If `num % 2 == 1`, the number is odd.


```
print(3 % 2)

# Output: 1 (3 divided by 2 leaves a remainder of 1)
```

**Key Use Case:**

- The modulus operator is often used to **check whether a number is even or odd**. If `num % 2 == 0`, the number is even. If `num % 2 == 1`, the number is odd.

**Practical Use Case:**

- **Checking even or odd numbers:**

    ```
    print(2 % 2)
    # Output: 0 (even)

    print(3 % 2)
    # Output: 1 (odd)
    ```
## 3. Order of Operations (PEMDAS)

Python follows the standard order of operations for math expressions:

- **Parentheses**
- **Exponents**
- **Multiplication and Division**
- **Addition and Subtraction**

### Example Without Parentheses

```
print(3 * 2 + 1)

# Output: 7 (Multiplication happens first, then addition)
```

### Example with Parentheses

```
print(3 * (2 + 1))

# Output: 9 (Parentheses make addition happen first)
```

## 4. Incrementing Variables

### What Does "Incrementing" Mean?

When we **increment** a variable, we are increasing its value by a certain amount. This is a very common task in programming. For example, if you are counting items, looping through numbers, or updating a score in a game, you'll likely need to increment a variable.

In Python, there are a few ways to increment a variable, and understanding these methods is essential when working with loops, counters, or any repeated tasks.

### Key Use Case(s)
- **Counting iterations in a loop**: Imagine you are looping through a list of items. Each time the loop runs, you might want to count how many times it has run. This is where incrementing comes in handy.
- **Updating values repeatedly**: In a game, for example, you may want to update the player's score after every move. Incrementing makes it easy to adjust the value of a score variable.

## 4.1 Basic Increment

Let's start with the most straightforward way of incrementing a variable. You can increment a variable by assigning it the value of itself plus some number. This works like basic arithmetic.

For example, if we have a variable num set to `1`, and we want to increment it by `1`, we do the following:

```
num = 1  # The variable num starts at 1

num = num + 1  # We assign num to itself plus 1

print(num)

# Output: 2
```

#### What's Happening Here?

- We start with `num = 1`.
- Then, we say `num = num + 1`, which means: "Take the current value of `num` (which is `1`), add `1` to it, and then assign this new value back to `num`."
As a result, num now holds the value 2.
- As a result, `num` now holds the values `2`.

### 4.2 Using the `+=` Operator (Shorthand Way)
Although the basic method of incrementing works fine, Python provides a **shorter way** to do this using the `+=` operator.

The `+=` operator is a shorthand for adding a value to the variable itself. It does the same thing as `num = num + 1`, but in fewer keystrokes.

Let’s see the same example, but using `+=`:

```
num = 1  # The variable num starts at 1

num += 1  # Increment num by 1 using the += operator

print(num)

# Output: 2
```

### What's Happening Here?
- `num += 1` is just a shorter way of writing `num = num + 1`.
- This means: "Take the current value of `num`, add `1` to it, and then store this new value back in `num`."
The result is the same as before: `num` is now `2`.


## 4.4 Applying Incrementing to Other Operations

The `+=` operator isn't just limited to addition. Python allows you to use similar shorthand operators for other arithmetic operations like multiplication, subtraction, and division.

### Example: Multiplying a Variable
Let's see how we can use `*=` to multiply a variable by a value. This works similarly to `+=`:

```
num = 1  # The variable num starts at 1

num *= 10  # Multiply num by 10 using the *= operator

print(num)

# Output: 10
```

#### What's Happening Here?
- num `*= 10` is shorthand for `num = num * 10`.
- It means: "Multiply the current value of num by `10` and store the result back in `num`."
- After this line runs, num is `10` because `1 * 10 = 10`.

### Example: Subtracting from a Variable
You can also use the `-=` operator to subtract a value from a variable:

```
num = 10  # The variable num starts at 10

num -= 3  # Subtract 3 from num using the -= operator

print(num)

# Output: 7
```

#### What's Happening Here?
- `num -= 3` is shorthand for `num = num - 3`.
- It means: "Subtract `3` from `num` and store the result back in `num`."
- After this line runs, num is `7` because `10 - 3 = 7`.

### Summary
- **Incrementing** is when you increase a variable’s value. It's commonly used when counting, updating scores, or iterating through loops.
- The **basic way** to increment a variable is `num = num + 1`.
- You can use the `+=` shorthand to increment a variable in fewer steps: `num += 1`.
- This shorthand can be applied to other operations like multiplication (`*=`), subtraction (`-=`), and division (`/=`).

By using these operators, you can efficiently manage and update variables in your programs.

## 5. Built-in Functions for Numbers

### 5.1 `abs()` - Absolute Value
The `abs()` function returns the absolute value of a number (removes the negative sign).

**Key Use Case**:
- The absolute value is useful when calculating distances or when you want to work with non-negative values.

    ```
    print(abs(-3))
    
    # Output: 3
    ```

## 5.2 `round()` - Rounding
The `round()` function rounds a float to the nearest whole number. You can also specify the number of decimal places.

**Key Use Case**:
- Rounding is often used when limiting decimal places is necessary, such as when dealing with money or precise measurements.

    ```
    # Rounding to Nearest Whole Number
    print(round(3.75))

    # Output: 4

    # Rounded to 1 Decimal Place
    print(round(3.75, 1))

    # Output: 3.8
    ```

## 6. Comparisons

**Ky Use Case**:
- Comparisons are critical in conditional statements (e.g., `if` conditions), determining which values are equal, greater, or less than others.

Comparisons are used to check relationships between values. They return a boolean value (`True` or `False`).

### 6.1 Equal (`==`)
Checks if two values are equal.

```
num_1 = 3
num_2 = 2
print(num_1 == num_2)

# Output: False
```

### 6.2 Not Equal (`!=`)
Check if two values are not equal.

```
print(num_1 != num_2)  # Output: True
```

## 6.3 Greater Than and Less Than
Check if one value is greater or less than another.

```
print(num_1 > num_2)
# Output: True

print(num_1 < num_2)
# Output: False
```

## 7. Type Casting

**Key Use Case**:
- Type casting is useful when you receive **input as a string** and need to **perform arithmetic**. 
- For example, you may get a string input from a user or read data from a file, and you need to convert that string to an integer or float.

When working with user input or data from files, numeric values may be stored as strings. To use them in arithmetic, you'll need to convert them (or "cast" them) into integers or floats.

**Converting Strings to Integers**

```
num_1 = '100'
num_2 = '200'

# Converts the strings into type int
num_1 = int(num_1)
num_2 = int(num_2)

print(num_1 + num_2)

# Output: 300
```

**Converting Strings to Floats**

```
num_1 = '3.14'

# Assigns num_1 to type float
num_1 = float(num_1)

print(num_1)

# Output: 3.14
```

**Common Issue: Adding Numbers as Strings**
If you forget to cast, Python will treat numbers as strings and concatenate them instead of adding them:

```
num_1 = '100'
num_2 = '200'

print(num_1 + num_2)

# Output: 100200 (concatenates the strings)
```

To fix this, always remember to cast your strings to the appropriate numeric type (int or float).

## 8. Dealing with Problems
**Problem: Accidentally Working with Strings Instead of Numbers**<br>
You might sometimes have a number in the form of a string (from user input or files). Python will treat these as strings and perform string operations (like concatenation) instead of arithmetic.

**Solution: Casting** <br>
Always cast these strings into integers or floats using int() or float() to perform proper arithmetic.

```
num_1 = '100'
num_2 = '200'

# Where the casting the performed
num_1 = int(num_1)
num_2 = int(num_2)

print(num_1 + num_2)

# Output: 300
```

## Summary
- **Integers** and **Floats** are the two main numeric data types in Python.
- Use arithmetic operators like `+`, `-`, `*`, `/`, `//`, `**`, and `%` for basic math.
- **Order of operations** follows PEMDAS, but you can control the order using parentheses.
- **Incrementing** variables can be done with shorthand operators like `+=`.
- Use built-in functions like `abs()` and `round()` to manipulate numbers.
- **Comparisons** help you evaluate relationships between values, returning `True` or `False`.
- Always **cast** strings to integers or floats when performing arithmetic.

## Key Use Cases:
- **Modulus operator** for checking even or odd numbers.
- **Incrementing variables** for counting or updating values in loops.
- **Absolute value** for calculating distances or removing negative signs.
- **Rounding** for limiting decimal places in calculations.
- **Comparisons** for conditional logic and decision-making.
- **Type casting** when handling input or mixed data types.