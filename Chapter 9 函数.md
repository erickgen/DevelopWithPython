# 函数

我们使用函数的方式来模块化的解决问题。

使用def定义一个函数

函数可以有返回值，也可以没有返回值

函数可以返回任意类型的值

## 有返回值的函数
```
def foo():
	return "abc"
```
## 没有返回值的函数通常会打印出结果
```
def showCode():
	print("Hello world!")
```
## 函数可以接收一个以上不同类型的参数
```
def countAnts(ants):
	return count(ants)
```

## 我们可以创建一个用来生成指定边界的斐波那契数列的函数:
```
def fib(n):
	"""打印斐波那契数"""
	a, b = 0, 1
	while a < n:
		print(a, end=' ')
		a, b = b, a+b
	print()
```
执行函数
```
fib(2000)
0 1 1 2 3 5 8 13 21 34 55 89 144 233 377 610 987 1597
```
关键字 def 引入了一个函数 定义。在其后必须跟有函数名和包括形式参数的圆括号。函数体语句从下一行开始，必须是缩进的。
函数体的第一行语句可以是可选的字符串文本，这个字符串是函数的文档字符串，或者称为_docstring_。 有些工具通过 docstrings 自动生成在线的或可打印的文档，或者让用户通过代码交互浏览；在你的代码中包含 docstrings 是一个好的实践，让它成为习惯吧。



定义一个返回斐波那契数列数字列表的函数，而不是打印它，是很简单的:
```
def fib2(n): # return Fibonacci series up to n
	result = []
	a, b = 0, 1
	while a < n:
		result.append(a)
		a, b = b, a+b
	return result

f100 = fib2(100)
f100
[0, 1, 1, 2, 3, 5, 8, 13, 21, 34, 55, 89]
```
return 语句从函数中返回一个值，不带表达式的 return 返回 None。过程结束后也会返回None。
