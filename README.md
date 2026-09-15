# 冷檬配图 Skill（lengmeng-illustrations）

生成冷檬风格的中文正文配图。固定 IP 是「冷檬」——一个金色双丸子头、穿黄色蕾丝连衣裙的水彩软萌 Q 版小女孩。

## 冷檬形象

![冷檬形象参考](https://aka.doubaocdn.com/s/9KrOQP0A9V)

浅金双丸子头配黄色小花发饰，灰蓝大眼，明黄蕾丝连衣裙，黑玛丽珍鞋，柔和水彩风。

## 核心特点

- **先问尺寸再生图**：用户发文案后，第一步强制确认画幅（16:9 / 1:1 / 3:4 / 4:5 / 9:16 / 自定义），用户答复前不调生图。
- **冷檬必须做核心动作**：不是站桩卖萌，而是浇水、分类、推门、贴标签等具体动作。
- **水彩暖黄治愈风**：奶油白底、柔和水痕、明黄主色，区别于黑白怪诞线稿。
- **一张图只讲一个结构**：大量留白，少量暖棕手写中文标注。

## 安装

把本仓库克隆或下载到你的 `~/.user_skills/` 目录下：

```bash
git clone https://github.com/1162711644/lengmeng-illustrations.git ~/.user_skills/lengmeng-illustrations
```

然后把冷檬参考图下载到 `assets/coldmeng-character-ref.jpg`（可直接保存上方预览图）。

## 文件结构

```
lengmeng-illustrations/
├── SKILL.md                        # 主流程（含强制第一步：问尺寸）
├── assets/
│   └── coldmeng-character-ref.jpg   # 冷檬参考图（需自行放置）
└── references/
    ├── style-dna.md                # 水彩暖黄配色、留白、禁忌
    ├── lengmeng-ip.md              # 冷檬外形/性格/动作库
    ├── composition-patterns.md     # 结构类型 + 软萌物件/动作池
    ├── prompt-template.md          # 生图提示词（含尺寸变量）
    └── qa-checklist.md             # 出图后检查与迭代
```

## 使用流程

1. 用户发来文案。
2. Skill 先问配图画幅尺寸。
3. 用户答复后，消化正文并给出 shot list（3-6 张）。
4. 用户确认后，逐张用 `image_gen` 单独生成。
5. 按 QA 清单检查，必要时局部编辑。
6. 保存到 `assets/<article-slug>-illustrations/`。

## License

MIT
