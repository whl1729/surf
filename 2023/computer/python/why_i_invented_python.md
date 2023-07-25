# Why I Invented Python 分析笔记

- Python's Birthday: Xmas 1989

- Some Design Goals
  - Shell-like (interactive prompt as well as script files)
  - Extensible architecture (create new types)
  - One tool amongst many, work well with others
  - Additional functionality implementable separately
  - Avoid Not-Invented-Here syndrome (borrow freely)
  - Doable as a one-person project (cut some corners)

- Why Object Oriented?
  - One word: extensibility
  - The original design was OO inside and used OO notation for method access, but did not support user-defined classes
  - Method access was generalized to namespaces
  - One unified namespace for everything in a module
  - Each object is a namespace in its own right
  - A module is just another object
  - Name lookup is customized per namespace
  - User-defined classes were added within the first year, but for a long time remained second-class citizens (until new-style classes in Python 2.2)

- Biggest mistakes:
  - 32-bit integers (premature optimization)
  - int/int truncating the value (mindlessly copied C)
  - class/type dichotomy (user-classes an afterthought)
  - string exceptions (exceptions came before classes!)

## 疑问

- Biggest mistakes 里面每一点为什么被认为是错误？