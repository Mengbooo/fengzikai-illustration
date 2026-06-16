# 丰子恺水墨插图 / Feng Zikai Ink-Wash Illustration

> 把中文内容里的情绪、观点和哲理，变成一张有温度的丰子恺水墨风格配图。
>
> 竖版 3:4 配图 | 水墨淡彩 | 简笔人物 | 手写题字 | 兼容 Claude Code / Codex / Hermes

---

## 这是什么

丰子恺水墨插图是一个 AI Agent Skill，用来指导 AI 为中文文章、帖子、课程、随笔、哲理短文生成丰子恺（1898-1975）风格的配图。

它不是通用插画 prompt，也不是商业插画模板。核心目标是：**把一段文字的抽象情绪，变成一个可看见的生活场景——像丰子恺那样，用三笔两笔画出生活本身的诗意。**

核心公式：

```
简笔人物 + 水墨淡彩 + 大面积留白 + 手写题字 + 生活诗意
```

一句话：**让读者先感受到一种安静、温暖、有诗意的画面，再在一秒内被题字点出文章的核心情绪。**

---

## 丰子恺风格特征

| 维度 | 规则 |
|------|------|
| **线条** | 毛笔软锋，粗细变化，起笔收笔有顿挫 |
| **色彩** | 极其克制——墨黑 + 2-3 种极淡水彩色（淡赭石、花青、藤黄） |
| **人物** | 简笔——3-5 笔勾勒，无五官，无解剖结构 |
| **留白** | 画面 50%-70% 为空，主体偏下或一侧 |
| **背景** | 暖白宣纸色（`#F5F0E8`），不是纯白 `#FFFFFF` |
| **题字** | 手写毛笔字，3-12 字，一句诗或白话哲理 |
| **印章** | 1-2 个朱红色小方章 |
| **场景** | 喝茶、望月、散步、读书、柳下、舟中、庭前、窗边 |

---

## 兼容平台

本 Skill 遵循 **Agent Skills 开放标准**，可在以下平台使用：

| 平台 | 安装路径 |
|------|----------|
| **Claude Code** | `.claude/skills/fengzikai-illustration/` |
| **Codex CLI** | `~/.codex/skills/fengzikai-illustration/` |
| **Hermes Agent** | `~/.hermes/skills/fengzikai-illustration/` |
| **Cursor** | `.cursor/skills/fengzikai-illustration/` |
| **其他兼容 Agent Skills 的平台** | 按平台约定路径 |

### 安装方式

**方式一：直接克隆**
```bash
# 在你的 Agent skills 目录下克隆
cd ~/.claude/skills/     # 或 ~/.codex/skills/ 或 ~/.hermes/skills/
git clone https://github.com/Mengbooo/fengzikai-illustration.git
```

**方式二：只复制 skill 目录**
```bash
git clone https://github.com/Mengbooo/fengzikai-illustration.git /tmp/fengzikai
cp -r /tmp/fengzikai/fengzikai-illustration ~/.claude/skills/
```

---

## 使用方式

在任何兼容 AI Agent 中输入触发词即可：

- "给这篇文章配一张丰子恺风格的图"
- "水墨淡彩风格，画一个人喝茶看月亮"
- "丰子恺风，题字写'春风又绿江南岸'"
- "用丰子恺的风格，为这段文字配图"

AI Agent 会自动加载 SKILL.md 中的完整流程：消化内容 → 提炼情绪 → 选择母版 → 生成配图 → QA 检查。

---

## 文件结构

```
fengzikai-illustration/
├── README.md                           # 仓库说明（本文件）
├── LICENSE                             # MIT 许可证
├── NOTICE.md                           # 署名声明
├── examples/images/                    # 母版参考图（待补充）
└── fengzikai-illustration/            # Skill 主目录
    ├── SKILL.md                        # Skill 主文件（Agent Skills 标准）
    ├── assets/examples/                # 母版参考图（待补充）
    └── references/                     # 参考文档
        ├── style-dna.md                # 风格DNA：色彩、线条、留白、题字规则
        ├── prompt-template.md          # 生图提示词模板
        ├── story-extraction.md         # 故事提炼：五步法
        ├── master-selection.md         # 母版系统：01-06 号母版
        └── qa-checklist.md             # 质量检查清单
```

---

## 适合谁用

- 写中文文章，需要正文配图的内容创作者
- 做 AI 课程、教程、知识付费的创作者
- 想把哲理、观点、生活感悟画出来的人
- 想要一种有温度、有辨识度的中国画风配图风格的人
- 用 AI Agent（Claude Code / Codex / Hermes）做内容生产的人

## 不适合

- 需要技术信息图、架构图、流程图的人（用 Excalidraw、Mermaid）
- 需要商业海报、品牌 KV 的人
- 需要写实插画、3D 渲染的人
- 需要英文配图的人（丰子恺风格深度绑定中文语境）

---

## 参考资源

- [CivitAI Feng Zikai LoRA](https://civitai.com/models/186722/artist-style-lora-feng-zikai) — 触发词 `FENG ZIKAI`
- [Pinterest 丰子恺插画](https://www.pinterest.com/b020521285/%E8%B1%90%E5%AD%90%E6%84%B7%E6%8F%92%E7%95%AB/) — 152 张原作参考

---

## 许可

MIT License — 详见 [LICENSE](./LICENSE)
