# Concepts

## try/except
Some code can produce errors that will cause the program to fail unless you do something about them. Take for example parsing an integer:

```python
int("5") # This works because 5 is a number
int("Hello") # This will produce an error, because the input "hello" is a string and not a number
```

We can use the try/except keywords to handle these errors.  In the example below, we will get the users input as a string and parse it to an integer.  If the user inputs anything other than a number, the program will tell them that there was an error and prompt them for input again.

```python
parsed_input = None
while parsed_input == None:
  x = input("Enter a number: ")
  try:
    parsed_input = int(x)
  except:
    print('Error: Please enter a number...')

print(x)
```

## clearing the screen
To clear the screen of any prior printed text you can do the following

```python
import os
clear = lambda: os.system('clear')

print("this text will be erased by the next line and we won't see it...")
clear()
print("this text will be seen, because it's after the clear")
```

## loops
```python
while BOOLEAN_VALUE:
    print('inside loop')
```

# Project: Tic Tac Toe
Create a Tic Tac Toe game where the user inputs a number from 1-9 to take a space on the game board.  The game board should be setup as follows:

```text
 1 | 2 | 3 
----------- 
 4 | 5 | 6
-----------
 7 | 8 | 9
```

Requirements
1. When the game starts, the AI or Human should be randomly selected to go first.
2. Use a while loop to get the player's move and make the AI move.
3. When the game has ended, display text that states the outcome.
4. After each move the screen should be cleared so we only see the current board.