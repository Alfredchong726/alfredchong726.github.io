# str type

?> Here again, whether you use ```""``` or ```''``` to create a variable will be the same, ```print()``` will show the result of the code

## Assign string types
The process of assign a variable is based on the variable name plus an equal sign, followed by a variable

```python
x = "alfred"
print(x)
```

## Assign a multiline string variable
When assigning values, you can assign multiple lines of variables, and you can always use three pairs of quotation marks to assign values

?> It's the same here, whether you are using ```""``` or ```''``` to will be accepted

```python
x = """My name is alfred
I am 10 years old
My hobby is swimming"""
print(x)
```

## Extraction of strings
```python
x = "Hello, world!"
print(x[4])
```

Result:
```
0
```
The reason why it turns out is this way is because x[4] represents the number that starts with H in the x variable and counts to the content of the 4th, so some people may wonder if the fourth is not l
!> Computer arithmetic always starts at 0
```python
x = "Hello, world!"
#    0123456789
```
where H is 0, e is 1, and so on

## String Slicing
As mentioned above, how computers start counting from the first letter is used in string slicing
```python
x = "Hello, world!"
print(x[0:5])
```

Result:
```
Hello
```

The idea here is to imagine adding a wall in front of the 0th and 5th letters in the x variable, and the result will be something in the middle of the two walls

```python
x = "Hello, world!"
#   |01234|5
```
So the result is Hello

In addition, there are other ways to use ```:```


In this case, a wall is added before the second and fifth letters, and the content in the middle is taken
```python
x = "Hello, world!"
#   01|234|5
print(x[2:5])
```

Result:
```
llo
```

In this case, it means starting from 0, adding a wall before the 0th and 5th letters, and taking the content in the middle
```python
x = "Hello, world!"
print(x[:5])
```

Result:
```
Hello
```

In this case, the second letter starts and the last letter is obtained by default
```python
x = "Hello, world!"
print(x[2:])
```

Result:
```
llo, world!
```

## The application of operators to strings
If you use the ```+``` symbol directly, the two variables will be directly linked into a string
```python
x = "Hello"
y = "World"

print(x + y)
```

Result:
```
HelloWorld
```

If you use ```,``` a blank space will be added between the two variables
```python
x = "Hello"
y = "World"

print(x, y)
```

Result:
```
Hello World
```

Of course, if you have to use +, you can manually add a blank yourself
```python
x = "Hello"
y = "World"

print(x + " " + y)
```

Result:
```
Hello World
```

## 在字符串中加入其它数据类型

如以下例子，当运行时是会报错的
```python
age = 18
name = "alfred"

print('My name is ' + name + ' and i amd ' + age + 'years old')
```
报错的原因是使用```print```和```+```时，不能出现不同数据类型的东西


所以我们就要用其它方法，那就是```format()```


这个的原理是在定义字符串时，先预留几个空位，然后用format方法把空位填上
```python
age = 18
name = "alfred"
print("My name is {} and i am {} years old".format(name, age))
```

这个的原理是先表明，这个字符串需要格式化并把要带入的变量名先写好，那个f也是format的缩写
!> 注意，这里一定要用```{}```不能用其它符号
```python
age = 18
name = "alfred"
print(f"My name is {name} and i am {age} years old")
```

## 忽略某些特殊符号
在python中有好几种特殊符号，包括```"", ''```等

以下例子是会造成报错的
```python
x = "My name is "Alfred" and i am 18 years old"
print(x)
```

解决方法就是加```\```
```python
x = "My name is \"Alfred\" and i am 18 years old"
print(x)
```

这样子，Python就知道，围绕着alfred的```""```要忽略，除此之外```\```配合其它东西会有不同效果

| 代码 | 解释 |
|-----|-----|
|\\'| 忽略当前```'```|
|\\"| 忽略当前```"```|
|\\ | 只显示\ |
| \n | 换行 |
| \t | 一个缩进 | 
| \b | 一个退格 | 

## str类型的方法大杂烩

Python的str类型有非常多内置方法可以使用，这里就没有一一列举，有兴趣的可以慢慢看，也可以到自己喜欢的IDLE里面试试,如果还没下载的话这里有推荐两个，而且有详细教程
- [Pycharm安装](../pycharm.md)
- [Vscode安装](../vscode.md)

| 方法 | 解释 | 
|-----|-----|
| capitalize() | 把字符串的第一个字母转换成大字母 |
| count() | 返回字符串的总长度 | 
| endswith() | 返回一个布尔值，具体结果会根据判断内容 |
| find() | 查询特定的字母，如果有将返回索引 |
| format() | 格式化特定的变量进字符串 |
| format_map() | 格式化特定的变量仅字符串 |
| index() | 查询特定字母在字符串，如果有就返回索引号 |
| isalnum() | 如果字符串全是字母或数字将返回true，否则返回false |
| isalpha() | 如果字符串全是字母将返回true,否则返回false |
| isdecimal() | 如果字符串全是浮点数将返回true,否则返回false |
| isdigit() | 如果字符串全是数字将返回true,否则返回false |
| isnumeric() | 如果字符串全是数值将返回true,否则返回false |
| isprintable() | 如果字符串内容全是可打印的返回true,否则返回false |
| isspace() | 如果字符串是全空白将返回true,否则返回false |
| islower() | 如果字符串全是小字母将返回true,否则返回false |
| isupper() | 如果字符串全是大字母将返回true,否则返回false |
| join() | 将可迭代元素连接到字符串的末尾 |
| lower() | 将所有字母转换成小字母 |
| upper() | 将所有字母转换成大字母 |

当然，不止那么少的，还有很多其它的方法，只是不会经常用到所以这里就媒提及，实在有兴趣的话可以去查资料
