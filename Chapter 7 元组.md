# 元组

元组和列表很相似，但元组更像一个字符串，其值不可改变。
我们常常用元组来存储坐标信息，或者是员工的个人信息。

```
point = (100,200)
print(100,200)
```

元组的使用也很方便
```
student = ("张三", 19, "男")
for item in student:
	print(item)
	
print(student[0])
```

可以有空元组
```
t = ()
```

或者只有一个元素的元组，但是结尾必需一个逗号，虽然不好看，但是很实用。
```
t = ("that",)
```

在很多情况下，元组会做为字典或者列表的值，例如：
```
sheets = [(11,12),(21,22),(31,32)]
sheets = {1:(11,12),2:(21,22)}
```
