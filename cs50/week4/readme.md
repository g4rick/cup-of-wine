# 第四周 数据结构

## 知识点碎片

1. 如果使用了超出声明范围的内存，可能不会崩溃，因为操作系统*可能*会给你分配更多的位置以防万一，但是这个不安全，所以不要这样做。例子：memory1.c