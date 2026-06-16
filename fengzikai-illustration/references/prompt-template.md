# 生图提示词模板

每张图单独生成。根据当前内容替换变量，不要把多张拼在一起。

## LoRA 参数参考（使用 CivitAI 丰子恺 LoRA 时）

- 触发器词: `FENG ZIKAI`
- CLIP strength: 0.8-0.9
- Model strength: 0.8-0.9
- CFG scale: ~6.0
- ⚠️ CFG 不宜过高——6.0 以上颜色会变饱和、偏卡通，丧失水墨淡彩质感

---

## 标准模板（竖版 3:4）

```text
Generate one standalone vertical illustration in the style of FENG ZIKAI (丰子恺), the renowned 20th century Chinese painter and cartoonist.

Core visual DNA:
Traditional Chinese ink wash painting (水墨画) with light color washes (淡彩). Hand-drawn with a soft calligraphy brush. Simple, expressive line work with natural variation in thickness — not uniform digital strokes. The entire image feels like a painting on warm-toned xuan paper (宣纸), with subtle paper fiber texture. Background is warm off-white close to #F5F0E8 or #FAF6EE — NOT pure digital white #FFFFFF, NOT grey, NOT cold white.

Composition & proportion:
Vertical 3:4 format. Generous negative space — 50% to 70% of the canvas is empty (the paper itself). Subject matter occupies the middle-lower portion of the frame. The composition breathes. Elements are sparse and intentional. Not crowded, not busy, not filled.

Brushwork & line quality:
Soft ink brush lines (毛笔线条) with visible variation in thickness — thicker at turns, thinner in motion. Lines feel alive, not mechanical. Figures drawn with 3-5 simple brush strokes: a dot for the head, two arcs for the body, one stroke for limbs. NO facial features — faces are blank or have a single ink dot for hair. NO anatomical detail, NO realistic proportions. Expressiveness comes from body posture and line rhythm alone.

Color palette — extremely restrained:
- Main lines: warm ink black (#2C2C2C to #1A1A1A)
- Distant elements: light ink grey (#8A8A8A to #B0B0B0)
- Light color washes (transparent, barely-there, brushed on over ink lines):
  - Pale umber (淡赭石): for clothing, tree trunks, ground hints
  - Pale indigo (花青): for distant mountains, water surface, garment folds
  - Pale gamboge (藤黄): for moonlight, flower centers
  - Pale vermilion (淡朱砂): ONLY for seal stamps and tiny flower dots
- NO saturated colors. NO bright red, NO vivid yellow, NO electric blue, NO emerald green.
- Color washes are loose brushstrokes with soft edges, NOT flat fills.

Scene:
{具体场景描述，例如："两个人坐在竹椅上喝茶，窗外柳枝轻垂"}

Figures:
{人物描述，例如："两个人，一左一右对坐。左边穿长衫，右手举茶杯；右边微微侧身倾听。简笔勾勒，无五官。"}
- Drawn with 3-5 strokes per person
- No facial features (blank faces)
- Simple, flowing clothing lines
- Posture conveys mood, not anatomical precision

Nature elements:
{自然元素，例如："上方垂下 3-4 条柳枝，远山淡影一抹，地面淡赭石薄涂"}

Handwritten calligraphy (题字):
{题字内容，例如："人散后，一钩新月天如水"}
- Position: upper-right or upper-left corner
- Vertical (top-to-bottom) or horizontal single line
- Hand-brushed kaishu (楷书) or xingshu (行书) style — natural, slightly irregular, clearly hand-written
- NOT printed font, NOT typeset, NOT sans-serif, NOT bold display type
- Characters should feel like they were written with the same brush as the painting

Red seal stamp (印章):
- 1 or 2 small square red seal marks in vermilion (#C04040 to #A03030)
- Position: below the calligraphy text OR in one bottom corner
- Size: about 1/20 to 1/15 of image width
- Ancient seal script style (篆书), small and understated

Negative constraints — DO NOT include:
- NO electronic devices (phones, laptops, headphones, tablets)
- NO modern clothing (suits, T-shirts, sneakers, baseball caps)
- NO modern architecture (glass buildings, concrete, neon signs)
- NO vehicles (cars, planes, subways)
- NO logos, QR codes, brand elements
- NO speech bubbles, dialog boxes
- NO infographic elements, step numbers, arrows, charts
- NO saturated or bright colors
- NO pure white or pure black large areas
- NO 3D rendering, vector flat style, digital illustration feel
- NO detailed facial features on people
- NO realistic anatomy or proportions
- NO Western objects (coffee cups, wine glasses, smartphones)
- NO complex backgrounds with excessive detail
- NO filled compositions — must have 50-70% empty space
- NO filters, vignettes, lens effects, digital post-processing
```

---

## 横版变体（16:9，适合广阔场景）

将标准模板中的比例描述替换为：

```text
Horizontal 16:9 format. Generous negative space — 50% to 65% of the canvas is empty. Subject matter occupies the lower third of the frame, with vast sky/air above. The composition feels open, breathable, like a wide scroll partially unrolled.
```

---

## 方版变体（1:1，适合对称/庭院）

将标准模板中的比例描述替换为：

```text
Square 1:1 format. Generous negative space around the central subject — 45% to 60% empty. Subject placed slightly below center. Balanced, meditative composition. The square format recalls traditional Chinese album leaves (册页).
```

---

## 极简变体（封面感、强留白）

用于需要极强留白、一句题字主导画面的场景：

```text
Ultra-restrained Feng Zikai style variant. Keep one figure, one nature element, and 4-8 character calligraphy. 70%+ empty space. The calligraphy carries the emotional weight. The painting is a whisper, not a statement. Muted to the edge of monochrome — only ink black, light grey wash, and one tiny red seal for color.
```

---

## 提示词组装清单

每次生成前确保以下所有变量已填充：

- [ ] 比例（竖 3:4 / 方 1:1 / 横 16:9）
- [ ] 场景描述（一句话）
- [ ] 人物数量、姿态、关系
- [ ] 自然元素（至少 1 个，最多 3 个）
- [ ] 题字内容（3-12 字）
- [ ] 印章位置
- [ ] 淡彩色调（选了哪 2-3 种淡彩）
- [ ] 母版锁定（用了哪张参考母版，做了哪些变异）
