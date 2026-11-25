# Variables and Data Types

A variable is a name that stores a value, so the computer can remember it and use it later.

- A computer needs to remember things while a program runs, like your name, your age, or a score in a game. Variables are how it does that.

### Real-Life Example

## The Labeled Box 📦
- Imagine you have a box with a label on it:
    1. The **label** says `sugar`
    2. Inside the box, there is sugar

- The label is the <b>variable name</b> and the thing inside the box is the <b>value</b>. Whenever you need the sugar, you just ask for the box named `sugar`. Variables work the same way.
- You can also take the sugar out and put something else in the box. In the same way, a variable's value can be changed later.

## What are Variables?

- A variable is a container with a name that stores a value.
- The name helps us find the value again whenever we need it.
- The value can be a number, some text, and more.

## Creating Variables

- To create a variable, write the name, then `=`, then the value.

```python
name = "Sam"
age = 20
```

- Here, `name` stores `"Sam"` and `age` stores `20`.
- The `=` sign does not mean "equals" like in maths. It means <b>"store the value on the right into the name on the left"</b>.
- You don't need any special word to create a variable in Python. Just write the name and give it a value.

### Using a Variable

- We can show the value of a variable using `print()`.

```python
name = "Sam"
print(name)
```

Output:
```
Sam
```

### Changing a Variable

- We can put a new value in the same variable. The old value is replaced.

```python
age = 20
age = 21
print(age)
```

Output:
```
21
```

## Rules for Naming Variables

- Use only letters, digits, and underscore `_`.
- A name must start with a letter or an underscore. It can never start with a digit.
- No spaces allowed. Use an underscore instead, like `my_age`.
- No special characters like `@`, `$`, `-`, `!`.
- You can't use Python's special words (keywords) like `if`, `for`, `while`, `True`.
- Names are <b>case-sensitive</b>, so `age`, `Age`, and `AGE` are three different variables.

| Name | Valid? | Why |
|------|--------|-----|
| `name` | ✅ Yes | Only letters |
| `my_age` | ✅ Yes | Underscore is allowed |
| `age2` | ✅ Yes | Digit is fine, but not at the start |
| `2age` | ❌ No | Starts with a digit |
| `my age` | ❌ No | Has a space |
| `my-age` | ❌ No | `-` is not allowed |
| `for` | ❌ No | It's a Python keyword |

### Tip for Good Names

- Choose names that explain what is stored. `age` is better than `x`.
- For names with more than one word, join them with an underscore: `student_name`, `total_marks`.

## What are Data Types?

- A data type tells Python <b>what kind of value</b> is stored in a variable.
- Think of the contact details in your phone:
    1. Name → text
    2. Age → whole number
    3. Height → decimal number
    4. Is a student? → Yes or No

- Python has a data type for each of these. The four basic ones are `int`, `float`, `str`, and `bool`.

## Integers (`int`)

- Whole numbers with no decimal point.
- Can be positive, negative, or zero.

```python
age = 20
temperature = -5
score = 0
```

## Floating-Point Numbers (`float`)

- Numbers with a decimal point.

```python
height = 5.8
price = 99.99
```

- `5` is an `int`, but `5.0` is a `float`. The decimal point makes the difference.

## Strings (`str`)

- Text. Anything written inside quotes is a string.
- You can use double quotes `" "` or single quotes `' '`.

```python
name = "Sam"
city = 'Mumbai'
```

- Be careful: `"20"` in quotes is <b>text</b>, not a number. Python treats it like a word.

## Boolean (`bool`)

- Has only two possible values: `True` or `False`.
- Like a light switch, it is either ON or OFF.
- `True` and `False` must start with a capital letter.

```python
is_student = True
is_raining = False
```

## Checking Data Types using `type()`

- `type()` tells us what data type a value or variable has.

```python
print(type(20))
print(type(5.8))
print(type("Sam"))
print(type(True))
```

Output:
```
<class 'int'>
<class 'float'>
<class 'str'>
<class 'bool'>
```

- Ignore the word `class` for now. Just look at the name inside the quotes: `int`, `float`, `str`, `bool`.

- We can also check a variable:

```python
age = 20
print(type(age))
```

Output:
```
<class 'int'>
```

## Putting It All Together

```python
name = "Sam"
age = 20
height = 5.8
is_student = True

print(name)
print(age)
print(height)
print(is_student)
```

Output:
```
Sam
20
5.8
True
```

## Summary

| Data Type | What it stores | Example |
|-----------|----------------|---------|
| `int` | Whole numbers | `20`, `-5`, `0` |
| `float` | Decimal numbers | `5.8`, `99.99` |
| `str` | Text | `"Sam"`, `'Mumbai'` |
| `bool` | True or False | `True`, `False` |