# 生图提示词模板

每张图单独生成。根据正文内容替换变量，不要把多张图拼在一起。`{RATIO}` 必须换成用户选定的画幅描述（例如 "16:9 horizontal" / "1:1 square" / "3:4 vertical" / "9:16 vertical"）。

```text
Generate one standalone {RATIO} Chinese article illustration in soft watercolor hand-drawn style.

Visual DNA:
Cream-white / off-white background with subtle watercolor paper warmth, no busy texture, no harsh shadows. Soft transparent watercolor washes, gentle edges, slightly visible watercolor bleed. Lots of clean empty space, at least 35% blank. Warm color palette: soft yellow, warm cream, light gold, blush pink, mint or pale blue accents. No vector flat design, no bold black outlines, no PPT infographic, no 3D render, no realistic UI, no dark or gloomy mood.

Recurring IP character required:
冷檬 (Lengmeng), a chibi little girl about 2.5 head-to-body ratio. Soft light-gold / milky-blonde hair in two round double-bun hairstyles, each bun decorated with a small bright-yellow five-petal flower hair accessory; wispy bangs and loose side strands. Big round grey-blue eyes with long lashes, rosy cheeks, small focused mouth. Wearing a bright yellow puff-sleeve dress with white lace ruffle collar, white lace cuffs, and multi-layer white lace hem. White lace-trimmed ankle socks, black shiny Mary Jane shoes. Soft watercolor rendering. She must be the one doing the core action in the scene — holding, watering, sorting, pushing, opening, reaching, writing — not just standing as a mascot.

Theme:
{正文配图主题}

Structure type:
{结构类型：流程闭环 / 前后对比 / 角色状态 / 概念隐喻 / 方法分层 / 路径地图 / 小场景叙事}

Core idea:
{这张图要表达的核心意思}

Composition:
{具体画面：冷檬在哪里、正在做什么、主要物件是什么、信息如何流动}

Suggested elements:
{元素1} / {元素2} / {元素3}

Chinese handwritten labels (short, warm brown / soft dark grey handwritten style):
{标注词1} / {标注词2} / {标注词3} / {可选标注词4}

Color use:
Warm yellow as the main character dress and key emotional color. Soft blush pink, mint, pale blue only as tiny accents. Cream background. Keep it gentle and transparent.

Constraints:
One image explains only one core idea. Keep the main subject around 40%-60% of the canvas. Preserve generous blank space. At most 4-6 short handwritten Chinese labels, 2-8 characters each. Do not write a title in the top-left corner. Do not write the structure type on the image. No dense diagram, no course slide, no cute sticker collage. Keep Lengmeng's hairstyle, hair color, and yellow lace dress exactly as described. It should feel warm, healing, and gently narrative — like a girl quietly explaining an idea to you through watercolor.
```

## 图像编辑提示

去掉左上角标题：

```text
Edit the provided image. Remove only the handwritten title "{要删除的文字}" and any underline from the top-left corner. Fill that area with the same clean cream-white watercolor background, matching the surrounding tone. Preserve everything else exactly: Lengmeng, her pose and outfit, labels, props, soft watercolor style, composition, and aspect ratio. Do not add any new text or objects.
```

纠正冷檬形象（发色/服装走样时）：

```text
Regenerate this image with the same scene and composition, but make the character 冷檬 strictly match: light-gold double buns with small yellow flower accessories, grey-blue big eyes, bright yellow puff-sleeve dress with white lace ruffles, black Mary Jane shoes. Keep the soft watercolor style, warm cream background, and all props and labels. Do not change her into an adult, a different hairstyle, or different clothing.
```

太像 PPT / 太满：

```text
Regenerate with the same core meaning. Remove extra nodes, arrows, and labels. Keep only Lengmeng doing one clear action and 3-4 short handwritten labels. Add more blank cream space. Keep it soft watercolor and gentle, like a quiet illustration.
```
