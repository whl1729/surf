# [Reasoning about asyncio.Semaphore][1] 分析笔记

- 作者对餐厅点餐系统和计算机系统的 `Lock` 进行了类比
  - `acquire()` 代表顾客等待蜂鸣器振动，蜂鸣器振动后 acquire 返回结果
  - `release()` 代表顾客离开，顾客离开时 release 返回结果
  - `cancel()` 代表顾客在蜂鸣器还没振动或刚振动时选择归还蜂鸣器并离开

- 当餐厅厨师和座位变多时，可以允许多个顾客同时就位时，应该使用 `Semaphore` 代替 `Lock`

- 设计同步原语时，需要考虑4个因素：fairness, correctness, semantics and performance

- 关于公平性的一个问题
  - task 刚 release semaphore 又立即 acquire semaphore
  - 类比点餐：顾客刚离开餐厅又立即返回拿到蜂鸣器

- cancellation 的一个问题
  - 当 await 一个 Future 时，这个 Future 可能会中途被取消了，这时 await 操作会抛出 CancelledError
  - 但 await 操作抛出 CancelledError 时，不代表 Future 一定被取消了。
  - 也可能是 Future 可能已经完成，但恰恰这时发生任务调度，新任务取消了 Future 对应的任务。

- Future 的 4 种状态
  - Waiting
  - Done, holding a result
  - Done, holding an exception
  - Done, but cancelled

- [CPython Lock 的实现代码][2]

  [1]: http://neopythonic.blogspot.com/2022/10/reasoning-about-asynciosemaphore.html
  [2]: https://github.com/python/cpython/blob/c70c8b69762f720377adaf22f2e5ec6496a7be53/Lib/asyncio/locks.py#L330
