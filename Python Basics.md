<h1 style="color:#3389FF">Python Basics</h1>

<h2 style="color:#33ECFF">Python Basics</h2>

<h3 style="color:#33FFA2">Python Basics</h3>

<h4 style="color:#33FF54">Python Basics</h4>

***

<h2 style="color:#33ECFF">Outputs</h2>

Use `print()` to get an output.

```python
print("Hello word")
```

``` 
>> Hello world
```

<h2 style="color:#33ECFF">Variables</h2>

* <h3 style="color:#33FFA2">Assigment</h3>

```python
var1 = 3.14
var2 = "Hello worl"
var3 = 'a'
var4 = '5'
var5 = 8.0/2

print(var1)
print(var2)
print(var3)
print(var4)
print(var5)
```

```
>>  3.14
>> Hello world
>> a
>> 5
>> 4.0
```

* <h3 style="color:#33FFA2">Multiple Variable Assigment</h3>

```python
var1 = var2 = var3 = 5

var4, var5, var6 = 2, 'Four', False

print(var1, " is type: ", type(var1))
print(var2, " is type: ", type(var2))
print(var3, " is type: ", type(var3))
print(var4, " is type: ", type(var4))
print(var5, " is type: ", type(var5))
print(var6, " is type: ", type(var6))
```

```
>> 5 is type: <class 'int'>
>> 5 is type: <class 'int'>
>> 5 is type: <class 'int'>
>> 2 is type: <class 'int'>
>> Four is type: <class 'str'>
>> False is type: <class 'bool'>
```

<h2 style="color:#33ECFF">Inputs</h2>

You can make an input by using `varName = input()`.

```python
print('Please enter your fullname:\n')
fullname = input()
print('Welcome to this repository, ' + fullname)
```

```
>> Please enter your fullname:
<< Daniel Ramírez
>> Welcome to this repository, Daniel Ramírez
```

<h2 style="color:#33ECFF">Data Type</h2>

Use `type()` to know the type of a variable.

```python
var1 = 5
var2 = '8'
var3 = 3.5

print("The type of var1 is:   ", type(var1))
print("The type of var2 is:   ", type(var2))
print("The type of var3 is:   ", type(var3))
```

```
>> The type of var1 is:    <class 'int'>
>> The type of var2 is:    <class 'str'>
>> The type of var3 is:    <class 'float'>
```

* <h3 style="color:#33FFA2">Define or Change a type</h3>

To change the type of a variable use `int()`, `str()`, or `float()`, depending on the type of data you need to change to.

```python
var1 = '7'
print("var1 is of type:", type(var1), ", \nand the value is:", var1, "\n")

var2 = int(var1)
print("var2 is of type:", type(var2), ", \nand the value is:", var2, "\n")

print("How old are you?")
var3 = input()
print("\nvar3 is of type: ", type(var3), ", \nand the value is:", var3)
print("but using int(), \nnow the type is ", type(int(var2)))
```

```
>> var1 is of type: <class 'str'> , 
>> and the value is: 7 

>> var2 is of type: <class 'int'> , 
>> and the value is: 7 

>> How old are you?
<< 27

>> var3 is of type:  <class 'str'> , 
>> and the value is: 27
>> but using int(), 
>> now the type is  <class 'int'>
```

* <h3 style="color:#33FFA2">From ASCII to Character and vice versa</h3>

Use `chr()` to get the character of an ASCII value, and use `ord()` to get the ASCII of a character.

```python
# From ASCII to Char
var1 = chr(76)
var2 = chr(83)
 
print(var1)
print(var2)

# From Char to ASCII
var3 = ord('a')
var4 = ord('A')

print(var3)
print(var4)
```

```
>> L
>> S
>> 97
>> 65
```

<h2 style="color:#33ECFF">Operators</h2>

* <h3 style="color:#33FFA2">Arithmetic Operators</h3>

| Operator | Name           | e.g.   |
| -------- | -------------- | ------ |
| +        | addition       | x + y  |
| -        | subtraction    | x - y  |
| *        | multiplication | x * y  |
| /        | division       | x / y  |
| %        | modulus        | x % y  |
| **       | exponentiation | x ** y |
| //       | floor division | x // y |

