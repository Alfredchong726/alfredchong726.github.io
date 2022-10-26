# 变量
## 注释
每个编程语言都有自己注释的符号，而注释了的代码或者其它内容将不被运行，在Python中注释的符号为#

```python
print("Hello World")
# 这是一个注释，这里的内容将不被运行
```

这个方法用于注释一行，除此之外还有一个方法能够注释多行

```python
print("Hello World)
"""
这是多行注释
这里的所有东西将不被运行
"""
```


## 创建变量
首先，我们要先了解什么是变量，变量就像一个储存资料的容器,当你定义一个变量时，电脑会将资料存进记忆体里
?> 创建变量的过程也称之为 赋值
那么要在Python中要怎么定义变量呢
```python
x = 10
y = "alfred"

print(x)
print(y)
```

?> 在Python中，不需要先定义一个变量的数据类型，可以直接定义变量

## 单引号还是双引号
```python
a = 'Shelly'
a = "Shelly"
# 在Python定义变量的时候无论是使用单引号还是双引号都是可以的
```

## 区分大小写
```python
#在Python中定义变量时，变量名的大小写是区分开来的
a = 'Shelly'
jA = 'alfred'
# 这里的a和A是不一样的 并不会被覆盖内容
```

## 定义变量的规则

?> 这里的例子是可以的
```python
var = 10
_var = 10
my_var = 10
VAR = 10
Var = 10
var1 = 10
```

?> 这些例子则是会报错的
```python
2var = 10
my-var = 10
my var = 10
```

## 同时定义多个变量
这个例子是一行代码中定义多个不同的变量
```python
x, y, z = "alfred", "shelly", "jane"
print(x)
print(y)
print(z)
```

这个例子是一行代码中定义多个一样但不同变量名的变量
```python
x = y = z = "alfred"
print(x)
print(y)
print(z)
```

## 打印结果
```python
x = y = z = "alfred"
print(x)
print(y)
print(z)
```
这里```print```的意思是打印出内容


?> 这个例子是将x的内容和y的内容一起打印
```python
x = "shelly"
y = "alfred"

print(x + y)
```

结果 ：
```
shellyalfred
```

!> 这里要注意一点，这个例子是会报错的，因为数字不能同时和字符串一起打印出来
```python
x = 10
y = "alfred"

print(x + y)
```

结果 ：
```
10alfred
```

?> 但是一下内容可以打印出来，原因是虽然一样都是在同一样打印出来，但是却是分开打印的
```python
x = 10
y = "alfred"

print(x, y)
```

结果 ：
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