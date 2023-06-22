# Review
## Array
Arrays are lists of values of the same type.
```python
strings = ["string0", "string1"]
numbers = [0, 1, 2, 3]
booleans = [True, False]
```

The first element of an array is always at the zero position.
```python
strings[0]  # string0
numbers[0]  # 0
booleans[0] # True
```

## Dictionaries
Like arrays, dictionarys store values, but instead of numbering up from
0, dictionaries allow us to specific the key.
```python
car = {
    "make": "Tesla",
    "model": "Model Y",
    "color": "White"
}
```

Then we can reference the values by the key names
```python
car["make"] # Telsa
car["model"] # Model y
```

# Tuples
Tuples are like arrays but instead of having all the elements of the same 
type, tuples can contain different types. The elements in tuples can be 
the same as an array (with square braces).
```python
x = (1, "hello", True)
print(x[0]) # prints 1
print(x[1]) # prints "hello"
```
# Functions
Functions are reusable bits of code that can produce (return) zero or 
more values.  Take for example a function that sums two numbers.
```python
def sum(x, y):
    return x + y

print(sum(1, 2)) # prints out 3
```

Now that same function but doesn't return anything.
```python
def sum(x, y):
    print(x + y)

sum() # prints 3
```

# Project: TicTacToe
Continue to work on the TicTacToe game.
