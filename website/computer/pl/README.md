# 冲浪笔记：编程语言

## Compiler

- [Technique: Compile Time Code Generation and Optimization][c1]: C++ 实现 brainfuck 编译器

  [c1]: https://www.foonathan.net/2022/01/compile-time-codegen/

## Programming Language Exercises

- [exercism][e1]

  [e1]: https://exercism.org/

## Programming Language History

- [编程珠玑番外篇-D. 高级语言怎么来的-1][h1]
  - Fortran
    - 第一版的 FORTRAN 不支持递归.
    - 不支持递归的语言能**图灵完全**么?　当然可以, 图灵机就是没递归的典型的例子.
    - 用现在的眼光看,　FORTRAN 语言能构模拟图灵机上的一切操作,　所以是图灵完全的.
  - Lisp
    - McCarchy 喜欢丘齐的那一套 **Lambda 演算**, 而非图灵的机械构造.
      所以, LISP 从一开始, 就支持递归的调用, 因为递归就是 lambda 演算的灵魂.
    - REPL (read–eval–print loop)
    - 因为有了**运行时**的概念, LISP 想怎么递归, 就可以怎么递归。
    - 对空间分配的动态支持, 随之就带来了一项新技术: 垃圾收集器. 这个技术出现在　LISP 里面不是偶然的, 是解释器的自然要求和归宿.
    - LISP 的划时代意义和解释器技术, 使得伴随的很多技术, 比如抽象语法树, 动态数据结构, 垃圾收集, 字节码等等, 都很早的出现在了 LISP 中.

  [h1]: https://blog.youxu.info/2009/05/13/hpl/