```python
print("5 + 2 is:  ", 5 + 2)
print("2 - 5 is:  ", 2 - 5)
print("5 * 5 is:  ", 5 * 5)
print("7 / 2 is:  ", 7 / 2)
print("19 % 4 is: ", 19 % 4)
print("2 ** 3 is: ", 2 ** 3)
print("36 // 3 is:", 36 // 3)
```

```
>> 5 + 2 is:   7
>> 2 - 5 is:   -3
>> 5 * 5 is:   25
>> 7 / 2 is:   3.5
>> 19 % 4 is:  3
>> 2 ** 3 is:  8
>> 36 // 3 is: 12
```

<h3 style="color:#33FFA2">Binary Operators</h3>

| Operator | Name | case 1               | case 2               | case 3               | case 4               | e.g.                | e.g.         |
| -------- | ---- | -------------------- | -------------------- | -------------------- | -------------------- | ------------------- | ------------ |
| \|       | or   | 1 \| 1 = 1           | 1 \| 0 = 1           | 0 \| 1 = 1           | 0 \| 0 = 0           | 1000 \| 1010 = 1010 | 8 \| 10 = 10 |
| &        | and  | 1 & 1 = 1            | 1 & 0 = 0            | 0 & 1 = 0            | 0 & 0 = 0            | 1000 \| 1010 = 1000 | 8 & 10 = 8   |
| ^        | xor  | 1 ^ 1 = 0            | 1 ^ 0 = 1            | 0 ^ 1 = 1            | 0 ^ 0 = 0            | 1000 \| 1010 = 0010 | 8 ^ 10 = 2   |
| ~        | not  | ~00000000 = 11111111 | ~11111111 = 00000000 | ~00000001 = 11111110 | ~11110000 = 00001111 | ~1001 = 1111 0110   | ~9 = -10     |

```python
# or
print(8|10)

# and
print(8&10)

# xor
print(8^10)

# xor
print(~1)
print(~0)
print(~9)
```

```
>> 10
>> 8
>> 2
>> -2
>> -1
>> -10
```

* <h3 style="color:#33FFA2">Assignment Operators</h3>

| Operator | e.g.    | equivalent |
| -------- | ------- | ---------- |
| =        | x = y   | x = x      |
| +=       | x += y  | x = x + y  |
| -=       | x -= y  | x = x - y  |
| *=       | x += y  | x = x * y  |
| /=       | x /= y  | x = x / y  |
| %=       | x %= y  | x = x % y  |
| **=      | x **= y | x = x ** y |
| //=      | x //= y | x = x // y |
| \|=      | x \|= y | x = x \| y |
| &=       | x &= y  | x = x & y  |
| ^⁼       | x ^= y  | x = x ^ y  |

```python
n_sum = n_exp = n_and = 5

# -=
print(n_sum)
n_sum += 3
print(n_sum)

# **=
print(n_exp)
n_exp **= 3
print(n_exp)

# &=
print(n_and)
n_and &= 3
print(n_and)
```

```
>> 5
>> 8
>> 5
>> 125
>> 5
>> 1
```

* <h3 style="color:#33FFA2">Logical Operators</h3>

| Operator | case 1               | case 2                 | case 3                 | case 4                  |
| -------- | -------------------- | ---------------------- | ---------------------- | ----------------------- |
| or       | True or True = True  | True or False = True   | False or True = True   | False or False = False  |
| and      | True and True = True | True and False = False | False and True = False | False and False = False |
| not      | not True = False     | not False = True       |                        |                         |

```python
print(5 != 4 or 5 < 1)
print("Ric" in "Costa Rica" and "pura vida" == "pura vida")
print(5 != 4 and 5 < 1)
print(not "Ric" in "Costa Rica")
```

```
>> True
>> True
>> False
>> False
```

* <h3 style="color:#33FFA2">Comparison Operators</h3>

When we use comparison, the result is a boolean (`True` if the statement happens, `False` if not) .

| Operator | Name                     | Example |
| -------- | ------------------------ | ------- |
| ==       | equal to                 | x == y  |
| !=       | not equal to             | x != y  |
| >        | greater than             | x > y   |
| >=       | greater than or equal to | x >= y  |
| <        | less than                | x < y   |
| <=       | less than or less to     | x <= y  |

