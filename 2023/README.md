# 2023年网上冲浪记录

## 2023-12-14

- [OpenAI 翁家翌：ChatGPT 训练师之路][121401]
  - ChatGPT 的训练方法：就直接 RLHF（Reinforcement Learning from Human Feedback，基于人类反馈的强化学习），没啥特殊的玄学技巧。
  - ChatGPT 的不足：肉眼可见的问题还很多，性能还没见顶，以及个人觉得算法层面还有很大的优化空间。
  - 正向反馈
    - 我觉得美国这边相比国内而言，工作环境更友好一些；这边文化上而言就是各种夸夸，其实可以看作一个正的 reward；
    - RL 有个实验结论是长期给负的 reward 是训不出好的策略的，可能他们很早就意识到了这点吧。
  - 如何打造开源生态
    - 代码层面就是兼容性，能够兼容各种上下游的项目、软件，有完善的测试和高覆盖率，文档层面就是有入门指南、API文档、能跑的示例。
    - 社区层面分两部分：
      - 第一部分是用户，提出的issue需要及时回复和跟进（我最近不太跟了因为还有别的工作的事情……十分抱歉）；
      - 第二部分是开发者，项目创立者需要放权（这个是陈天奇老师给的建议），让有能力、有激情的开发者上，不然就只是一个人，不能 scale up上 去；code review 得做好，大家在 code review 的过程中相互交流和学习。
  - 这一年来的一些感想，其实 AI 和非 AI 领域的差别不是想象中那么大：
    - 软件工程很重要，没有好的工程规范，写出来的代码一堆 tech debt，research 再好也没用；
    - 迭代反馈很重要，工作也好，产品也好，生活也好，需要迈出第一步然后去不断打磨迭代；
    - 生产力正比于信息流的传递速度，所以为什么人们总是更喜欢创建一个小的项目而不喜欢在屎山上面堆屎，因为人的 context length 是有限的，
      但是假如一个人的 context length 是无限的话，他就能完全的掌控整个项目，从而做出更精准的决策。同理，公司管理也是这样，人员过多会导致信息流通不畅，导致决策变形；
    - 生产力还反比于一个流程中的人力成本，提升生产力等价于自动化之前需要人力的步骤，很多创业的机会都是这么来的。

  [121401]: https://gitee.com/gitee-stars/32

## 2023-12-13

- [深圳将人工智能教育融入中小学课堂][121301]
  - 深圳外国语学校等61所学校已成为深圳市首批“中小学人工智能教育项目”实验工作学校。深圳园岭小学、南山外国语小学等学校均已开设人工智能相关课程。
  - 2017年，国务院印发《新一代人工智能发展规划》，明确在中小学阶段设置人工智能相关课程，逐步推广编程教育。
  - 2023年7月，深圳市发布《深圳市推进中小学人工智能教育工作方案》，提出要大力促进人工智能与教育教学深度融合，着力培育具有人工智能创新潜质的青少年群体。
  - 目前深圳南山实验教育集团麒麟小学已引入人工智能教育实训平台。该平台采用国产自研编程工具，具备图像识别、人脸识别、声音识别等功能，内置卡通元素、IP角色等创作素材，方便教师教学与学生实训

- [世界机器人大会][121302]
  - 8月16日下午，备受瞩目的2023世界机器人大会在北京北人亦创国际会展中心盛大开幕。

- [世界机器人大赛][121303]
  - 大赛自2015年起已成功举办了8届，共吸引了全球20余个国家20余万名选手参赛，被广泛赞誉为机器人界的“奥林匹克”。
  - 2023世界机器人大赛设共融机器人挑战赛、BCI脑控机器人大赛、机器人应用大赛、青少年机器人设计大赛共四大赛事

- [新基建][121304]
  - 5G 基站
  - 特高压
  - 城际高速铁路，城市轨道交通
  - 新能源汽车充电桩
  - 大数据中心
  - 人工智能
  - 工业互联网

- [build-your-own-x][121305]
  - Master programming by recreating your favorite technologies from scratch.

- [Project Based Learning][121306]
  - A list of programming tutorials in which aspiring software developers learn how to build an application from scratch.

  [121301]: http://edu.people.com.cn/n1/2023/1213/c1006-40137719.html
  [121302]: https://www.worldrobotconference.com/
  [121303]: https://www.worldrobotconference.com/cn/view/1693.html
  [121304]: https://github.com/ruanyf/weekly/blob/master/docs/issue-281.md
  [121305]: https://github.com/codecrafters-io/build-your-own-x
  [121306]: https://github.com/practical-tutorials/project-based-learning

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
