# 点评 [Syntactic sugar to encourage use of named arguments][1]

这其实是 Python 讨论区的一个话题，有人提出给命名变量增加一个语法糖，让它写起来更方便（如下所示）：

```python
# 目前的写法
my_function(
  my_first_variable=my_first_variable,
  my_second_variable=my_second_variable,
  my_third_variable=my_third_variable,
)

# 加上语法糖的写法
my_function(=my_first_variable, =my_second_variable, =my_third_variable)
```

Python 之父以及其他一些人对这个特性表示欢迎，但 [Miraculixx][2] 及其他一些人则表示[强烈反对]，
原因是：不明显、隐晦、跟 `keyword=value` 的语法不一致、增加复杂度、导致糟糕的命名空间等。

我也不喜欢这个语法糖，觉得这个写法有点奇怪。

  [1]: https://discuss.python.org/t/syntactic-sugar-to-encourage-use-of-named-arguments/36217
  [2]: https://discuss.python.org/t/syntactic-sugar-to-encourage-use-of-named-arguments/36217/21