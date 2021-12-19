# Meta
# Text
- [微信读书](https://weread.qq.com/web/reader/5ec326407198d66c5ec29c3)
- 解释型, 面向对象, 动态数据类型
- Life is short, you need Python.
## C1 进入Python 3.7的精彩世界
- Python在云计算方面的用途很大，比如云计算中IaaS（Infrastructure as a Service，基础设施即服务）层的很多软件都大量使用Python，云计算的其他服务都建立在IaaS服务的基础上

- 不断更新与发展, [python.org](http://www.python.org)
- http://www.liaoxuefeng.com/（2）http://www.runoob.com/python3/python3-tutorial.html

## C2 开启Python之旅
### 数据类型
- Python 3中有6种标准的对象类型：Number（数字）、String（字符串）、List（列表）、Tuple（元组）、Sets（集合）、Dictionary（字典）
- Python 3支持3种不同的数值类型：整型（int）、浮点型（float）、复数（complex）
- 两个整数相除, / 浮点除, // floor
- 有浮点数, 结果为浮点数


## C3 列表和元组
- 序列(Sequence), Python包含6种内建序列，即列表、元组、字符串、Unicode字符串、buffer对象和xrange对象
### 通用序列操作
- 索引(Indexing), Python支持负数索引
- 索引既可以对变量的引用操作，也可以直接操作序列，还可以操作函数的返回序列
    - 变量, str = 'hello', str[0]
    - 直接操作序列, 'hello'[0]
    - 操作函数的返回序列, input()[0]
- 索引访问单个元素, 切片访问一定范围的元素
- 切片, nums[start:end:step]
    - start指向一个索引, end指向一个索引, 都可以用负数索引, [start, end)
    - start出现位置在end的后面, 得到一个空序列
    - 省略end以获取到最后一个元素, 省略start以从头开始
    - step不能为0, 当step为负数时, start要大于end
- 序列相加, 两个同类型的序列合并为同一个序列
- 序列乘法, 序列乘以一个数字
- 成员资格, a in nums, 数字类型不能在字符串类型中通过in进行成员资格检测，而字符串类型可以在数字列表中通过in进行成员资格检测
- len, max, min
### list
- List is mutable, so we can change the element by nums[i] = obj.
- list.append(obj)
- del list[i]
- myList = list(seq)
- 切片赋值功能很强大
- show = list('abcd'), show[3:] = list('xyz'), show is ['a', 'b', 'c', 'x', 'y', 'z']
- x = list('ae'), x[1:1] = list('bcd'), x is ['a', 'b', 'c', 'd', 'e'], 添加元素
- myList[start:end] = [], 可以做到删除元素的目的
- list.count(obj)
- list.extend(seq)
- list.index(obj)
- list.insert(index, obj)
- elem = list.pop(index), 不填默认-1
- list.remove(obj)
- 