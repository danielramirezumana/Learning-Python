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

* <h3 style="color:#33FFA2">Reversing a string</h3>

| D    | a    | n    | i    | e    | l    |
| ---- | ---- | ---- | ---- | ---- | ---- |
| 0    | -1   | -2   | -3   | -4   | -5   |

```python
var1 = "Daniel"
print(var1[::-1])

# From 4 to 1 (the loop ends in 2) by iterating one position in the negative
print(var1[4:1:-1])
```

```
>> leinaD
>> ein
```

<h2 style="color:#33ECFF">Working with strings</h2>

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



* <h3 style="color:#33FFA2">Replace</h3>



* <h3 style="color:#33FFA2">In  |  Not in</h3>




<h2 style="color:#33ECFF">Conditionals and Loops</h2>