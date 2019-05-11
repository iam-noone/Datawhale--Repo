
# Datawhale--Python基础

## Task1（2day）
1.环境搭建<br>
- 1)Anaconda环境配置<br>
- 2)解释器<br>

2.python初体验<br>
- 1)print and input<br>

3.python 基础讲解<br>
- 1)python变量特征+命名规则<br>
- 2)注释方法<br>
- 3)python中“：”的作用<br>
- 4)学会使用dir()及help()<br>
- 5)import使用<br>
- 6)pep8 介绍<br>

4.pyhon 数值基本知识<br>
- 1)python 中数值类型，int float bool e记法等<br>
- 2)算数运算符<br>
- 3)逻辑运算符<br>
- 4)成员运算符<br>
- 5)身份运算符<br>
- 6)运算符优先级<br>


### 1 自己找资料
### 2 print和input


```python
print(2 + 2, 50 - 5*6, 2**3)
print("我是print")
print("数字" + str(1))
```

    4 20 8
    我是print
    数字1
    


```python
var1 = input("please input num")
print(int(var1) / 10)

var2 = input("please input string")
print("you input '", var2, "'")
```

    please input num 12345678
    

    1234567.8
    

    please input string hello python
    

    you input ' hello python '
    

### 3 基础


```python
a = 1
b = 1.1
c = 1e100
d = True
e = None   # 特殊的空值， 这是注释

a, b, c, d, e
```




    (1, 1.1, 1e+100, True, None)



help(obj) 查看如何使用obj
dir() 函数不带参数：返回当前范围的所有变量、方法等<br>
dir() 函数带参数，返回该对象的属性、方法等<br>
某一对象使用obj.__ dir __ () , 也可调用该对象的对象、方法<br>


```python
help(print)
```

    Help on built-in function print in module builtins:
    
    print(...)
        print(value, ..., sep=' ', end='\n', file=sys.stdout, flush=False)
        
        Prints the values to a stream, or to sys.stdout by default.
        Optional keyword arguments:
        file:  a file-like object (stream); defaults to the current sys.stdout.
        sep:   string inserted between values, default a space.
        end:   string appended after the last value, default a newline.
        flush: whether to forcibly flush the stream.
    
    


```python
dir(), dir(help), help.__dir__
```

import 可以导入某个模块，多种导入方法


```python
import numpy
import numpy as np
from numpy import array
from numpy import array as arr
```

### 4 python运算符
算数运算符中的 * 可以表示<br>
 1. 两个数相乘
 2. 被重复若干次的字符串


```python
s = "abc"
ss = 3 * s
s, ss
```




    ('abc', 'abcabcabc')



成员运算符<br>
A in, not in B：若A在、不在B中，则返回True、False


```python
A = 1
B = [1, 2, 3]

flag1 = A in B
flag2 = A not in B

flag1, flag2
```




    (True, False)



其余的运算符跟大多数语言类似


```python

```
