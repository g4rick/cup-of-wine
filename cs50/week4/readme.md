# 第四周 数据结构

## 知识点碎片

1. 如果使用了超出声明范围的内存，可能不会崩溃，因为操作系统*可能*会给你分配更多的位置以防万一，但是这个不安全，所以不要这样做。例子：memory1.c
2. 小黄鸭调试：如果没有人帮你调试，把你的思路对着小黄鸭或者其他什么东西说出来，主要目的是为了梳理思路，很大情况下你自己就会发现问题。
3. `malloc` 申请 堆中的内存 `heap`; 变量，函数 申请 栈 （stack）中的内存。
4. `array` 有很多限制：只能存储同样的类型；被限制了大小；
5. `realloc` 可以用来重新分配内存空间。
6. 链表的实现。
7. `Control + d` 用法，结束输入
8. `struct` 中的`->` 语法糖，相当于 `*n.next` 从struct中获取到地址位置，然后通过点操作符得到属性。
9. hash table: 一个 array 每一个字段包含了 一个 link list。
10. 简单介绍了一下其他的数据类型：树(tree)、字典树(trie)、图(graph)。这一部分内容在今后的算法中非常常用，后续会继续学习。

## 堆栈的区别

栈- stack: 

1. 由系统自动分配和释放，用来存放函数、函数参数、变量等值。
2. 向低地址扩展的连续内存, 也就是 array 。


堆- heap : 

1. 由开发手动分配和释放。例如 `malloc`;
2. 向高地址扩展的不连续内存，一般是链表 link list。

## 定义链表

```c
typedef struct node // 这里必须要写一遍node是因为下面在使用node *next的时候必须提前声明过才能用。这个类似前面写的调用方法的上移操作。
{
  int x;
  struct node *next;
}
node;
```

```c
// 正常定义一个结构体是不需要提前定义名字的
typedef struct
{
  char *name;
  char *dorm;
}
student;
```
