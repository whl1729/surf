# What Color is Your Function 分析笔记

[原文链接][1]

## 这篇文档讨论什么话题

- 异步编程
- promise
- future
- await
- continuation-passing style (CPS)
- 事件循环
- 调用栈
- 异步编程的实现

## 目前为止我知道什么

- JavaScript 有 async、await 、promise、future 等语法
- Python 有 async 和 await 等语法，其中 async 有 async def、async with、async for 等结构
- JavaScript 存在回调地狱的现象
- JavaScript 异步编程容易犯的一个错误是漏掉 await
- JavaScript 异步编程容易犯的另一个错误是没有正确处理异常，导致 uncaught exception

## 目前为止我不知道什么

- JavaScript 和 Python 的事件循环（event loop）的内部实现
- 异步编程和异步I/O有什么联系
- 异步编程的异常处理
- JavaScript promise 的内部实现
- Python yield 的用法（不熟悉）
- Python asyncio 的用法（不熟悉）
- 回调函数的内部实现
- continuation-passing style (CPS) 的作用、用法与原理

## 这篇文档的主要内容是什么

### 这篇文档的章节

- 一门新的语言
- 你的函数是什么颜色
- 这是函数式编程的错误
- 一个丰富多彩的的寓言
- I promise the future is better
- I'm awaiting a solution
- 哪些语言没有颜色
- 记住过去的操作
- Awaiting a generated solution
- 具体化的回调

### 这篇文章各章的内容

- 一门新的语言
  - 语法类似 JS
  - 函数为一等公民，因而有高阶函数

- 这门语言的怪异特性
  - 所有函数都有颜色：红色或蓝色
  - 函数的调用方式取决于颜色：函数颜色不同，调用方式也不同
  - 每个红色函数的调用者必须为红色函数
  - 调用红色函数比调用蓝色函数更痛苦
  - 部分核心库函数是红色的

- 红色的传染性
  - 如果你的函数参数存在高阶函数，那么你的函数需要定义为红色
  - 如果你的函数调用了红色的库函数，那么你的函数需要定义为红色
  - 并且自你的函数而上，整条调用链的函数都需要定义为红色

- 红色函数隐喻异步函数
  - 同步函数返回值，异步函数不会返回值，而是调用回调函数
  - 同步函数通过返回值提供执行结果，异步函数通过回调函数提供执行结果
  - 同步函数不能调用异步函数，因为拿不到执行结果
  - 异步函数的错误处理方式不同，无法用在 try/catch 或其他一些控制流语句里面
  - Node.js 的核心库函数全部是异步的

- I promise the future is better
  - Promise 是一个表达异步操作的类，它封装了回调函数和错误处理
  - Promise 使用起来相对没那么痛苦，但没有改变问题的本质
    - 仍然无法用在异常处理或其他控制流语句
    - 仍然无法被同步函数调用

> 伍注：作者在这里似乎玩了点幽默：我承诺未来会更好，但事实并非如此。

- I'm awaiting a solution
  - await 解决了问题4，但没有解决其他4个问题

- 哪些语言没有颜色
  - Go, Lua 和 Ruby 没有颜色
  - 这三门语言的共同点是使用线程（可以是用户线程）
  - Goroutine、coroutine、fiber

> Threads. Or, more precisely: multiple independent callstacks that can be switched between.
> It isn’t strictly necessary for them to be operating system threads.
> Goroutines in Go, coroutines in Lua, and fibers in Ruby are perfectly adequate.

- 记住过去的操作
  - 调用异步函数后，编译器会将任务放在事件循环中，然后立即返回
  - 任务完成后恢复到调用处的常用方法是调用栈
  - continuation-passing style

> But to do async IO, you have to unwind and discard the entire C callstack.
> Kind of a Catch-22.
> You can do super fast IO, you just can’t do anything with the result!
> Every language that has async IO in its core—or in the case of JS, the browser’s event loop—copes with this in some way.
>
> 伍注：没看懂以上这段话？

- Awaiting a generated solution
  - 编译器在执行 await 语句时实际上进行了 CPS-transform
  - 生成器和 async-await 是同构的

> So with callbacks, promises, async-await, and generators,
> you ultimately end up taking your asynchronous function and smearing it out into a bunch of closures that live over in the heap.
>
> Your function passes the outermost one into the runtime.
> When the event loop or IO operation is done, it invokes that function and you pick up where you left off.
> But that means everything above you also has to return. You still have to unwind the whole stack.
>
> This is where the “red functions can only be called by red functions” rule comes from.
> You have to closurify the entire callstack all the way back to main() or the event handler.
>
> 伍注：没看懂以上这几段话？

- Reified callstacks
  - Go 是线程实现得最漂亮的语言
  - Go 消除了同步代码和异步代码的差别

> 伍注：需要好好体会。

## 如何评价这篇文档

## 这篇文档对我有什么帮助

  [1]: https://journal.stuffwithstuff.com/2015/02/01/what-color-is-your-function/