```python
score_1 = 57
score_2 = 57
score_3 = 42
print(score_1 == score_2)
print(score_1 == score_3)
print(score_1 != score_2)
print(score_1 != score_3)
print(score_1 > score_2)
print(score_1 >= score_3)
print(score_1 < score_2)
print(score_1 <= score_3)
```

```
>> True
>> False
>> False
>> True
>> False
>> True
>> False
>> False
```

* <h3 style="color:#33FFA2">Membership & Identity Operators</h3>

Both of them return a boolean value (`True` or `False`).

| Type       | Operator | How it works                                                 |
| ---------- | -------- | ------------------------------------------------------------ |
| Membership | in       | check if the sequence is contained within an element         |
| Membership | not in   | check if the value is not contained within an element        |
| Identity   | is       | check if the element is exactly the same as the other element |
| Identity   | not is   | check if the element is not exactly the same as the other element |

```python
fruit = "pineapple"
colors = ["red", "green", "blue"]

print("apple" in "pineapple")
print("apple" not in "pineapple")
print("banana" in "pineapple")

print("red" in colors)
print("bl" in colors)

print(5 == "5")
print(5 is "5")
print(5 is not "5")

```

```
>> True
>> False
>> False
>> True
>> False
>> False
>> False
>> True
```

<h2 style="color:#33ECFF">String and Slicing</h2>

A string is a data structure that stores a sequence of characters.

```python
var1 = "Python"

print(var1)
print(var1[0])
print(var1[1])

# The last char in a string is on the position len() - 1
print(len(var1))
lastPos = len(var1) -1
print(var1[lastPos])

print(var1[2:4])
print(var1[0:2])

#From 0 to 5 each 2 steps
print(var1[0:5:2])
print(var1[:2], var1[2:], var1[0:5:2])
```

```
>> Python
>> P
>> y
>> 6
>> n
>> th
>> Py
>> Pto
>> Py thon Pto
```

### Let's see some string slicing examples

```python
#Note that the loop ends one position before expected
var1 = "Daniel Ramírez Umaña"
print(var1[1:5])
print(var1[0:6])

#Multiple slicing:
print(var1[0:3], var1[7:10], var1[15:18])

#From 0 to 12 each 2 steps
print(var1[0:13:2])

#From 0 to 12 each 3 steps
print(var1[0:13:3])
```

```
>> anie
>> Daniel
>> Dan Ram Uma
>> Dne aíe
>> Di me
```

* <h3 style="color:#33FFA2">Reversing a string  (or other data structures)</h3>

| D    | a    | n    | i    | e    | l    |
| ---- | ---- | ---- | ---- | ---- | ---- |
| 0    | 1    | 2    | 3    | 4    | 5    |
| -6   | -5   | -4   | -3   | -2   | -1   |

```python
var1 = "Daniel"
print(var1[::-1])

# From 4 to 1 (the loop ends in 2) by iterating one position in the negative
print(var1[4:1:-1])

# var1[5] es igual a var1[-1]
print(var1[-1], "is iqual to", var1[5])
# var1[4] es igual a var1[-2]
print(var1[-2], "is iqual to", var1[4])

# So now we have another way to reverse a string
print(var1[-1:-7:-1])
```

```
>> leinaD
>> ein
>> l is iqual to l
>> e is iqual to e
>> leinaD
```

<h2 style="color:#33ECFF">Working with strings (or other data structures)</h2>

* <h3 style="color:#33FFA2">Remove blanks</h3>

You can remove blanks at the beginning and at the end by using `strip()`

```python
word1 = "        Hi, how are you? "

print(word1)

print(word1.strip())
```

```
>>         Hi, how are you? 
>> Hi, how are you?
```

* <h3 style="color:#33FFA2">Capitalizing</h3>

If you want to capitalize the first letter of a string, you should use `.capitalize()`

```python
fruit = "apple"
print(fruit.capitalize())

text = "the apple"
print(text.capitalize())
```

```
>> Apple
>> The apple
```

* <h3 style="color:#33FFA2">To lowercase</h3>

If you want to change to lowercase a string, you should use `.lower()`

