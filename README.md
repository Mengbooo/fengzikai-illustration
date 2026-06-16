# 丰子恺水墨插图 / Feng Zikai Ink-Wash Illustration

[![skills.sh](https://skills.sh/b/Mengbooo/fengzikai-illustration)](https://skills.sh/Mengbooo/fengzikai-illustration)

> 用丰子恺的方式画画——温暖、俏皮、不严肃。支持淡彩和纯黑白两种模式。
>
> 竖版 3:4 | 水墨淡彩 | 纯黑白 | 简笔人物 | 手写题字 | 兼容 Claude Code / Codex / Hermes

---

## 这是什么

一个 AI Agent Skill，用丰子恺（1898-1975）的风格为文章配图。

丰子恺的画不是端庄的"国风插画"——他画小孩打架、猫咪捣乱、大人出糗，都带着一种"觉得好笑但不说破"的温柔。这个 Skill 的核心任务就是捕捉这种**生活里的俏皮瞬间**。

核心公式：

```
毛笔线条 + 简笔人物 + 留白 + 手写题字 + 生活趣味
```

## 风格特征

| 维度 | 淡彩模式 | 纯黑白模式 |
|------|----------|------------|
| **线条** | 毛笔软锋，有飞白和浓淡变化 | 同左，层次更依赖墨色 |
| **色彩** | 墨色 + 极淡赭石/花青/藤黄 | 只有墨的浓淡四层 |
| **人物** | 3-6 笔勾勒，无五官 | 同左 |
| **留白** | 40%-60% | 同左，意境更空远 |
| **题字** | 手写行书，字大小不齐 | 同左 |
| **印章** | 1-2 个朱红 | 黑白画里唯一的颜色 |
| **情绪** | 温暖、俏皮、诗意 | 哲思、寂静、怀旧 |

## 安装

```bash
# 推荐：一行安装
npx skills add Mengbooo/fengzikai-illustration

# 或手动克隆到 Agent skills 目录
git clone https://github.com/Mengbooo/fengzikai-illustration.git ~/.claude/skills/fengzikai-illustration
```

## 兼容平台

| 平台 | 安装命令 |
|------|----------|
| **Claude Code** | `npx skills add Mengbooo/fengzikai-illustration` |
| **Codex CLI** | `npx skills add Mengbooo/fengzikai-illustration` |
| **Hermes Agent** | `npx skills add Mengbooo/fengzikai-illustration` |
| **Cursor** | `npx skills add Mengbooo/fengzikai-illustration` |
| **其他 71 个 Agent** | 同上 |

## 使用方式

触发词：
- "丰子恺风格，给这段文字配图"
- "水墨淡彩，画一个人喝茶看月亮"
- "**黑白水墨**，画雪夜独行" ← 纯黑白模式
- "用丰子恺的风格，题字'谁偷了我的枇杷'"

---

## 文件结构

```
.
├── SKILL.md                 # Skill 主文件
├── README.md
├── LICENSE                  # MIT
├── skills.sh.json
├── references/
│   ├── style-dna.md         # 风格DNA
│   ├── prompt-template.md   # 生图模板（含黑白模式）
│   ├── story-extraction.md   # 故事提炼
│   ├── master-selection.md   # 母版系统
│   └── qa-checklist.md       # QA清单
└── assets/examples/          # 参考母版图（待补充）
```

---

## 许可

MIT
