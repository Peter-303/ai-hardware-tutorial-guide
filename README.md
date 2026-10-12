# ✍️ tutorial-writer · AI 硬件教程写作助手

一个 [Claude Code](https://claude.com/claude-code) Skill，让 Claude 帮你写出**亲切不劝退、与运营高度适配**的 AI 硬件开源教程。

写作规范沉淀自 [Datawhale](https://github.com/datawhalechina) 社区 200+ 开源教程的实践（含官方 DOPMC 流程与 [whale-bot 鲸鱼小车](https://github.com/datawhalechina/whale-bot)）。

## 它能干什么

| 你说 | 它做 |
|---|---|
| "帮我写第 3 章" | 先问齐关键信息，再按六段式模板产出"保姆级"章节正文 |
| "写教程 README" | 按"路人 30 秒决策路径"的区块骨架成文，含目录即看板 |
| "写这期招募帖" | 套用组队学习话术库，保留"晒成果→降门槛→造稀缺"三板斧 |
| "审校这篇教程" | 对照风格自检清单，输出 ✅/❌ 两栏 + 修改建议 |

每次出稿前自动过 9 条**终审红线**：劝退词黑名单、步骤三件套（操作+图+预期结果）、版本号精确到牙齿、高危步骤兜底……

## 安装

把整个 `tutorial-writer` 文件夹复制到你项目的 `.claude/skills/` 目录下：

```
你的项目/
└── .claude/
    └── skills/
        └── tutorial-writer/   ← 就是这个文件夹
            ├── SKILL.md
            └── references/
```

重启 Claude Code 会话后，用自然语言（"帮我写教程章节"）或 `/tutorial-writer` 即可触发。

> 📦 本 skill 为自包含设计：风格指南、流程 SOP、运营手册、三套模板全部内置在 `references/` 中，拷到任何项目都能独立工作。

## 目录结构

```
tutorial-writer/
├── SKILL.md                          # skill 主文件：工作流程 + 终审红线
├── README.md                         # 本文件
└── references/
    ├── 01-教程生产流程SOP.md          # 七阶段教程生产流程（筹划→立项→开发→内测→公测→毕业→运营）
    ├── 02-语言与风格指南.md           # 措辞规范（核心资产，每条配正反例）
    ├── 03-运营手册.md                 # 组队学习运营打法 + 话术库
    └── templates/
        ├── README模板.md              # 教程仓库首页骨架
        ├── 章节模板.md                # 单章正文六段式骨架
        └── 贡献指南模板.md            # 社区贡献分级指南
```

## 方法论来源

- [datawhalechina/DOPMC](https://github.com/datawhalechina/DOPMC) —— Datawhale 官方项目流程
- [datawhalechina/whale-bot](https://github.com/datawhalechina/whale-bot) —— AI 硬件教程标杆
- [datawhalechina/self-llm](https://github.com/datawhalechina/self-llm) / [llm-universe](https://github.com/datawhalechina/llm-universe) / [tiny-universe](https://github.com/datawhalechina/tiny-universe) 等 —— README 与内容组织范式
- [datawhalechina/team-learning](https://github.com/datawhalechina/team-learning) —— 组队学习运营模式

## 📄 License

[CC BY-SA 4.0](https://creativecommons.org/licenses/by-sa/4.0/) · 模板可自由取用，不必署名
