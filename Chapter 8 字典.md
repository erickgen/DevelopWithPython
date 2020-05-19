# 字典

**列表是以连续的整数作为索引，字典是以字符串做为索引。关键字可以是任何不可变类型，通常情况是字符串或数字。**

字典总是以键值对的方式出现，同一个字典中的键永远不能相同。我们用花括号{}来创建一个字典。用逗号“,"来分割数据。

字典的主要操作是通过键来存储和获取值，用del来删除键。

如果一个关键字已经存在，再次为它设置值时将会报错。

## 定义一个字典
```
a = {'name':"张三", "age":28}
b = dict(name="张三",age=28)
```

## 取值和设置值
```
val = a["name"]
print(val)
a["sex"] = "男"
print(a)
```

## 取出所有键
```
key_list = list(a.keys())
print(key_list)
```
## 按键排序
```
sort_keys = sorted(a.keys())
print(sort_keys)
```

## 某个键是否在字典中存在
```
if True == ("age" in a):
	print("In")
else:
	print("Not in")
```

## 综合场景
有个团队有3个人
```
team = [
	{"name":"Elen", "age":28, "manager":True},
	{"name":"Huggo", "age":38, "manager":False},
	{"name":"Otto", "age":21, "manager":False}
]

for item in team:
	print("姓名:"+item["name"]+",年龄:"+str(item["age"])+",是否是经理:"+str(item["manager"]))
```

## 作业
有一场马拉松比赛，总共有10人参加。每个人的字段有：姓名、出生日期、是否为精英选 手、完赛时间。请自行模拟参赛选手数据。
- 请打印出参加马拉松比赛的所有选手
- 请根据完赛时为所有选手排定名次
