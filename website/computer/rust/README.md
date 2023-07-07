# 冲浪笔记：Rust

## Blog

- [fasterthanli][b1]

  [b1]: https://fasterthanli.me/

## Design

- [Rust's Type System is Turing-Complete][d1] (to_read)
- [Rust 异步不是有色函数！][d2] (to_read)
- [Speed of Rust vs C][d3] (to_read)
- [Rust vs Go][d4] (to_read)
- [What Rust could learn from Kotlin][d5]

  [d1]: https://sdleffler.github.io/RustTypeSystemTuringComplete/
  [d2]: https://www.hobofan.com/blog/2021-03-10-rust-async-colored/
  [d3]: https://kornel.ski/rust-c-speed
  [d4]: https://thenewstack.io/rust-vs-go-why-theyre-better-together/?s=09
  [d5]: https://medium.com/@cedricbeust/what-rust-could-learn-from-kotlin-b32ebe2da28d

## Exercises

- [rust_quiz][e1]
- [经典Rust面试题六道][e2] (Q3: 目前都不会做。)

  [e1]: https://github.com/dtolnay/rust-quiz
  [e2]: https://rustcc.cn/article?id=0b0afa3e-db03-428e-9fc5-b06347997d41

## Frontend Development

- [Rust 是 JavaScript 基础设施的未来][f1]
- [前端研发的新基础设施 - Rust][f2]
- [仅仅过去 4 年，微软最终放弃了 Electron][f3]

  [f1]: https://mp.weixin.qq.com/s?__biz=MzkxNDIzNTg4MA==&mid=2247485792&idx=1&sn=682a4dee7ce4d3b47a81baf9ebd7a98a
  [f2]: https://mp.weixin.qq.com/s/JOnz0IVWRm_bYWReACyWAg
  [f3]: https://mp.weixin.qq.com/s/EeOd-Ln9RUNmeWLlMkJmIg

## Language

- [Rust ownership, the hard way][l1] (Q1: not understand the fourth rule?) (to_read)
- [Rust中的泛型（Part 1.5）][l2] (Q2: not understand) (to_read)
- [Rust: 提防转义序列][l3] (Q7: not understand serde?)
- [Avoiding single-threaded memory access bugs with Rust (for C++ developers)][l4] (to_read)
- [Why Rust strings seem hard][l5] (to_read)
- [Rust shenanigans: return type polymorphism][l6] (to_read)
- [Move Constructors in Rust: Is it possible?][l7] (to_read)
- [Red & blue functions are actually a good thing][l8] (to_read)

  [l1]: https://chrismorgan.info/blog/rust-ownership-the-hard-way/
  [l2]: https://rustyyato.github.io/type/system,type/families/2021/02/22/Type-Families-1_5.html
  [l3]: https://d3lm.medium.com/rust-beware-of-escape-sequences-85ec90e9e243#ee0e-58229fc84d02
  [l4]: https://radekvit.medium.com/avoiding-single-threaded-memory-access-bugs-with-rust-for-c-developers-2b7fc9c877ec
  [l5]: https://www.brandons.me/blog/why-rust-strings-seem-hard
  [l6]: https://loige.co/rust-shenanigans-return-type-polymorphism/
  [l7]: https://mcyoung.xyz/2021/04/26/move-ctors/
  [l8]: https://blainehansen.me/post/red-blue-functions-are-actually-good/

## Libraries

- [Tour of Rust's Standard Library Traits][lib1] (to_read)

  [lib2]: https://github.com/pretzelhammer/rust-blog/blob/master/posts/tour-of-rusts-standard-library-traits.md

## Meetings

- [Rust@Linux Plumbers Conference 2021 (YouTube Video)][m1]
- [Rust in 2021: Where to next?][m2]
- [RustConf 2021 YouTube][m3]
- [官方 RustConf 2021 盘点][m4]

  [m1]: https://www.reddit.com/r/rust/comments/pxz7at/rustlinux_plumbers_conference_2021/
  [m2]: https://nikomatsakis.github.io/rustconf-2021-e44bec44/#1
  [m3]: https://www.youtube.com/playlist?list=PL85XCvVPmGQgACNMZlhlRZ4zlKZG_iWH5
  [m4]: https://www.yuque.com/chaosbot/rust_magazine_2021/mur1r1

## News

- [Rust Blog][n1]
- [Inside Rust Blog][n2]
- [This Week in Rust][n3]
- [Rust语言中文社区][n4]
- [2021年Rust语言中文精选][n5]

  [n1]: https://blog.rust-lang.org/
  [n2]: https://blog.rust-lang.org/inside-rust/index.html
  [n3]: https://this-week-in-rust.org/
  [n4]: https://rustcc.cn/
  [n5]: https://www.yuque.com/chaosbot/rust_magazine_2021

## Practices

- [Rust Style Guide][pr1]
- [Rust Web Developed Roadmap][pr2]
- [Where to go to learn Rust in 2021][pr3]
- [Rust Language Cheat Sheet][pr4]: Rust 函数快查表网站
- [Continuous Integration with Github Actions and Rust][pr5]
- [Effective Rust][pr6]

  [pr1]: https://github.com/rust-dev-tools/fmt-rfcs/blob/master/guide/guide.md
  [pr2]: https://github.com/anshulrgoyal/rust-web-developer-roadmap
  [pr3]: https://loige.co/where-to-go-to-learn-rust-in-2021/
  [pr4]: https://cheats.rs/
  [pr5]: https://www.homeops.dev/continuous-integration-with-github-actions-and-rust/
  [pr6]: https://www.lurklurk.org/effective-rust/

## Projects

- [Ray tracing in One Weekend (Rust Version)][pj1]: Rust for rendering. 
- [Speedy2D: 兼容 OpenGL (ES) 2.0+ 的图像库][pj2] 
- [RG3D: Rust Game engine 3D (and 2D)][pj3]
- [Rust GPU][pj4]: This is a very early stage project to make Rust a first-class language and ecosystem for building GPU code.
- [Tauri][pj5]: 桌面应用开发框架，包含了JavaScript API，可以结合各种主流前端框架进行开发。
- [Postage][pj6]: 异步通道库，提供了丰富的通道集，并在 Sink/Stream 上有很多实用的组合子，方便了异步程序的开发。(to_read)
  (Q8: sink/stream、组合子分别是什么东西？）
- [meio][pj7]: 异步 actor 框架，其设计受 Erlang/OTP 启发. (to_read) (Q9: actor 框架是什么？）
- [message-io][pj8]: 事件驱动的消息库，可轻松快速地构建网络应用程序。
- [nlprule][pj9]: Rust 实现的 NLP 库。
- [Writing a 3D Shooter using rg3d - #3 - Bots, AI][pj10]
- [rkyv][pj11]: `rkyv`宣称堪比`serde_json`序列化更快的crates。
- [华为 | 基于Rust的下一代虚拟化平台-StratoVirt][pj12]
- [Superconsole: A Text-based User Interface (TUI) library written in RUST][pj13]

  [pj1]: https://jduchniewicz.com/posts/2021/02/c-to-rust-or-how-to-render-your-mindset/
  [pj2]: https://github.com/QuantumBadger/Speedy2D
  [pr3]: https://github.com/rg3dengine/rg3d
  [pj4]: https://github.com/EmbarkStudios/rust-gpu
  [pj5]: https://github.com/tauri-apps/tauri
  [pj6]: https://docs.rs/postage/0.4.1/postage/
  [pj7]: https://github.com/rillrate-open/meio
  [pj8]: https://crates.io/crates/message-io
  [pj9]: https://github.com/bminixhofer/nlprule
  [pj10]: https://rg3d.rs/tutorials/2021/03/11/tutorial3.html
  [pj11]: https://github.com/rkyv/rkyv
  [pj12]: https://www.yuque.com/chaosbot/rust_magazine_2021/nc4nvv
  [pj13]: https://developers.facebook.com/blog/post/2022/07/21/superconsole/

## Resources

- [rust-learning][r1]
- [用RUST进行系统编程的自学资源][r2]
- [13年资深开发者分享一年学习Rust经历：从必备书目到代码练习一网打尽][r3]
  - [How I went about learning Rust][r4]
- [Blessed: An unofficial guide to the Rust ecosystem][r5]

  [r1]: https://github.com/ctjhoa/rust-learning
  [r2]: https://github.com/rcore-os/rCore/wiki/study-resource-of-system-programming-in-RUST
  [r3]: https://www.qbitai.com/2022/07/36355.html
  [r4]: https://eli.thegreenplace.net/2022/how-i-went-about-learning-rust/
  [r5]: https://blessed.rs/crates

## Standards

- [2021-02-11 Announcing Rust 1.50.0][s1]
  - Const-generic array indexing (Q4: How to understand the example code?)
  - `const` value repetition for arrays
  - Safe assignments to `ManuallyDrop<T>` union fields (Q5: What does it mean?)
  - A niche for File on Unix platforms (Q6: Not really understand?)
  - Library changes

  [s1]: https://blog.rust-lang.org/2021/02/11/Rust-1.50.0.html

## for Systems

- [Datenlord | 重新思考Rust Async - 如何实现高性能IO][sys1]
- [Writing dockerfile in rust project][sys2]

  [sys1]: https://www.yuque.com/chaosbot/rust_magazine_2021/gxfucm
  [sys2]: https://this-week-in-rust.org/blog/2021/10/06/this-week-in-rust-411/

## Tool

- [使用Meson将Rust混合到现有的C共享库中][tool1]: Cargo的一个替代物。

  [tool1]: https://nibblestew.blogspot.com/2021/03/mixing-rust-into-existing-c-shared.html

## Web

- [Rust for web development][w1]
  - **actix-web** for the HTTP layer.
  - **sqlx** for the database (PostgreSQL).
  - **rusoto** to interface with AWS services for storage (S3), background jobs (SQS) and sending emails (SES).
  - **tera** for email templates.
  - **thiserror** for my error types.
  - **sentry** for error monitoring.

- [MoonZoon 一个 Rust 全栈框架][w2]
- [salvo][w3]: A simple but powerful web server framework written in Rust.
- [Combining Axum, Hyper, Tonic, and Tower for hybrid web/gRPC apps: Part 1][w4]
- [基于Poem的OpenAPI服务端框架][w5]

  [w1]: https://kerkour.com/blog/rust-for-web-development-2-years-later/
  [w2]: https://github.com/MoonZoon/MoonZoon
  [w3]: https://github.com/salvo-rs/salvo
  [w4]: https://www.fpcomplete.com/blog/axum-hyper-tonic-tower-part1/
  [w5]: https://www.yuque.com/chaosbot/rust_magazine_2021/ui0zhh

