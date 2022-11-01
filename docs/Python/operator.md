# Variable
## Comments
Each programming language has its own annotated symbol, and the annotated code or other content will not be run, and the annotated symbol in Python is #

```python
print("Hello World")
# This is a comment, the content here will not be execute
```

This method is used to comment one line, but there is also another method to comment multiple lines

```python
print("Hello World)
"""
This is a multi-line comment
Everything here will not be run
"""
```


## Create a variable
First of all, we need to understand what a variable is, a variable is like a container for storing data, when you define a variable, the computer will store the data in memory

?> The process of creating a variable is also called assign variable

So how do you define variables in Python?
```python
x = 10
y = "alfred"

print(x)
print(y)
```

?> In Python, you don't need to declare the data type of a variable first, you can directly define the variable

## Single or double quotes
```python
a = 'Shelly'
a = "Shelly"
# It is possible to use either single or double quotes when defining variables in Python
```

## Case sensitive
```python
# When creating a variable in Python, the variable names are case-distinguished
a = 'Shelly'
jA = 'alfred'
# Here a and A are not the same and will not be overwritten
```

## Rules of creating variables

?> Here are legal examples
```python
var = 10
_var = 10
my_var = 10
VAR = 10
Var = 10
var1 = 10
```

?> Here are illegal values
```python
2var = 10
my-var = 10
my var = 10
```

## Define multiple variables at the same time
This example is defining several different variables in a single line of code
```python
x, y, z = "alfred", "shelly", "jane"
print(x)
print(y)
print(z)
```

This example is multiple variables with the same but different variable names defined in a single line of code
```python
x = y = z = "alfred"
print(x)
print(y)
print(z)
```

## Print the result
```python
x = y = z = "alfred"
print(x)
print(y)
print(z)
```
Here ````print`` means to print out the content


?> This example is to print the content of x together with the content of y
```python
x = "shelly"
y = "alfred"

print(x + y)
```

Result ：
```
shellyalfred
```

!> It should be noted here that this example will report an error, because the number cannot be printed with the string at the same time
```python
x = 10
y = "alfred"

print(x + y)
```

Result ：
```
10alfred
```

?> But the content can be printed because although they are all printed in the same way, they are printed separately
```python
x = 10
y = "alfred"

print(x, y)
```

Result ：
```
10 alfred
```

## 全局变量与局部变量

在函数内外定义的变量是不一样的，一个是全局变量，一个是局部变量
?> 如果有不知道函数的什么的也不急，后面会有详细的讲解

```python
# 这个是全局变量
x = "alfred"

def func():
    # 这个是局部变量
    x = "shelly"
    print("My name is " + x)

print("My name is " + x)
```
它们出来的结果会截然不同

结果 ：
```
My name is alfred
My name is shelly
```


当然，我们也可以在函数内定义全局变量

```python
def my_func():
    # global是在函数内定义全局变量的关键字
    global x
    x = "shelly"
    
my_func()
print(x)
```