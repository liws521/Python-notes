Python包含6种内建序列, 即列表, 元组, 字符串, Unicode字符串, buffer对象和xrange对象

### 序列通用操作
- 通用操作: 索引(indexing), 分片(slicing), 序列相加(adding), 乘法(multiplying), 成员资格, 长度, 最小值和最大值
---
- 索引(Indexing), Python支持负数索引
- 索引既可以对变量的引用操作, 也可以直接操作序列, 还可以操作函数的返回序列
    - 变量, str = 'hello', str[0]
    - 直接操作序列, 'hello'[0]
    - 操作函数的返回序列, input()[0]
---
- 索引访问单个元素, 切片访问一定范围的元素
- 切片, nums[start:end:step]
    - start指向一个索引, end指向一个索引, 都可以用负数索引, [start, end)
    - start出现位置在end的后面, 得到一个空序列
    - 省略end以获取到最后一个元素, 省略start以从头开始
    - nums[:], 取得整个序列
    - step默认为1, 不能为0, 当step为负数时, start要大于end才能得到元素, 否则是空序列
- 序列相加, 两个同类型的序列通过加号进行连接
- 乘法, 序列乘以一个数字, 得到一个新的序列, 'hello' * 5
- 成员资格, a in nums, 数字类型不能在字符串类型中通过in进行成员资格检测, 而字符串类型可以在数字列表中通过in进行成员资格检测
- len, max, min
