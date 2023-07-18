# 冲浪笔记：Go

## Blog

- [Go Blog][b1]

  [b1]: https://blog.golang.org/index

## Design

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
- [Go to use pdqsort instead of quicksort][d7] Go 采用新的排序算法 [pdqsort][d8]
- [The Go Scheduler][d9]
- [Go: A Documentary][d10] Go 历史文献
- [100 Go Mistakes and How to Avoid Them][d11]
- [go ExperienceReports][d12] 类似「用户体验反馈」，提出 Go 使用过程中的一些问题。
- [Proposing Changes to Go][d13] 类似「特性提议」，希望 Go 增加/修改某些特性。
- [How Go was made][d14]
- [The Evolution of Go][d15]
- [Go, Open Source, Community][d16]
- [Go at Google: Language Design in the Service of Software Engineering][d17] Go 发明者谈 Go 的设计
- [Go Proverbs][d18]

  [d1]: https://vorpus.org/blog/notes-on-structured-concurrency-or-go-statement-considered-harmful/
  [d2]: https://medium.com/eureka-engineering/understanding-allocations-in-go-stack-heap-memory-9a2631b5035d
  [d3]: https://romanyx90.medium.com/go-errors-with-additional-details-66873577f3a9
  [d4]: https://blog.urth.org/2021/03/27/down-the-golang-nil-rabbit-hole
  [d5]: https://betterprogramming.pub/three-things-go-needs-right-now-more-than-generics-a6225d62f76b
  [d6]: https://erik-engheim.medium.com/go-does-not-need-a-java-style-gc-ac99b8d26c60
  [d7]: https://github.com/golang/go/commit/72e77a7f41bbf45d466119444307fd3ae996e257
  [d8]: https://arxiv.org/pdf/2106.05123.pdf
  [d9]: https://morsmachine.dk/go-scheduler
  [d10]: https://golang.design/history/
  [d11]: https://github.com/teivah/100-go-mistakes
  [d12]: https://github.com/golang/go/wiki/ExperienceReports
  [d13]: https://github.com/golang/proposal
  [d14]: https://go.dev/talks/2015/how-go-was-made.slide#1
  [d15]: https://go.dev/talks/2015/gophercon-goevolution.slide#1
  [d16]: https://go.dev/blog/open-source
  [d17]: https://go.dev/talks/2012/splash.article
  [d18]: https://go-proverbs.github.io/

## Libraries

- [The Go libraries that never failed us: 22 libraries you need to know][l1]

  [l1]: https://threedots.tech/post/list-of-recommended-libraries/

## News

- [Golang News][n1]
- [Golang Weekly][n2]

  [n1]: https://golangnews.com/
  [n2]: https://golangweekly.com/issues

## Practices

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

## Resource

- [Go 101][r1]: an up-to-date knowledge base for Go programming self learning
- [Airs – Ian Lance Taylor][r2]: A gopher's blog
- [Awesome Go][r3]
- [Go Wiki][r4]
- [Go Documentation][r5]

  [r1]: https://go101.org/
  [r2]: https://www.airs.com/blog/
  [r3]: https://github.com/avelino/awesome-go
  [r4]: https://github.com/golang/go/wiki/
  [r5]: https://go.dev/doc/

## Test

- [How to use mocks in your table-driven tests in Go][t1]

  [t1]: https://cbrgm.net/post/2022-12-05-go-table-driven-tests-testify/
