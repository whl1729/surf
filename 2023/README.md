# 2023年网上冲浪记录

## 2023-12-12

- [国家统计局关于2023年粮食产量数据的公告][121201]
  - 2023年全国粮食总产量为 69541 万吨（13908亿斤），其中谷物产量 64143 万吨（12829亿斤）
  - 2023年全国粮食总产量13908.2亿斤，比上年增加177.6亿斤，增长1.3%，连续9年稳定在1.3万亿斤以上。
  - 粮食包括谷物、豆类、薯类。
  - 谷物主要包括稻谷、小麦、玉米、大麦、高粱、荞麦和燕麦等。
  - 各省份产量排名：黑龙江（7788.2）、河南（6624.3）、山东（5655.3）、吉林（4186.5）、安徽（4150.8）、内蒙古（3957.8）、河北（3809.9）

- [Text Editor Data Structures: Rethinking Undo][121202]
  - 讨论编辑器中 Undo 和 Redo 的一些设计问题

  [121201]: https://www.stats.gov.cn/sj/zxfb/202312/t20231211_1945417.html
  [121202]: https://cdacamar.github.io/data%20structures/algorithms/benchmarking/text%20editors/c++/rethinking-undo/

## 2023-12-07

- [How Often Should We Sharpen Our Tools?][120701]
  - 作者讲述自己的文本编辑器的切换过程：NEdit（使用15年以上） -> vim （几年）-> neovim
  - neovim 相比 vim 的优势：异步操作（不会阻塞UI）、支持 Lua
  - 在提升工具使用效率与处理实际工作任务之间取得平衡，「磨刀不误砍柴工」

- [Nuclear Reactor Simulator][120702]
  - 一个核反应堆模拟器，可以用来熟悉核反应堆的原理。有空玩一下。
  - 另外，这种科普类的软件作品，也是我比较感兴趣的项目。以后可以多了解这方面的软件作品。

  [120701]: https://tratt.net/laurie/blog/2023/how_often_should_we_sharpen_our_tools.html
  [120702]: https://dalton-nrs.manchester.ac.uk/

## 2023-12-03

- [朱雀二号遥三火箭已转运至发射区][120301]：该火箭由民商火箭蓝箭航天研发。

- [Code is run more than read][120302]
  - 提出一个模型，来概括软件开发时对各种优先级的权衡，比如：`biz > user > ops > dev`
  - 对我的启示：软件开发不仅要考虑开发规范性和可维护性，还需要考虑商业价值和用户需求。

  [120301]: https://www.chinanews.com.cn/shipin/cns-d/2023/12-03/news976846.shtml
  [120302]: https://olano.dev/2023-11-30-code-is-run-more-than-read/

## 2023-12-02

- [Not Everything Is Google’s Fault (Just Many Things)][120201]: 批评谷歌云的一些坑
  - 网络不稳定
  - 自动清空 Artifact Registry
  - 人工支持不给力
  - 用户空间到内核的内存通信存在致命的 bug

- [世界最大的国际热核聚变实验反应堆（ITER计划，又称人造太阳）][120202]

  [120201]: https://blog.railway.app/p/gcp-incidents
  [120202]: http://finance.people.com.cn/n1/2023/1202/c1004-40130319.html

## 2023-11-30

- [Fourteen Years of Go][113001]：Go 1.21 增加的内容
  - PGO (Profile-guided optimization)
  - cmp, maps, slices packages
  - log/slog

- [Fixing For Loops in Go 1.22][113002]
  - A mistake: keeping a reference to a loop variable past the end of its iteration, at which point it takes on a new value that you didn’t want.

  [113001]: https://go.dev/blog/14years
  [113002]: https://go.dev/blog/loopvar-preview

## 2023-11-29

- 2023年11月28日，查理·芒格去世。

## 2023-11

- 2023-11-29: [How to build a self driving car in one month][112901]
- 2023-11-06: [Syntactic sugar to encourage use of named arguments][110601]

  [112901]: ./automation/how_to_build_a_self_driving_car_in_one_month.md
  [110601]: ./computer/python/syntactic_sugar_to_encourage_use_of_named_arguments.md

## 2023-10

- 2023-10-25: [沉潜十年：最诚恳的希望][102501]
- 2023-10-19: [Write more "useless" software][101901]

  [102501]: ./psychology/10_years_of_silent_hard_work.md
  [101901]: ./computer/attitude/write_more_useless_software.md

## 2023-09

- 2023-09-12: [The roots of an obscure Bourne shell error message][091201]

  [091201]: ./computer/shell/the_roots_of_an_obscure_bourne_shell_error_message.md

## 2023-08

- 2023-08-28: [How To Do Great Work][082801]
- 2023-08-12: [The Legacy of Bram Moolenaar][081202]
- 2023-08-12: [Vim Boss][081201]
- 2023-08-09: [What to do with your computer science career][080901]
- 2023-08-09: [King's Day Speech][080902]

  [082801]: ./psychology/how_to_do_great_work.md
  [081202]: ./computer/python/the_legacy_of_bram_moolenaar.md
  [081201]: ./computer/python/vim_boss.md
  [080901]: ./computer/python/what_to_do_with_your_computer_science_career.md
  [080902]: ./computer/python/kings_day_speech.md

## 2023-07

- 2023-07-31: [Why operators are useful][073101]
- 2023-07-28: [Reasoning about asyncio.Semaphore][072801]
- 2023-07-25: [Python 3000 and You][072501]
- 2023-07-25: [Why I Invented Python][072502]

  [073101]: ./computer/python/why_operators_are_useful.md
  [072801]: ./computer/python/reasoning_about_asyncio_semaphore.md
  [072501]: ./computer/python/python_3000_and_you.md
  [072502]: ./computer/python/why_i_invented_python.md

## 2023-05

- 2023-05-15: [What Color is Your Function?][0515]
- 2023-05-14: [Creative Thinking][0514]

  [0515]: ./computer/pl/what_color_is_your_function.md
  [0514]: ./psychology/creative_thinking.md