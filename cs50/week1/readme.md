# 第1周 C 

## 知识点碎片

1. 复习上周内容，通过二进制标示数字，这些数字在不同的解析下解释成 HI! 或者 一种类似黄色的颜色。
2. 复习上周：input + algorithms = output。还有时间复杂度。
3. 通过游戏指出：计算机只能执行确定的指令，不能有假设，否则会出错。如果不是你，那么总要有一个人至少做一次这些繁琐的事情。
4. 通过 Scratch 对比 C 中的一些语法来介绍C。这块比较熟悉，快速过一下。
5. 机器只能理解机器语言，所以我们需要某种方法将我们写的东西(source code) 转换成机器理解的 machine code，这个叫做编译器 compiler。
6. 简单的 hello.c 项目，用来入门。同时 clang 是一个基础命令我们可以在自己的 mac 上尝试。 
7. stdio 也就是 standard input & output 是 c 用来执行 IO 操作的基础库。需要引入否则编译器不认识 printf 函数。
8. clang 接受很多参数 例如： `clang -o hello hello.c` 也就是 `output` 来重新命名，可以用 `clang --help` 来查看支持的命令。
9. `make` 命令，并不是一个 compiler ，而是一个封装了 clang 命令的程序。用来简化输入的命令。
10. 调试技巧。同时解释了为什么要引入文件。
11. `printf` 参数 `%s %i` 等的解释
12. IEEE754 float 浮点数 精度问题，32位或者64位系统的向上溢出问题。


## 总结

这周算是以 c 为入门语言介绍了编程中的一些思想，毕竟写了7年了所以都是1.5倍速看的。对于入门编程的人来说非常有意义，当时我就在想如果当时大学我的老师是这种水平我可能就不会需要多花费那么多时间在图书馆和实验室了，哈哈~。

总之，简单的入门，后面我应该也会以1.25倍速来看吧，毕竟这些都太熟悉了，虽然很久没有写 c 了。

c 的重学将是我下下阶段的事情，在学习这个视频的同时睡前也在看那本非常厚的 CSAPP。
