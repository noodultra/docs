# while循环

*最后编辑于2026/06/09 by:nood*

欢迎来到小南梁的编程手册 Python3第三节 while循环
本节你会学到while循环

## 3.1while循环介绍
while循环就是满足条件就重复执行 不满足条件就停止

## 3.2结构

while循环代码块的结构是:
```python
while 条件 : # 最后面的冒号一定要加
    要重复做的事
```

## 3.3条件

True和False应该知道吧 True的意思是真 False的意思是假 如果你以前不知道 现在应该也知道了吧
在while循环里面 如果条件为True 那这段代码会一直执行 比如:
```python
a = 1
while True:
    a += 1 # a += 1的意思是a = a + 1相当于a加上1然后又赋值给a了
```
那有True肯定也有False 如果条件为False 那这段代码就不会执行 比如:
```python
while False:
    print("这段代码不会执行")
```
你也可以去.py文件里面写上然后运行试试

但是我们也可以写别的条件 不止True和False 比如:
```python
a = 1
while a <= 3:
    a += 1
print(a)
```
这段代码会在a小于等于3的时候重复执行a加1 当a小于等于3的时候 就会跳出循环(也就是停止继续循环执行代码 我们叫做跳出循环) 然后会输出a 那你就会看到a的结果了 现在快去运行一下试试吧

## 3.4break和continue

break和continue在Python3的意思是跳出和跳过

### 3.4.1break

如果while循环里面有个break那就直接跳出循环 比如:
```python
a = 1
while True:
    if a == 5:
        break
    a += 1
print(a)
```
这段代码的意思就是 先判断a是否等于5 如果等于5就跳出循环 直接输出a 如果a不等于5 那就继续执行a加1 顺便说一下 在Python中"="是赋值 而"=="才是等于<br>
防止你们弄混 我再写一段代码
```python
a = 1
while True:
    a += 1
    if a == 5:
        break
print(a)
```
跟刚才那段代码不一样 这段代码是先执行a加1再判断a是否等于5

### 3.4.2continue

如果while循环里面有个continue那就跳过这次循环 直接执行下一轮循环比如:
```python
a = 0
while a < 5:
    a += 1
    if a == 3:
        continue
    print(a)
```
这段代码的意思是 while先判断a是否小于5 如果大于或等于5 直接停止循环 如果小于5 那就先a加1 然后if判断a是否等于3 如果不等于 继续执行 如果等于跳过本轮循环 print会输出每轮循环a的结果 最后的输出是 1 2 4 5 没有"3"是因为到3就跳过了