```python
myName = "Daniel Ramírez Umaña"
print(myName.lower())
```

```
>> daniel ramírez umaña
```

* <h3 style="color:#33FFA2">To uppercase</h3>

If you want to change to uppercase a string, you should use `.upper()`

```python
myName = "Daniel Ramírez Umaña"

print(myName.upper())
```

```
>> DANIEL RAMÍREZ UMAÑA
```

* <h3 style="color:#33FFA2">Split</h3>

Splits the string every time it encounters a separator character

```python
myName = "Daniel Ramírez Umaña"
# Now myName is a list with 3 elements

splited = myName.split("e")
print(splited)

splited = myName.split(" ")
print(splited)

splited = myName.split("a")
print(splited)
```

```
>> ['Dani', 'l Ramír', 'z Umaña']
>> ['Daniel', 'Ramírez', 'Umaña']
>> ['D', 'niel R', 'mírez Um', 'ñ', '']
```

* <h3 style="color:#33FFA2">Replacing a value</h3>

By using `replace()` you van replace all letters equal to the one indicated by another specified one.

```python
myName = "Daniel Ramírez Umaña"

replaced_1 = myName.replace('e','3')
print(replaced_1)

# You can also replace more than one character at a time
replaced_1 = myName.replace('el','2')
print(replaced_1)

replaced_1 = myName.replace('a','_AA_')
print(replaced_1)
```

```
>> Dani3l Ramír3z Umaña
>> Dani2 Ramírez Umaña
>> D_AA_niel R_AA_mírez Um_AA_ñ_AA_
```

* <h3 style="color:#33FFA2">Is / is not contained</h3>

On the one hand you can check whether or not a value is contained in a string by using a `in` statement, on the other hand, using an `is not` statement you can get the opposite answer

```python
myName = "Daniel Ramírez Umaña"

print("Uma" in myName)
print("Umma" in myName)
print("Uma" not in myName)
print("Umma" not in myName)
```

```
>> True
>> False
>> False
>> True
```


<h2 style="color:#33ECFF">Conditionals and Loops</h2>

### `if` condition :

​    action

### `elif` condition :

​    action

### `else` :

​    action

The following code compares two values and indicates if the first of them is less than, greater than or equal to the second one.

```python
isLess = False
var1 = 5
var2 = 5

if var1 < var2 :
  print("less")
elif var1 > var2 :
  print("greater")
else:
  print("equal")
```

```
>> equal
```

Now we have a code that indicates if a grade entered is one of an allowed value or not and if it is allowed, if yes, it indicates if the student has passed, failed or should go to extension

```python
# An integer or float format is required to be entered
print('What grade did you get?:')
grade = input()

if float(grade) < 0 or float(grade) > 10:
  print("It is not a valid grade")
else:
  if float(grade) >= 7:
    print("Congratulations, you passed the course")
  elif float(grade) >= 6 and float(grade) < 7:
    print("well, you can still pass the course \ n give your best effort")
  else:
    print("Sorry you failed the course")

  if not float(grade) < 7:
    print("Now you can enroll the next course")
```

```
>> What grade did you get?:
<< 12
>> It is not a valid grade

>> What grade did you get?:
<< -5
>> It is not a valid grade

>> What grade did you get?:
<< 8.7
>> Congratulations, you passed the course
>> Now you can enroll the next course

>> What grade did you get?:
<< 6.5
>> well, you can still pass the course 
   give your best effort

>> What grade did you get?:
<< 5.3
>> Sorry you failed the course
```

* <h3 style="color:#33FFA2">Ternary Operator</h3>

With an ternary operator you can check whether if a statement happens or not by writing it in a single line. You can use it if there are only two possibilities.

```  python
# Example 01
is_nice = False
state1 = "nice" if is_nice else "not nice"
print(state1)

# Example 02
theGrade = 9.5
state2 = "approved" if theGrade >= 6.75 else "failed"
print(state2)

# Example 03
condition = True
print("ally" if condition else "enemy")
```

```
>> not nice
>> approved
>> ally
```

### `for`

* <h3 style="color:#33FFA2">Looping through a list</h3>





* <h3 style="color:#33FFA2">Looping through a string</h3>



# This is the end of this tutorial

## I very thank you!