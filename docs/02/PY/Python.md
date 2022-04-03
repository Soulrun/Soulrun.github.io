# Python 基础
> 9.9网课？ 不不不 网上自学！
> Based on nowcoder.com Python Tutorial
> https://www.nowcoder.com/tutorial/10005/455c61e35dd440ba9d0cd4c0b6f97a3e


## Python 标准数据类型

Python3 中有六个标准的数据类型:
- Number (数字)
- String (字符串)
- Tuple (元组)
- List (列表)
- Set (集合)
- Dictionary (字典)

其中不可变数据的有： 数字 字符串 元组
可变数据的有： 列表 字典 集合

## 列表 List 
是 Python中使用最频繁的数据类型。
可以完成大多数集合类的数据结构实现。

列表是写在方括号[]之间，用逗号分隔开的元素列表。
重点是List中的元素是可以改变的

``` python
a = [1, 2, 3, 4, 5, 6]
a[2:5] = [13,14,16]
print(a)
```
其中append(), pop()等等都是List的修改方法



``` python
# 将一段话的单词倒置

def reversewrd(str):
    str_split = str.split(" ") # 以空格区分
    str_split = str_split[-1::-1]
    str_n = ''.join(str_split)
return str_n
```

## Tuple 元组

元组与列表类似，不同之处在于元组的元素不能修改且写在小括号()内。

元组中的元素类型也可以不同

字符串、列表和元组都属于序列(Sequence)

## Set 集合

集合是由一个或数个形态各异的大小整体组成的，构成集合的事物或对象称作为元素或是成员。

基本功能是进行成员关系测试和删除重复元素，可以使用大括号{}或者set()来创建集合，创建一个空集合必须使用set()

``` python
# Set可以进行集合运算
a = set('asdifojfgodisfgk')
b = set('asd')

if 'a' in a:
    print('T’)
else :
    print('F')

print(a - b) # a与b的差集
print(a | b) # a与b的并集
print(a & b) # a与b的交集
```

## Dictionary 字典
字典是Python中有用的内置数据类型

列表是有序的对象集合，字典是无序的对象集合。
两者之间的区别在于字典当中的元素是键来存取的。

字典是一种映射类型，用{}来表示，且是Key和Value的无需集合。

## Python 数据类型转换

| 函数          	| 描述            	|
|---------------	|-----------------	|
| int(x[,base]) 	| 将x转换成整数型 	|
|               	|                 	|
|               	|                 	|

## Python 运算符

Python的运算符有

| 运算符          	| 描述            	|
|---------------	|-----------------	|
|算数运算符	| +, -, *, /, % 取模, **, // 取整除 	|
| 比较运算符       	|      ==, !=,  >, <,  >=, <=         	|
| 赋值运算符              	|  =, += 加法赋值运算符, -= 减法赋值运算, /=, *=, &=, **=, //=             	|
| 位运算符（二进制下）   	|  &, |, ^, ~, << 	|
| 逻辑运算符   	|  and, or, not 	|
| 成员运算符   	|  in, not in 	|
| 身份运算符   	|  is, not is  	|


## Python 转义字符
| 转义字符          	| 描述            	|
|---------------	|-----------------	|
| \b 	| 退格 Backspace 	|
|       \000        	|     空        	|
| \n   	|   换行   	|
| \v   	|   纵向制表符   	|
| \t   	|   横向制表符   	|
| \r   	|   回车   	|
| \f   	|   换页   	|

@1.16 迭代器 