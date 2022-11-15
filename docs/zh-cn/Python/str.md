# str(字符串)类型
?> 这里重新说明一次，无论是用```""```还是```''```来创建变量都是一样的，```print()```则是显示结果

## 赋值字符串类型
赋值的流程具体为，变量名加上一个等于号，后面跟着一个变量
```python
x = "alfred"
print(x)
```

## 赋值多行字符串变量
赋值的时候可以赋予多行的变量，可以一定要用三对引号来赋值

?> 这里一样，无论是```""```还是```''```都可以
```python
x = """My name is alfred
I am 10 years old
My hobby is swimming"""
print(x)
```

## 字符串的提取
```python
x = "Hello, world!"
print(x[4])
```

结果：
```
0
```
之所以结果会如此是因为x[4]表示的是在 x变量 中的H开始数，数到第4个的内容，那么可能有人会好奇，第四个不是l吗
!> 电脑算数一律都是从0开始的
```python
x = "Hello, world!"
#    0123456789
```
这里H是0,e则是1，以此类对

## 字符串的切割
上文有提到，电脑是如何从第一个字母开始数数，在字符串的切割中就是使用这个技巧
```python
x = "Hello, world!"
print(x[0:5])
```

结果：
```
Hello
```

这里的原理是想象在x变量中各自在第0和第5个字母前面加一道墙，出来的结果将会是两道墙中间的内容

```python
x = "Hello, world!"
#   |01234|5
```
所以出来的结果就是Hello

除此之外```:```还有其它的使用方法


这个情况就是在第2和第5个字母前面加一道墙，取中间的内容
```python
x = "Hello, world!"
#   01|234|5
print(x[2:5])
```

结果：
```
llo
```

这个情况则代表从0开始，在第0个和第5个字母前面加一道墙，取中间的内容
```python
x = "Hello, world!"
print(x[:5])
```

结果：
```
Hello
```

这个情况是在第二个字母开始，默认拿到最后的字母
```python
x = "Hello, world!"
print(x[2:])
```

结果：
```
llo, world!
```

## 运算符在字符串的应用
如果直接用```+```符号的话，两个变量会直接链接成为一个字符串
```python
x = "Hello"
y = "World"

print(x + y)
```

结果：
```
HelloWorld
```

如果用```,```的话，则会在两个变量的中间加个空白
```python
x = "Hello"
y = "World"

print(x, y)
```

结果：
```
Hello World
```

当然非要用+的话，可以自己手动加个空白
```python
x = "Hello"
y = "World"

print(x + " " + y)
```

结果：
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