# 生图提示词模板

**最关键的规则：这是墨笔画，不是彩色画。只有黑色墨、灰色墨、纸的暖白。没有其他颜色。**

---

## 淡彩模式

```text
BLACK INK DRAWING on warm paper, in the naive style of FENG ZIKAI. This is NOT a colorful illustration. The entire drawing uses ONLY black ink and grey ink wash. No warm colors, no peach, no beige tones in the artwork itself. The paper is warm off-white — that is the ONLY warmth in the image.

Drawn like a child with a brush: clumsy wobbly lines, simple shapes. A figure made of 4-6 strokes (circle head, curved body, stick limbs). No face. Proportions slightly wrong — good.

Scene: {一句话，如 a person sitting under a tree reading}

The drawing has very few elements. 50%+ of the canvas is empty paper. 

Color rule — CRITICAL: the ENTIRE image uses black ink (for lines), grey ink wash (for one or two light areas), and warm paper color (#F0E8D8). Optionally ONE tiny touch of pale color in one spot — and ONLY if the user explicitly wants color mode. Otherwise: black, grey, paper. One small red seal stamp.

Hand-brushed calligraphy: {题字}. Uneven, childlike handwriting, slightly tilted.

DO NOT: colorful illustration, warm peach tones, beige washes, multiple colors, gradient backgrounds, detailed brushwork, facial features, complex composition, filled canvas, professional calligraphy, polished lines.
```

---

## 纯黑白模式

```text
PURE BLACK INK DRAWING on warm paper, naive Feng Zikai style. ONLY black ink, grey ink wash, and paper color. NO color of any kind — no warm washes, no peach, no beige, no blue, no green. One small red seal stamp is the only exception.

Clumsy childlike brush strokes. Simple shapes. A figure: 4-6 strokes, no face. 

Scene: {一句话}

Over half the canvas is empty paper. Very few elements. 

Hand-brushed calligraphy: {题字}. Uneven, childlike. One red seal.

DO NOT: any color except the seal, warm-toned illustration, complex composition, professional lines, facial features.
```

---

## 提示词组装清单

只填这三样，不要加任何东西：

- [ ] 一句话场景（10 字内）
- [ ] 题字（3-8 字）
- [ ] 淡彩还是纯黑白？
