# 点评 [Why operators are useful][1]

## 关键句

- 相比函数名，运算符更符合直觉，更容易被大脑在潜意识下处理

> I think that the fact that formulas written using operators are more easily processed *visually* has something to do with it:
> they engage the brain's visual processing machinery, which operates largely subconsciously, and tells the conscious part what it sees
> (e.g. "chair" rather than "pieces of wood joined together").

- 运算符的另一个强大之处是方便拓展（重载）

> Another very powerful aspect of operator notation is that it is convenient to apply them to objects of different types.

- 大多数情况下，可读性优先于性能

> "But what about performance?" I hear you ask. Good question. IMO, readability comes first, performance second.
> And in the basic example (d = d1 + d2) there is no performance loss compared to the two-line version using update, and a clear win in readability.
> I can think of many situations where performance difference is irrelevant but readability is of utmost importance, and for me this is the default assumption
> (even at Dropbox -- our most performance critical code has already been rewritten in ugly Python or in Go).
> For the few cases where performance concerns are paramount, it's easy to transform the operator version to something else -- 
> *once you've confirmed it's needed* (probably by profiling).

## 点评

赞同 Guido 的观点，可读性优先。

  [1]: http://neopythonic.blogspot.com/2019/03/why-operators-are-useful.html