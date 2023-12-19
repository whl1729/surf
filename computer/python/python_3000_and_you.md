# Python 3000 and You 分析笔记

- Python 3.0 (a.k.a. "Python 3000" or "Py3k") is a new version of the language that is incompatible with the 2.x line of releases.

- Why P33k
  - To fix early, sticky design mistakes
    - e.g. classic classes, int division, print statement
  - Changing times: time/space trade-off
    - e.g. str/unicode, int/long
  - New paradigms come along
    - e.g. dict views, argument annotations

- Major Breakages
  - Print function: print(a, b, file=sys.stderr)
  - Distinguish sharply btw. text and data
    - b"..." for bytes literals
    - "..." for (Unicode) str literals
  - Dict keys() returns a set view [+items()/values()]
  - No default <, <=, >, >= implementation
  - 1/2 returns 0.5
  - Library cleanup and reorganization

- Long Anticipated Breakages
  - Kill classic classes
  - Int/long unification
  - Kill string exceptions
    - Exceptions must subclass BaseException
  - Raise syntax: raise Exc(args) [from tb]
  - Except syntax: except Exc as var:
    - Also makes var undefined at block exit

- Major New Features, e.g.
  - Argument annotations:
    - `def f(a: 2*2, b: 'hello') -> 42: ...`
  - Abstract Base Classes
  - Extended iterable unpacking:
    - `a, b, *x, y = range(5) # 0, 1, [2, 3], 4`
  - New str.format() method:
  - `"Got {0} {kind}".format(42, kind='bugs')` => "Got 42 bugs"

- What’s In It For You
  - More predictable Unicode handling
  - Smaller language
    - Makes “Python fits in your brain” more true
  - **TOOWTDI (There’s Only One Way To Do It -- The Zen of Python)**
  - Common traps removed
  - Fewer surprises
  - Fewer exceptions
