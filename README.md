# Job Hunter / 求职匠 — Brand Book

> 这是一个 **UI 规范 / 品牌手册**，不是产品代码。
> 双击 `index.html` 就能看，不需要 npm install / 不需要 build。

---

## 目录结构

```
job-hunter/
├── index.html              ← 品牌手册（16 sections，双击打开就能看）
├── DESIGN.md               ← 完整设计规范（13 节）
├── _source_design.md       ← 原始设计研究稿（存档）
├── tokens/
│   ├── tokens.json         ← Design tokens 源数据（W3C 格式）
│   └── tokens.css          ← CSS Variables（--jh-*），任何项目 import 即可用
└── assets/
    ├── logo/               ← Logo 5 件套（TODO）
    ├── mascot/
    │   └── spec-sheet.png  ← ChatGPT spec 原图
    ├── cards/              ← 6 张卡片插图（TODO）
    ├── banners/            ← Hero banner（TODO）
    ├── stickers/           ← 装饰贴纸（TODO）
    └── decorations/        ← 装饰素材（TODO）
```

---

## 用法

### 看规范
双击 `index.html` 浏览器打开。16 个 section：
Brand / Colors / Typography / Mascot / Buttons / Inputs / Chips / Icons / Navigation / Cards / Alerts / Progress / Modal / Sample Modules / Banner / Spacing & Shadow + Principles + QR.

### 读设计决策
`DESIGN.md` — 完整 13 节规范，包含：
- 品牌定位（vs LinkedIn / Seek / 实习僧）
- Mascot 8 状态决策树
- 用色决策树 + 匹配度色逻辑
- 组件规范（buttons / inputs / 6 种卡 / alerts ...）
- Voice & Tone（专业 + 鼓励 + 行动导向）
- **跟 UniMate AI / Cert Master 的三方隔离规则**

### 在产品里用 tokens

```css
/* 任何 CSS 文件顶部 */
@import url('path/to/job-hunter/tokens/tokens.css');

.my-cta {
  background: var(--jh-grad-primary);  /* Periwinkle 蓝渐变 */
  color: white;
  border-radius: var(--jh-radius-full);
  box-shadow: var(--jh-shadow-blue-glow);
  padding: 0 var(--jh-space-6);
  height: 48px;
  font-weight: 700;
}
```

CSS 前缀 `--jh-*` 跟 `--um-*` / `--cm-*` 完全隔离，三个品牌可同 import。

### 在 Style Dictionary / Figma 里读

`tokens/tokens.json` 是 [W3C Design Tokens 格式](https://design-tokens.github.io/community-group/format/)。

---

## 品牌 DNA（一句话）

> **Warm Professional Blue** — LinkedIn × Canva × Linear × Airbotix × JR Academy Mascot.
> 让求职这件焦虑的事，变得清楚、有步骤、有反馈、有陪伴。

四条不可妥协：**暖白底 `#FFFEF7` · Periwinkle CTA · 求职牛 IP · 大数字驱动**。

---

## 红线（看到立即打回）

- ❌ 大块 `bg: #FFFFFF`（必须暖白 `#FFFEF7`）
- ❌ 银行 / 政府那种深蓝（保持 Periwinkle `#5F7CFB`）
- ❌ 求职牛去掉墨镜（家族识别核心）
- ❌ 出现企鹅 / 考证黄 / UniMate Coral（混到其它品牌）
- ❌ 自创新 mascot 表情（只用 8 标准态）
- ❌ Caveat 手写体（那是 UniMate 的）
- ❌ "您 / 智能化 / Deadline 战神"

---

## Mascot 8 个标准态

| State | 中文 | 触发场景 |
|-------|------|---------|
| analyzing | 分析中 | JD 分析 loading |
| interview-prep | 面试准备 | 题库练习 |
| resume-edit | 修改简历 | 简历优化 |
| offer | 拿到 Offer | 通过 / 庆祝 |
| thinking | 思考中 | 空状态 / loading |
| cheering | 加油中 | streak / 鼓励 |
| company-research | 公司研究 | 公司洞察 |
| networking | 人脉拓展 | 人脉 / AI 起草 |

新场景必须 map 到已有 8 态，**禁止自创**。

---

## 待补 (TODO)

- [ ] Logo 5 件套（horizontal / compact / avatar / app-icon / app-icon-ios）
- [ ] 8 个求职牛 mascot（黑白卡通 + 墨镜 + 西装 + 公文包）
- [ ] 6 张卡片插图（Job / Company / Interview / Progress / Profile / Salary）
- [ ] Hero banner 主图（spec 风的渐变 + 求职牛）
- [ ] Style Dictionary 配置 — 输出 Tailwind preset / iOS / Android

---

## Deploy

GitHub Pages auto-deploy via `.github/workflows/deploy.yml` — push to `main` 自动构建并发布。

---

## 维护

- 源 spec 图：`assets/mascot/spec-sheet.png`（ChatGPT 2026-05-11）
- 原始设计稿：`_source_design.md`
- 最近更新：2026-05-12

任何 token 改动必须**三处同步**：`DESIGN.md` → `tokens.json` → `tokens.css`。
冲突时以 `DESIGN.md` 为准。
