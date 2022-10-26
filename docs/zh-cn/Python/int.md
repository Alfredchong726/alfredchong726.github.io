# 数字类型
数字类型分为三大类，可是只有int和float经常用到，所有这里complex将不会提及

## int类型
int简单来说就是数字
```python
x = 100
y = "100"
print(type(x))
print(type(y))
```

?> 这里需要注意一点的就是当定义一个数字类型的变量时，都不要用单引号或者双引号，不然Python将默认其为字符串

其中int还包括正负值
```python
x = 1234567890
y = -12345
print(type(x))
print(type(y))
```
## float类型
float其实就是浮点数

?> float类型和int类型一样都是支持正负值的

```python
x = 3.142
y = -3.31

print(type(x))
print(type(y))
```

## 数据类型转换
其中数据类型之间也能进行转换

?> 最容易记的方法就是先输入你要转换的数据类型，后面价格括号，最好在括号里放入你要转换的变量

```python
x = 1       # int类型
y = 1.2     # float类型
z = "1"     # str类型

x = str(x)
y = int(y)
z = float(z)

print(x)
print(y)
print(z)

print(type(x))
print(type(y))
print(type(z))
```