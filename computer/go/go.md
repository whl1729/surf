# 冲浪笔记：Golang

## Golang language design

-  [Notes on structured concurrency, or: Go statement considered harmful][d1] (to_read)
  - The popular concurrency primitives – go statements, thread spawning functions, callbacks, futures, promises, ...
    they're all variants on goto.
  - These primitives are dangerous, because they undermine our ability to **reason about control flow** 
    and compose complex systems out of abstract modular parts,
    and they interfere with useful language features like **automatic resource cleanup and error propagation**.
  - **Nurseries** provide a safe and convenient alternative, and they encourage **clear thinking**.

- [Understanding Allocations in Go][d2] 介绍Go的内存管理
- [Go errors with additional details.][d3] Go对更详细的错误信息的支持
- [Down the Golang nil Rabbit Hole][d4] 关于Golang nil的一些讨论及潜在问题
- [3 Things Go Needs Right Now More Than Generics][d5]
  - Enum
  - Universal nil
  - Concise Error Handling

- [Go Does Not Need a Java Style GC][d6] 讨论Go的内存管理机制

- [Go: A Documentary][d7] Go 历史文献

- [100 Go Mistakes and How to Avoid Them][d8]

  [d1]: https://vorpus.org/blog/notes-on-structured-concurrency-or-go-statement-considered-harmful/
  [d2]: https://medium.com/eureka-engineering/understanding-allocations-in-go-stack-heap-memory-9a2631b5035d
  [d3]: https://romanyx90.medium.com/go-errors-with-additional-details-66873577f3a9
  [d4]: https://blog.urth.org/2021/03/27/down-the-golang-nil-rabbit-hole
  [d5]: https://betterprogramming.pub/three-things-go-needs-right-now-more-than-generics-a6225d62f76b
  [d6]: https://erik-engheim.medium.com/go-does-not-need-a-java-style-gc-ac99b8d26c60
  [d7]: https://golang.design/history/
  [d8]: https://github.com/teivah/100-go-mistakes

## Golang Practices

- [The ecosystem of the Go programming language][pr1]: 介绍Go语言的生态，包括各种工具、资源。 (to_read)
- [Taming Go’s Memory Usage, or How We Avoided Rewriting Our Client in Rust][pr2] (to_read)
- [Forcefully Close TCP Connections in Golang][pr3] (to_read)
- [Finding and fixing memory leaks in Go][pr4] (to_read)
- [Let’s Go with Redis and Lua Scripts][pr5] (to_read)
- [Tutorial: Getting started with fuzzing][pr6] fuzzing 工具可以为测试用例生成随机数据。

###

  [pr1]: https://henvic.dev/posts/go/
  [pr2]: https://www.akitasoftware.com/blog-posts/taming-gos-memory-usage-or-how-we-avoided-rewriting-our-client-in-rust
  [pr3]: https://itnext.io/forcefully-close-tcp-connections-in-golang-e5f5b1b14ce6
  [pr4]: https://dev.to/googlecloud/finding-and-fixing-memory-leaks-in-go-1k1h
  [pr5]: https://xitonix.io/go-lua-and-redis/
  [pr6]: https://go.dev/doc/tutorial/fuzz

## Go Resource

- [Go 101][r1]: an up-to-date knowledge base for Go programming self learning
- [Airs – Ian Lance Taylor][r2]: A gopher's blog

  [r1]: https://go101.org/
  [r2]: https://www.airs.com/blog/
