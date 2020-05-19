# 流程控制

## if 语句
if 语句是最基本的流程控制语句，其中仅涉及3个关键字，分别是：if、elif、else，其中elif 相当与if else的意思。

**例：**
```
val = int(input("请输入一个数字:"))
if 0 == val:
	print("你输入的数字是0")
elif 0 < val:
	print("你输入的数字是正数")
elif 0 > val:
	print("你输入的数字是负数")
```

## for 语句
当需要遍历一个字典或列表时，就必需要用到for 语句，它能够按顺序遍历每一项值。

**例：**
```
ls = ["when","who","what","where"]
for item in ls:
	print(item, len(item))
```

## range函数
如果你需要一个数值序列，内置函数 range() 会很方便，它生成一个等差级数链表:

**例：**
```
for i in range(5):
	print(i)
```
range(10) 生成了一个包含 10 个值的链表，它用链表的索引值填充了这个长度为 10 的列表，所生成的链表中不包括范围中的结束值。也可以让 range() 操作从另一个数值开始，或者可以指定一个不同的步进值（甚至是负数，有时这也被称为 “步长”）:

**例：**
```
range(5, 10)
range(0, 10, 3)
range(-10, -100, -30)
```

需要迭代链表索引的话，如下所示结合使 用 range() 和 len():

**例：**
```
words = ['do', 'does', 'did', 'don\'t', 'didn\'t']
for i in range(len(words)):
    print(i, words[i])
```


## break和continue
break语句用于跳出最近的一级 for 或 while 循环。

**例：**
```
for n in range(2, 10):
	for x in range(2, n):
		if n % x == 0:
			print(n, 'equals', x, '*', n//x)
			break
```

continue 语句表示循环继续执行下一次迭代:

**例：**
```
for num in range(2, 10):
	if num % 2 == 0:
		print("Found an even number", num)
		continue
		print("Found a number", num)
```
## pass语句

***pass 语句什么也不做***
它用于那些语法上必需要有什么语句，但程序什么也不做的场合，例如:

**例：**
```
>>> while True:
...     pass  # Busy-wait for keyboard interrupt (Ctrl+C)
...
```

***这通常用于创建最小结构的类***

**例：**
```
>>> class MyEmptyClass:
...     pass
...
```

另一方面，pass 可以在创建新代码时用来做函数或控制体的占位符。可以让你在更抽象的级别上思考。pass 可以默默的被忽视:

**例：**
```
>>> def foo(*args):
...     pass   # Remember to implement this!
...
```

**练习题**
- 一个列表里有10个人
- 遍历这个列表，并打印出第3个人和第7个人的名字

**练习题2**
- 有一个列表如下分别对应了越缅泰3国的[人口，面积，GDP]
```
[
[95540000,329556,244948000000], # 越南
[53710000,676581,71300000000], # 缅甸
[69430000,513120,504993000000] # 泰国
]
```
- 打印出面积最大的国家
- 打印出人口最多的国家
- 打印出GDP最高的国家
- 打印出三个国家的GDP总和
- 打印出三个国家的人均GDP
- 打印出三个国家的人口总和
- 打印出三个国家的面积总和
- 打印出人均GDP最高的国家
- 打印出人均GDP最低的国家
- 打印这三个国家的人均占地面积
- 打印出人均占地面积最大的国家
- 打印出人均占地面积最小的国家
