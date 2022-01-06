- 函数, 黑盒, 可复用代码段
- 内建函数
    - https://docs.python.org/zh-cn/3.10/library/functions.html
- 用户自定义函数
- 函数名其实是指向一个函数对象的引用，完全可以把函数名赋给一个变量，相当于给这个函数起了一个“别名”

### 
- 定义函数
```python
def functionName(arguments):
    function body
```
- return
    - 没写return语句默认返回None
    - return None可以简写为return
- pass
    - pass, 占位符
    - 函数体至少需要有一条语句吧, 如果啥也不做, 写个pass即可

- 先定义后调用

### 函数的参数
- 必须参数
    - 按位置匹配, 数量要一致
- 关键字参数
    - 调用时指定形参名, myfunc(name="liws")
    - 调用时允许改变顺序, 因为编译器能通过形参名找到对应关系
- 默认参数
    - 定义时给一个默认值, 如果没传参, 就用默认值
    - 默认参数要放在非默认参数的后面
    - 下面这个例子
    - 如果我想给d传参, 不给c传, 可以通过关键字指定d
    - 一旦用关键字参数给d传了, 想给e传, 就必须用关键字了, 不能用位置了
```python
def myfunc(a, b, c=1, d=2, e=3):
    print(a, b, c, d, e)
```
- 可变参数
    - def myfunc(a, *b): 一个星, b是一个元组
    - def myfunc(a, **b): 两个星, b是一个字典
- 组合参数
    - 上述四种混合使用
    - 定义参数的顺序必须是必须参数、默认参数、可变参数和关键字参数