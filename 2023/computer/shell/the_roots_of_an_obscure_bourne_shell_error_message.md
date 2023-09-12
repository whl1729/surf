# 点评 [The roots of an obscure Bourne shell error message][1]

这篇博客是对 bash 一个小问题的分析，通俗易懂，主要涉及到两个知识点：临时设置环境变量、间接调用命令。

如果你没时间，只看这一段也能吸取整篇博客的精华：

> If you write 'AVAR= $(....)', the Bourne shell first sees 'AVAR= ' (with the space) and interprets it as you running some command with $AVAR set to a blank value.
> Then it takes the '$(...)' and uses it to generate the command to run (and its command line).
> When your subshell prints out its results, for example the number of lines reported by 'wc -l',
> the Bourne shell will try to use that as a command and fail, resulting in our weird and obscure error message.
> What you've accidentally written is similar to:

```sh
cmd=$(... | wc -l)
AVAR= $cmd
```

  [1]: https://utcc.utoronto.ca/~cks/space/blog/unix/BourneShellObscureErrorRoots
