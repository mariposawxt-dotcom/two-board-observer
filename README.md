# two-board-observer

一个用于 Codex 的轻量榜单观察 Skill：查询 GitHub Trending 和 Product Hunt，整理为两张简洁表格。

## 使用

将本仓库放入 Codex 的 skills 目录，文件夹命名为 `two-board-observer`，然后调用：

```text
$two-board-observer
```

Skill 会先询问“近一周还是近 3 日”，确认日期后才查询真实数据。也可以直接指定日期范围。

## 观察规则

- 默认每个榜单整理 5 项，不默认仅筛 AI 项目。
- GitHub 按所选区间新增 Star 排序，总 Star 仅作背景。
- Product Hunt 汇总所选日期的榜单、去重并按点赞排序，排除广告。
- 观察日期写完整区间；新增 Star 列名随所选区间变化。
- 点赞显示值与区间新增值分开说明，不将每日累计值相加。
- 缺失数据明确标注；候选样本不冒充全站排名，热度不等于技术成熟或市场验证成功。
- 保留完整表头，不为补齐评论进行深度调查。

完整执行要求见 [SKILL.md](SKILL.md)。使用需要可用的网络查询能力。
