### 集合

集合(set)是一种常见的数据类型。它是一个无序不重复的元素集。
基本功能包括关系测试和消除重复元素。集合对象还支持并集、交集、差集、对称差集等数学运算。

我们使用大花括号或者set()函数来创建集合。但是空集合必须使用set()而不是{}来创建。{}用于创建空字典。

例:
```
basket = {'apple', 'orange', 'apple', 'pear', 'orange', 'banana'}
print(basket)
{'orange', 'banana', 'pear', 'apple'}
'orange' in basket
True
'car' in basket
False
```

```
a = set('abracadabra')
b = set('alacazam')
print(a)     # 自动去除a中相同的项
{'a', 'r', 'b', 'c', 'd'}
print(a - b)                        #  在a中存在，但不在b中
{'r', 'd', 'b'}
print(a | b )                         # 在a中存在，或者在b中存在
```

### 增加、移除、更新元素
```
fruit =set(["apple","pear"])
print(fruit)
fruit.add("orange")
print(fruit)
fruit.remote("pear")
fruit.update(["lemon"])
```

### 其它函数说明

```
frozenset() 创建不可变集合

set() 创建集合

len() 返回集合中成员的个数
```

### 遍历元素
```
a = {'apple', 'pear', 'c++', 'css'}
for element in a:
	print(element)
```

### 作业： 确定如下函数的作用并写代码举例

```
pop()
clear()
discard()
copy()
union()
issubset()
```
