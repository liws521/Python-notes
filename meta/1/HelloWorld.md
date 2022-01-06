# Meta
# Text

### Q&A
- How to indicate a code block?
    - Python - tab
    - Other languages - {}
- Comment
    - Python - #
- ;
    - Python, Golang, - NO
- 变量声明
    - Python的变量名(一个标识符)不与特定类型的内存空间关联
    - a = 1; 声明变量时无须指定类型
    - 先声明后使用, del a, 删除变量
- 如何理解变量与内存
    - int a = 5;
    - 声明了一个4字节的内存空间, 是一个存储值的容器
    - C语言中的变量就是这个容器, a这个标识符和这块内存空间是一体的
    - Python中的a这个标识符只是一个容器上的标签, 可以多个标签指向同一个容器