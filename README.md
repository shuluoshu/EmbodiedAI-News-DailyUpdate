# AI自动总结每天讯息简报并push
## Prompt： 
每天早上 9点 给我推送一份“Embodied AI / World Model / Physical Intelligence / VLA”相关技术简报。

任务目标：
只推送近2天内真正有技术信息增量的内容，可以是小红书、Twitter（X）、官方blog、Arxiv paper，github上相关开源更新等，不要把营销宣传、泛媒体转载、招聘贴、公司品牌稿推上来。

主题范围：
1. world model
2. physical intelligence
3. embodied robotics
4. VLA / vision-language-action
5. robot foundation model
6. action model / latent action model
7. policy learning with diffusion or flow matching
8. sim2real / data engine / manipulation benchmarks
9. native multimodality relevant to embodied control

优先来源：
- arXiv / 官方论文
- 官方技术博客
- 官方 GitHub repo / release notes
- 顶会/实验室主页
- 一手访谈或演讲，但必须包含明确技术细节

严格过滤掉：
- 纯融资新闻
- 只有产品发布，没有技术细节
- 标题党二手媒体转载
- 没有方法、实验、数据、系统设计细节的内容
- 只是“某公司很厉害/某机器人会干活”的展示视频
- 与 embodied / world model 无实质关系的泛 AI 新闻

筛选标准：
只有满足以下至少 2 条，才允许进入日报：
A. 有新方法/新架构/新训练范式
B. 有实验、benchmark、ablation、规模信息
C. 有代码、模型、数据集、repo、demo 或技术文档
D. 对具身智能/机器人/VLA/自动驾驶 world model ， world action model等有直接借鉴意义

排序规则：
按“技术信息密度”优先，而不是按热度。
优先级：
论文/官方技术文档 > GitHub 代码更新 > 高质量技术博客 > 访谈/演讲摘要

输出格式：
- 只保留 3~4 条最值得看的内容
- 每条必须包含：
  1) 标题
  2) 来源
  3) 来源链接
  4) 1 句话结论
  5) 为什么值得看（具体技术点）
  6) 和 world model / embodied / VLA 的关系
- 最后单独给一个“今天不值得看但容易被误推的内容类型”小节，提醒我哪些被你过滤掉了
- 按照年月来分文件夹存储，不要直接放在库的根目录

去重规则：
- 已经推送过的内容不要重复推
- 同一论文/同一 repo 的小改动，不要连续多天重复报
- 如果是旧工作突然火了，只有在出现了重要新证据、新代码或新实验时才再次推送

质量要求：
宁缺毋滥。
如果今天没有高质量更新，就直接回复：
“今天没有值得推送的高技术密度内容。”
不要为了凑数而推送。
