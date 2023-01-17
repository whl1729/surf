# 冲浪笔记：Go

## Go language design

- [Notes on structured concurrency, or: Go statement considered harmful][d1] (to_read)
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

- [go ExperienceReports][d9] 类似「用户体验反馈」，提出 Go 使用过程中的一些问题。

- [Proposing Changes to Go][d10] 类似「特性提议」，希望 Go 增加/修改某些特性。

- [How Go was made][d11]

- [The Evolution of Go][d12]

- [Go, Open Source, Community][d13]

- [Go at Google: Language Design in the Service of Software Engineering][d14] Go 发明者谈 Go 的设计

  [d1]: https://vorpus.org/blog/notes-on-structured-concurrency-or-go-statement-considered-harmful/
  [d2]: https://medium.com/eureka-engineering/understanding-allocations-in-go-stack-heap-memory-9a2631b5035d
  [d3]: https://romanyx90.medium.com/go-errors-with-additional-details-66873577f3a9
  [d4]: https://blog.urth.org/2021/03/27/down-the-golang-nil-rabbit-hole
  [d5]: https://betterprogramming.pub/three-things-go-needs-right-now-more-than-generics-a6225d62f76b
  [d6]: https://erik-engheim.medium.com/go-does-not-need-a-java-style-gc-ac99b8d26c60
  [d7]: https://golang.design/history/
  [d8]: https://github.com/teivah/100-go-mistakes
  [d9]: https://github.com/golang/go/wiki/ExperienceReports
  [d10]: https://github.com/golang/proposal
  [d11]: https://go.dev/talks/2015/how-go-was-made.slide#1
  [d12]: https://go.dev/talks/2015/gophercon-goevolution.slide#1
  [d13]: https://go.dev/blog/open-source
  [d14]: https://go.dev/talks/2012/splash.article

## Go Libraries

- [The Go libraries that never failed us: 22 libraries you need to know][l1]

  [l1]: https://threedots.tech/post/list-of-recommended-libraries/

## Go Practices

- [The ecosystem of the Go programming language][pr1]: 介绍Go语言的生态，包括各种工具、资源。 (to_read)
- [Taming Go’s Memory Usage, or How We Avoided Rewriting Our Client in Rust][pr2] (to_read)
- [Forcefully Close TCP Connections in Golang][pr3] (to_read)
- [Finding and fixing memory leaks in Go][pr4] (to_read)
- [Let’s Go with Redis and Lua Scripts][pr5] (to_read)
- [Tutorial: Getting started with fuzzing][pr6] fuzzing 工具可以为测试用例生成随机数据。
- [100-go-mistakes][pr7]
- [Maps and Memory Leaks in Go][pr8]
- [dgryski/awesome-go-style][pr9]: A collection of Go style guides

  [pr1]: https://henvic.dev/posts/go/
  [pr2]: https://www.akitasoftware.com/blog-posts/taming-gos-memory-usage-or-how-we-avoided-rewriting-our-client-in-rust
  [pr3]: https://itnext.io/forcefully-close-tcp-connections-in-golang-e5f5b1b14ce6
  [pr4]: https://dev.to/googlecloud/finding-and-fixing-memory-leaks-in-go-1k1h
  [pr5]: https://xitonix.io/go-lua-and-redis/
  [pr6]: https://go.dev/doc/tutorial/fuzz
  [pr7]: https://github.com/teivah/100-go-mistakes
  [pr8]: https://teivah.medium.com/maps-and-memory-leaks-in-go-a85ebe6e7e69
  [pr9]: https://github.com/dgryski/awesome-go-style

## Go Resource

- [Go 101][r1]: an up-to-date knowledge base for Go programming self learning
- [Airs – Ian Lance Taylor][r2]: A gopher's blog

  [r1]: https://go101.org/
  [r2]: https://www.airs.com/blog/

## Go Test

- [How to use mocks in your table-driven tests in Go][t1]

  [t1]: https://cbrgm.net/post/2022-12-05-go-table-driven-tests-testify/
