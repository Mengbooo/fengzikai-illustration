# 生图提示词模板

每张图单独生成。选择淡彩或纯黑白模板，根据当前内容替换变量。

---

## 淡彩模式（默认）

```text
Generate one standalone illustration in the style of FENG ZIKAI (丰子恺), the 20th century Chinese painter-cartoonist known for warm, playful, poetic ink-wash vignettes of everyday life.

CORE IDENTITY:
This is NOT a polished "Chinese-national-style illustration." Feng Zikai's work is casual, warm, sometimes funny — a person who noticed the small, absurd, tender moments of daily life and jotted them down with a brush. The drawing should feel like a spontaneous sketch, not a finished masterpiece.

COMPOSITION & FORMAT:
{竖版3:4 / 方版1:1 / 横版16:9}. Generous negative space — 40-60% of the canvas is empty xuan paper. Subject placed in the middle-lower portion, off-center. The composition breathes.

BRUSHWORK — THIS IS THE MOST IMPORTANT PART:
Hand-brushed ink lines with visible life:
- Lines have natural thick-thin variation from brush speed changes — fast sweeps are thin, slow turns are thick
- Ink density varies: dark ink for figures and foreground, medium ink for mid-ground, pale ink for distant elements
- Visible "flying white" (飞白) where the brush splits and paper shows through — this is essential for hand-drawn feel
- Stroke beginnings have a small rounded stop (where the brush first touched paper); stroke ends taper naturally
- Lines are NOT uniform, NOT vector-perfect, NOT digital-stroke — minor wobbles and imperfect connections are intentional
- Do NOT use even-width hard pen lines, technical pen lines, or bezier-perfect curves

PAPER:
Warm off-white xuan paper background close to #F5F0E8, with subtle paper fiber texture. NOT pure white #FFFFFF.

FIGURES:
Drawn with 3-6 simple brush strokes per person: a dot or small circle for the head, 1-2 curved strokes for the body, single strokes for limbs. NO facial features — the face is blank. Emotion comes from body angle and posture. Slight proportional exaggeration is welcome (larger head on a child, rounded back on an elder) — this adds charm, not anatomical precision.

{人物描述}

COLOR — extremely restrained, "color washed three times in water":
- Dark ink (#1A1A1A-#2C2C2C): figure outlines, foreground lines, calligraphy
- Medium ink (#4A4A4A-#6A6A6A): secondary lines, tree trunks
- Pale ink (#8A8A8A-#A8A8A8): distant mountains, ground wash, water
- Color washes (barely-there translucent watercolor brushed loosely over ink lines):
  - Pale umber (淡赭石): clothing, tree trunks, ground hints — soft-edged wash
  - Pale indigo (花青): distant mountains, water surface, garment shadows
  - Pale gamboge (藤黄): moonlight glow, flower centers
  - Vermilion (朱砂): ONLY for the seal stamp(s) and tiny flower dots — the one slightly saturated color
- NO saturated colors. NO bright red, vivid yellow, electric blue, emerald green.
- Color washes are loose wet brushstrokes with soft diffused edges, not flat fills.

SCENE — a specific life moment, not a concept poster:
{场景，必须是具体的"瞬间"而非抽象概念}

CALLIGRAPHY (题字) — THIS IS CRITICAL:
Hand-brushed casual running script (行书偏行楷), written with the same ink as the painting:
- Characters are naturally irregular in size — the first character may be larger than the third
- Stroke connections are casual, some strokes may be slightly abbreviated
- The writing feels like a friend's quick note in the margin, NOT an exhibition-level calligraphy piece
- Position: upper-right or upper-left corner, slightly tilted — not perfectly aligned to a grid
- Content: {题字内容，3-12字}
- Vertical (top-to-bottom) or single horizontal line
- NOT typeset, NOT sans-serif, NOT bold display font, NOT formal kaishu (楷书) from a calligraphy manual, NOT wild cursive (狂草)

RED SEAL(S):
1-2 small square vermilion seal marks (#C04040-#A03030), vintage seal script style. Placed below the calligraphy or in a bottom corner. Size about 1/20 to 1/15 of image width.

NATURAL ELEMENTS:
{自然元素，1-3个}

NEGATIVE CONSTRAINTS:
NO electronic devices, NO modern vehicles, NO modern architecture, NO logos or QR codes, NO saturated colors, NO pure white background, NO even-width digital lines, NO vector/flat illustration style, NO 3D rendering, NO facial features on figures, NO printed/typeset text, NO speech bubbles, NO infographic elements, NO formal calligraphy, NO stiff "national style" polish.
```

---

## 纯黑白模式

当用户说"黑白""水墨单色""纯墨色""不要颜色"时，使用此模板。仅替换色彩描述部分：

```text
{保留淡彩模板中"COMPOSITION"到"CALLIGRAPHY"之间的所有内容，仅替换 COLOR 段落为：}

INK-ONLY PALETTE (纯墨色):
This image uses ONLY ink — no color washes at all.
- Dark ink (#1A1A1A-#2C2C2C): figures, foreground lines, calligraphy, tree trunks
- Medium ink (#4A4A4A-#6A6A6A): secondary lines, mid-ground elements
- Pale ink (#8A8A8A-#A8A8A8): distant mountains, ground wash, water ripples
- Very pale ink (#C8C8C8-#D8D8D8): furthest mountains, atmospheric haze
- The ONLY color allowed is the red seal stamp(s) — vermilion (#C04040-#A03030), 1-2 small square seals
- Rich ink layering replaces color: use wet-dark for depth, dry-pale for distance
- NO umber, NO indigo, NO gamboge — depth comes from ink density alone
- The mood is contemplative, quiet, wintery or nostalgic
```

---

## 提示词组装清单

每次生成前确认：

- [ ] 淡彩还是纯黑白？
- [ ] 比例（竖 3:4 / 方 1:1 / 横 16:9）
- [ ] 场景是"瞬间"不是"概念"？
- [ ] 人物姿态能传情绪？
- [ ] 题字有"随手写"感？
- [ ] 线条描述强调了浓淡变化和飞白？
- [ ] 自然元素 1-3 个，不堆砌？
