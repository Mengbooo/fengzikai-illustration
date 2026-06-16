# 生图提示词模板

核心原则：**提示词越短越好**。长提示词会让 AI 过度渲染，画出一张"太像样"的画。丰子恺只需要一句话说清楚。

---

## 淡彩模式

```text
A simple, naive Chinese ink brush drawing in the style of FENG ZIKAI (丰子恺). It should look like a child drew it with a brush — clumsy, sincere, unpolished.

The drawing has only a few brush strokes total. Wobbly, uneven lines. A figure drawn with 4-6 strokes: a rough circle head, a curved body line, two stick legs, one or two arm lines. No facial features. Proportions are slightly off — that's good.

Only one thing is happening in the scene: {一句话场景，如 "a person sitting under a tree reading"}

Warm off-white paper background, not pure white. Lots of empty space — over half the canvas is blank.

Barely any color — just black ink with maybe ONE pale wash of {淡赭石 或 花青} in one small area. Hand-brushed calligraphy in the corner: {题字}. The writing is casual, uneven — like a child's handwriting. One small red seal stamp.

DO NOT: detailed brushwork, controlled lines, complex composition, multiple objects, rich colors, facial features, professional calligraphy, filled canvas.
```

---

## 纯黑白模式

```text
A simple, naive Chinese ink brush drawing in the style of FENG ZIKAI (丰子恺). It should look like a child drew it — clumsy, sincere, black ink only.

Only a few brush strokes total. Wobbly, uneven lines. A figure with 4-6 strokes: rough circle head, curved body, stick legs, arm lines. No facial features. Slightly wrong proportions.

Only one thing happening: {一句话场景}

Warm off-white paper. Over half the canvas is empty. Pure black ink with one pale grey wash for ground or distant elements. No color at all — except one small red seal stamp. Hand-brushed uneven calligraphy: {题字}.

DO NOT: color, detailed brushwork, multiple objects, complex composition, facial features, professional calligraphy, filled canvas.
```

---

## 提示词组装清单

生成前只填这些，不要加更多：

- [ ] 一句话场景（10 字以内，如"树下看书""两人喝茶""小孩追蝴蝶"）
- [ ] 题字（3-8 字）
- [ ] 淡彩还是纯黑白？
- [ ] 如果淡彩：唯一一抹颜色是什么？（淡赭石/花青，只选一个）

**不要填的**：
- ❌ 不要详细描述人物姿态（"微微侧身""手指微曲"——太细）
- ❌ 不要列举自然元素（"柳枝、燕子、远山、桃花"——太多）
- ❌ 不要描述光影和氛围
- ❌ 不要重复风格约束（负面约束在模板里已经够了）
