## 保留关键字

**这些单词不能用作常量、变量或其它任何标识符名称**
```
and exec not assert finally or break for pass class from print continue global raise
def if return del import try elif in while else is with except lambda yield
```
## 行和缩进
**Python中通过缩进来写逻辑模块，而不是用{}**

python
```
if True:
	print("True")
else:
	print("False")
```

php
```
if (True) {
	print("True")
} else {
	print("False")
}
```

## 多行语句
Python语句中一般以新行作为语句的结束符
但是我们可以使用**斜杠**（ \）将一行的语句分为多行显示，如下所示：
```
total = 1 + \
        2 + \
        3
print(total)
```

语句中包含 [], {} 或 () 括号就不需要使用多行连接符。如下实例：
```
days = ['Zero', 'One', 'Two',
        'Three', 'Four']
```

## 字符串
字符串需要用单引号、双引号或三引号包裹起来，三引号可以引用多行文本，有时三引号被当作注释。
```
foo = '单引号括起来的字符串'
foo1 = "双引号括起来的字符串"
foo2 = """这是多行文本，
这是第二行。"""
```

## 注释
**注释分为两种**
```
# 这是一行注释

"""
这是多行注释的第一行
这是第二行
"""
```

## 开始编程
**文件开头、设定变量、逻辑判断、输出结果**
```
#!/usr/bin/python
# -*- coding: UTF-8 -*-

# 总预算
total_budget = 1000
# 旅行人数
person_num = input("请输入旅行人数:")
# 每人费用
pre_cost = input("请输入每人费用:")

# 总费用
total_cost = int(person_num) * float(pre_cost)

# 打印总费用
print("您的总预算是:" + str(total_budget) + ",这次旅行的总费用是：" + str(total_cost))

# 逻辑判断后给出建议
if (total_cost > total_budget) :
    print("您的费用已超出预算" + str(total_cost-total_budget)+"元，请重新制定您的旅行计划\n")
elif(total_cost == total_budget):
    print("您的费用和预算完全吻合, 祝您旅途愉快\n")
else:
    print("您此次旅行的费用比预算少了" + str(total_budget - total_cost) + "元，祝您旅行愉快\n")
```
