# Job Hunter / 求职匠 — Design System

> **完整设计规范文档**。目标读者：Claude / 设计师 / 前端 / 内容运营。
> 任何关于「该用什么色、什么字、什么 mascot、什么按钮」的问题，先来这里查。
>
> 配套文件：
> - `index.html` — 视觉品牌手册（双击就能看）
> - `tokens/tokens.json` — W3C Design Tokens 源数据
> - `tokens/tokens.css` — `--jh-*` CSS 变量
> - `README.md` — 仓库使用说明
> - `_source_design.md` — 原始设计研究稿（保留作存档）
>
> Last updated: 2026-05-12 · v0.1

---

## 目录

1. [品牌定位](#1-品牌定位)
2. [品牌 DNA](#2-品牌-dna)
3. [Mascot 系统](#3-mascot-系统)
4. [Color 系统](#4-color-系统)
5. [Typography 系统](#5-typography-系统)
6. [Spacing · Radius · Shadow](#6-spacing--radius--shadow)
7. [Logo & Banner](#7-logo--banner)
8. [组件规范](#8-组件规范)
9. [Voice & Tone](#9-voice--tone)
10. [Motion](#10-motion)
11. [Do / Don't 红线](#11-do--dont-红线)
12. [Asset 目录映射](#12-asset-目录映射)
13. [跟 UniMate AI / Cert Master 的隔离规则](#13-跟-unimate-ai--cert-master-的隔离规则)

---

## 1. 品牌定位

**Job Hunter / 求职匠** — 全球华人求职者的 AI 求职助手。

| 维度 | 内容 |
|------|------|
| **一句话** | 你的 AI 求职助手 — 帮你分析 JD、优化简历、准备面试、追踪投递进度 |
| **English** | Your AI job search assistant for smarter applications, better interviews, and faster offers. |
| **场景** | JD 分析 / 简历优化 / 面试准备 / 公司研究 / 投递追踪 / 薪资洞察 / 人脉管理 |
| **目标用户** | **毕业生、转行者、留学求职者**（澳新加美英华人优先），尤其是 IT / 金融 / 商科 |
| **竞品对标** | LinkedIn (招聘平台) · Seek (本地求职) · ChatGPT (通用) · 实习僧 (国内) |
| **核心差异** | **澳洲华人求职场景** + **全流程 AI 陪伴**（不是单点工具）+ **求职牛 IP** |
| **母品牌** | JR Academy (匠人学院) — 跟 UniMate AI / Cert Master / SigmaQ 同属一家 |

### 产品关系（三角架构）

| Product | Audience | Core Scenario | Visual Mood |
|---------|----------|---------------|-------------|
| **UniMate AI / 牛小匠** | 大学生 / 留学生 | 课程 / 复习 / AI 课代表 | Warm Coral · Playful Study Companion |
| **Cert Master / 考证匠** | 考证人 (在职+应届) | 注会 / 一建 / 法考 等证书 | Yellow · Professional 备考 |
| **Job Hunter / 求职匠** ← | **求职者 / 毕业生 / 转行者** | **求职全流程** | **Warm Blue · Professional Career** |

### 不做什么

- 不做"代写简历 / 代投简历"（违反平台规则）
- 不做"代面试 / 替身考"（同理）
- 不做线下中介 / 内推服务（线上 AI 是核心）
- 不做纯招聘平台（不抢 LinkedIn / Seek 的活）

---

## 2. 品牌 DNA

### 一句话
**Warm Professional Blue** — 让求职这件焦虑的事情，变得清楚、有步骤、有反馈、有陪伴。

### 设计北极星

UI 必须帮用户秒懂以下问题：

1. 这个职位值不值得投？
2. 我的匹配度是多少？
3. 简历哪里需要优化？
4. 面试该准备什么？
5. 我当前投递进度如何？
6. **下一步该做什么**？

### 视觉对标

> **LinkedIn × Canva × Linear × Airbotix × JR Academy Mascot**

**不要像**：
- 冷冰冰的 SaaS Dashboard
- 企业 CRM / ATS 后台
- 传统招聘网站
- 过度卡通的儿童产品
- 金融产品

### 四条不可妥协（看到就打回）

| 铁律 | Why |
|------|-----|
| **暖白底 `#FFFEF7`** 做大块页面 bg，绝不纯白 | 跟 UniMate 同族暖白 — 避免 SaaS 冷感 |
| **Periwinkle 蓝 `#5F7CFB`** 做主 CTA，绝不深蓝 / 企业蓝 | 长春花蓝 = 专业 + 年轻 + 记忆点；深蓝 = 银行 / 政府 |
| **求职牛 IP** 贯穿全场景 | 没有 mascot 就跟 LinkedIn 没区别 |
| **大数字** — 匹配度 86% / 进度 75% / 整体进度等显眼 | 求职是数据驱动 — 让用户秒懂状态 |

### 跟其它求职产品的差别

| 产品 | 主色 | Mascot | 调性 |
|------|------|--------|------|
| LinkedIn | 企业蓝 | 无 | 严肃职业 |
| Seek | 红色 | 无 | 本地强势 |
| Indeed | 蓝 | 无 | 海量列表 |
| 实习僧 | 蓝绿 | 蘑菇头 | 大学生本土 |
| **Job Hunter** | **Periwinkle** | **求职牛** | **专业 + 暖 + AI 陪伴** |

---

## 3. Mascot 系统

### 3.1 IP 设定

**求职牛** — 跟 UniMate AI / 牛小匠**同源**（都是公牛），但**穿西装 + 戴墨镜 + 公文包**变成"职场牛"。

> ⚠️ **共用 IP 但不同 outfit** — 这是个有意识的设计决策：JR Academy 旗下的"匠人系"产品共享牛形象做家族识别，但通过 outfit 区分子产品。

### 3.2 服装与道具

#### Outfit
- 白衬衫
- 橙色领带（保留 UniMate 暖意）
- 深色西装裤
- 可选蓝色 / 深色 blazer
- **墨镜保留**（强化家族识别）

#### Career Props（按场景选）
- 公文包 / Briefcase
- 简历纸 / Resume
- 放大镜 / Magnifying glass
- Offer letter
- 上升箭头 / Growth arrow
- 公司大楼 / Company building
- Chat bubble（聊天 / AI 消息）
- Calendar（面试日程）
- Bookmark（收藏职位）

### 3.3 8 个标准态（禁止自创）

| State | 中文名 | 视觉特征 | 触发场景 |
|-------|--------|---------|---------|
| `analyzing` | 分析中 | 拿放大镜看 JD | JD 分析 loading / 解析职位 |
| `interview-prep` | 面试准备 | 拿小本子 / microphone | 面试模拟 / 题库练习 |
| `resume-edit` | 修改简历 | 拿简历打勾 | 简历优化页 / score card |
| `offer` | 拿到 Offer | 举 offer letter / 欢呼 | Offer 收到 / 成功通过 |
| `thinking` | 思考中 | 手托下巴 | 空状态 / loading 通用 |
| `cheering` | 加油中 | 拿旗子 / 拳头 | streak / 倒计时 / 鼓励 |
| `company-research` | 公司研究 | 指向公司图表 | 公司研究卡 / 数据洞察 |
| `networking` | 人脉拓展 | 拿聊天气泡 | 人脉管理 / AI 消息起草 |

### 3.4 选择决策树

```
用户在干嘛？
├── 分析职位
│   ├── 分析中 / loading → analyzing
│   └── 看公司数据 → company-research
│
├── 简历
│   └── 优化 / 改简历 → resume-edit
│
├── 面试
│   └── 准备 / 模拟 → interview-prep
│
├── 投递追踪
│   ├── 拿到 Offer → offer
│   └── 鼓励 / streak → cheering
│
├── 人脉
│   └── 拓展 / AI 起草 → networking
│
├── 卡住 / 空状态
│   └── 默认 → thinking
│
└── 不知道用哪个 → analyzing（最高频）
```

### 3.5 Mascot 红线

- ❌ 不要去掉墨镜（家族识别核心元素）
- ❌ 不要把求职牛画成 UniMate AI 牛小匠（要有西装/公文包区分）
- ❌ 不要换成企鹅（那是 Cert Master 的）
- ❌ 不要自创新表情 — 必须 map 到 8 标准态
- ❌ 不要给牛改色（黑白 + 橙领带是固定的）
- ❌ 一屏 ≥2 个不同状态 mascot

---

## 4. Color 系统

### 4.1 Core Palette（核心 8 色）

| Token | Hex | CSS Var | 用途 |
|-------|-----|---------|------|
| Primary Periwinkle | `#5F7CFB` | `--jh-primary` | **主按钮 / 核心操作 / AI 分析** |
| Secondary Periwinkle | `#9BB1FF` | `--jh-secondary` | 次级按钮 / 柔和高亮 / 图标 bg |
| Accent Coral | `#FF8A7A` | `--jh-accent` | **Offer / 提醒 / CTA 强调** |
| Career Navy | `#182035` | `--jh-navy` | 标题 / Logo / 重要文本 |
| Medium Gray | `#66728D` | `--jh-gray` | 正文 / 辅助 |
| Light Gray | `#E6E9F2` | `--jh-light-gray` | Border / divider / 禁用态 |
| Warm White | `#FFFEF7` | `--jh-warm-white` | **页面默认 bg**（不要纯白） |
| Pure White | `#FFFFFF` | `--jh-white` | 卡片 / 弹窗 |

### 4.2 功能色

| 用途 | Hex | CSS Var |
|------|-----|---------|
| Success Green | `#35C98B` | `--jh-success` — 高匹配 / 已投 / 完成 |
| Warning Amber | `#FFB84D` | `--jh-warning` — 待优化 / 注意 |
| Error Red | `#FF6B6B` | `--jh-error` — 缺失技能 / 失败 |
| Purple Insight | `#8B5CF6` | `--jh-insight` — AI 智能建议 |

### 4.3 Soft Washes（10% 浅色）

| 名称 | Hex | CSS Var |
|------|-----|---------|
| Soft Blue | `#EEF3FF` | `--jh-soft-blue` |
| Soft Green | `#EAFBF3` | `--jh-soft-green` |
| Soft Amber | `#FFF6E0` | `--jh-soft-amber` |
| Soft Purple | `#F2EDFF` | `--jh-soft-purple` |
| Soft Peach | `#FFF0E8` | `--jh-soft-peach` |

### 4.4 Gradients（first-class）

| Gradient | CSS Var | 用途 |
|----------|---------|------|
| Primary Blue | `--jh-grad-primary` `135deg #6F8CFF → #4F6EF7` | AI 分析 / 主按钮 / Active nav |
| Soft Blue | `--jh-grad-soft-blue` `135deg #F3F6FF → #EAF0FF` | Hero card / AI assistant 背景 |
| Coral | `--jh-grad-coral` `135deg #FF9A80 → #FF6B5F` | **Offer / 高紧迫 CTA / banner** |
| Success | `--jh-grad-success` `135deg #6BE7BF → #1FC692` | 高匹配 / 已完成 |

### 4.5 功能配色映射

| Feature | Main | Support |
|---------|------|---------|
| JD 分析 | Primary | Soft Blue |
| 简历优化 | Success | Soft Green |
| 面试准备 | Insight Purple | Soft Purple |
| 公司研究 | Navy | Soft Blue |
| 职位追踪 | Primary | Success |
| Offer / 成功 | Accent Coral | Success |
| 薪资分析 | Warning Amber | Soft Amber |
| 缺失技能 | Error | Soft Peach |
| 人脉管理 | Insight | Soft Purple |
| AI 消息起草 | Primary | Soft Blue |

### 4.6 匹配度色逻辑

```
80-100  →  Success Green  →  "很匹配 / 建议优先投递"
60-79   →  Primary Blue   →  "可以投，但建议先优化简历"
40-59   →  Warning Amber  →  "差一些技能 / 需要重点准备"
< 40    →  Error / Coral  →  "差距较大 / 慎投"
```

### 4.7 用色红线

- ❌ 不要用银行 / 政府那种深蓝（保持 Periwinkle 长春花蓝）
- ❌ 不要让全屏都是蓝（Coral / Green 做强调点）
- ❌ 不要把 Coral 滥用 — 它专属 Offer 和高紧迫 CTA
- ❌ 大块 bg 不要纯白（必须 Warm White `#FFFEF7`）
- ❌ 不要在一张卡里堆 ≥3 种功能色（混乱）
- ❌ 不要用霓虹 / 赛博朋克色

---

## 5. Typography 系统

### 5.1 字体族

| 角色 | 字体 | CSS Var |
|------|------|---------|
| 主字体 | `'PingFang SC', 'Source Han Sans SC', 'HarmonyOS Sans SC', 'Microsoft YaHei', 'Plus Jakarta Sans', 'Inter', system-ui, ...` | `--jh-font-sans` |
| 等宽 | `'JetBrains Mono', 'SF Mono', Menlo, Consolas, monospace` | `--jh-font-mono` |

**等宽专用**：匹配度数字（86%）/ 积分 / 时间戳 / 薪资范围。

### 5.2 字号尺度（9 级）

| Level | Size | Weight | 用途 | CSS class |
|-------|------|--------|------|-----------|
| Hero | 48px | Extrabold (800) | 首页主标题 44-56px | `.jh-hero` |
| Page | 36px | Bold (700) | 页面标题 32-40px | `.jh-page` |
| Section | 24px | Bold (700) | 模块标题 22-28px | `.jh-section` |
| Card | 18px | Bold (700) | 卡片标题 17-20px | `.jh-card` |
| Body | 16px | Regular/Medium | 正文 15-16px | `.jh-body` |
| Body Sm | 14px | Regular/Medium | 辅助文字 13-14px | `.jh-body-sm` |
| Caption | 12px | Medium | 标签 / metadata | `.jh-caption` |
| Button | 15px | Bold (700) | 按钮文字 15-16px | — |
| **Data Number** | 40px | Extrabold | **匹配度 / 积分 / 进度** 32-48px | `.jh-data` |

### 5.3 字重

| 名称 | 值 | CSS Var |
|------|-----|---------|
| Regular | 400 | `--jh-fw-regular` |
| Medium | 500 | `--jh-fw-medium` |
| Semibold | 600 | `--jh-fw-semibold` |
| Bold | 700 | `--jh-fw-bold` |
| **Extrabold** | 800 | `--jh-fw-extrabold` |

### 5.4 排版规则

- **数字要大**：86%、58%、120 积分 — 求职是数据驱动
- **中文标题厚重**：体现"匠"的力量
- **英文职位名清晰**：`Frontend Engineer`、`Senior PM` 等
- **辅助文字不要太淡**：求职信息需要可信度，避免 #C7C0D5 这种太浅

### 5.5 红线

- ❌ 求职匠**比 UniMate 更克制** — 不要用 Caveat 手写体（那是 UniMate 的）
- ❌ Body 字号不要 < 13px（中文阅读不舒服）
- ❌ 一屏 ≥4 种字号（视觉过载）
- ❌ 标题不要细字重（< Bold） — 体现专业可信感

---

## 6. Spacing · Radius · Shadow

### 6.1 Spacing — 4pt 网格

```
4 / 8 / 12 / 16 / 20 / 24 / 32 / 40 / 48 / 64 / 80
```

| 用途 | 推荐 |
|------|------|
| 内联元素 gap (chip / icon) | 4-8px |
| 表单内 padding | 12-16px |
| 卡片 padding | 16-24px |
| Section 之间 | 32-48px |
| 页面顶 / 底 padding | 64-80px |

### 6.2 Radius — 8 档

| 名称 | px | CSS Var | 用途 |
|------|-----|---------|------|
| xs | 6 | `--jh-radius-xs` | Icon micro |
| sm | 10 | `--jh-radius-sm` | Tags / chips |
| md | 14 | `--jh-radius-md` | Inputs |
| lg | 18 | `--jh-radius-lg` | Small cards |
| **xl** | **22** | `--jh-radius-xl` | **Standard cards (默认)** |
| xxl | 28 | `--jh-radius-xxl` | Feature cards / Modal |
| xxxl | 36 | `--jh-radius-xxxl` | Hero / promo banners |
| full | 9999 | `--jh-radius-full` | Buttons / pills |

**默认偏好**：卡片用 `xl` (22px)，hero banner 用 `xxxl` (36px)，按钮用 `full`。
求职匠**比 UniMate AI 略克制**（UniMate `lg=24/xl=40`，求职匠 `xl=22/xxl=28`），但仍然是友好圆角。

### 6.3 Shadow

| 名称 | 值 | 用途 |
|------|-----|------|
| xs | `0 2px 8px rgba(24,32,53,0.04)` | 小按钮 |
| sm | `0 4px 12px rgba(24,32,53,0.06)` | 输入框 |
| md | `0 8px 24px rgba(24,32,53,0.08)` | 卡片（默认） |
| lg | `0 16px 40px rgba(24,32,53,0.10)` | Hero / Modal |
| **blue-glow** | `0 12px 28px rgba(95,124,251,0.28)` | **主按钮发光** |
| coral-glow | `0 12px 28px rgba(255,138,122,0.25)` | Offer CTA 发光 |

阴影偏 navy 调（`rgba(24,32,53)`）— 让阴影自带蓝调，跟 Periwinkle 主色协调。

---

## 7. Logo & Banner

### 7.1 Logo 组成

```text
[ 求职牛头像 + 放大镜 / 公文包 / 上升箭头 ] + 求职匠
副标题：你的 AI 求职助手
```

### 7.2 Logo 用色

- 主文字：`#182035` (Navy)
- Accent：`#5F7CFB` (Primary) 或 `#FF8A7A` (Coral)
- "AI" 小字可用 Coral 或 Blue（按上下文）

### 7.3 Logo 5 件套（待补）

| 名称 | 文件 (TODO) | 用途 |
|------|------------|------|
| Horizontal | `assets/logo/horizontal.png` | 官网 header / 邮件签名 |
| Compact | `assets/logo/compact.png` | 海报 / PPT / App 启动 |
| Avatar | `assets/logo/avatar.png` | 圆头 / favicon |
| App Icon | `assets/logo/app-icon.png` | 通用 App 图标 |
| App Icon iOS | `assets/logo/app-icon-ios.png` | iOS 圆角方块 |

### 7.4 Banner 用法

| 变体 | 实现 | 场景 |
|------|------|------|
| Hero Promo | `--jh-grad-soft-blue` 底 + 求职牛右侧 + CTA | landing hero / 月度推广 |
| Coral Push | `--jh-grad-coral` 底 + Offer 文案 | "立即体验" / 转化 banner |
| Light Strip | 白底卡 + horizontal logo + tagline | 页眉 / 邮件签名 |

### 7.5 Logo 红线

- ❌ 不要拉伸 / 倾斜
- ❌ 不要去掉墨镜（家族识别）
- ❌ 不要把求职牛画成牛小匠（要西装/公文包）
- ❌ 不要用 Cert Master 的 `#FFC52A` 黄色（那是考证匠）
- ❌ 不要 logo 加 box-shadow / glow

---

## 8. 组件规范

### 8.1 Buttons

#### Primary Button（48px 蓝色胶囊）
```css
height: 48px; padding: 0 24px;
border-radius: var(--jh-radius-full);
background: var(--jh-grad-primary);
color: white; font-weight: 700; font-size: 15px;
box-shadow: var(--jh-shadow-blue-glow);
```
**用于**：AI 分析 / 一键优化简历 / 开始分析 / 保存职位

#### Coral CTA（高转化 / Offer 专用）
```css
background: var(--jh-grad-coral);
box-shadow: var(--jh-shadow-coral-glow);
```
**用于**：立即体验 / 开启 AI 求职助手 / 生成面试题

#### Secondary Button（白底蓝边）
```css
height: 44px; padding: 0 22px;
border-radius: var(--jh-radius-full);
background: var(--jh-white);
border: 1.5px solid #DCE4FF;
color: var(--jh-primary); font-weight: 700;
```

#### Ghost Button
```css
background: transparent;
color: var(--jh-primary); font-weight: 600;
```

#### 状态规则
- Hover: lift 1-2px
- Pressed: scale 0.98
- Disabled: 灰底 + light-gray text

### 8.2 Inputs

#### Job URL Input（导入 LinkedIn / Seek / Indeed / Glassdoor 链接）
```css
height: 52px; border-radius: var(--jh-radius-lg);
border: 1.5px solid #DCE4FF;
box-shadow: var(--jh-shadow-sm);
padding: 0 16px;
```
**Placeholder**：`粘贴职位链接，如 LinkedIn / Seek / Indeed / Glassdoor`

#### Focus
```css
border-color: var(--jh-primary);
box-shadow: 0 0 0 4px rgba(95,124,251,0.12);
```

#### Upload Field（简历上传）
- Dashed border
- Upload cloud icon
- 格式说明：`支持 PDF / DOCX，最大 10MB`
- 下方主按钮

### 8.3 Cards 6 种

#### Job Card（职位卡）
- 公司 logo + 职位名 + 公司名 + 地点 + 匹配度 + 薪资 + 收藏
- `border-radius: var(--jh-radius-xl)` (22px)

#### Match Score Card（匹配度卡）
- **大数字 40px+**：`86%`
- 进度条 + 匹配 tag + 技能 summary
- 颜色按 §4.6 色逻辑

#### Interview Prep Card
- 题数 + 类别 + 进度 + 练习按钮

#### Company Research Card
- 公司名 + 规模 + 评分 + 文化 / 薪资洞察

#### Job Progress Card
- Saved / Applied / Interview / Offered（stepper 或 stacked rows）

#### Profile Match Card
- Profile 匹配度大数字 + 圆环 + 优化建议条目数

### 8.4 Chips & Tags

#### Status Tags

| 状态 | 颜色 |
|------|------|
| Saved | Gray |
| Applied | Primary Blue |
| Interview | Coral |
| Offered | Success Green |
| Rejected | Gray / muted |
| Urgent | Coral |
| High Match | Success Green |
| AI Recommended | Primary / Insight Purple |

#### Tag Style
```css
height: 28px; padding: 0 12px;
border-radius: var(--jh-radius-full);
font-size: 12px; font-weight: 600;
```

#### 职位特性 tag
Remote / Hybrid / React / TypeScript / Python / Sponsor / Junior Friendly / High Match

### 8.5 Navigation

| 类型 | 规则 |
|------|------|
| Top Bar | Logo 左 + 主导航 + 积分 pill 右；active 用 Primary |
| Side Nav (Web) | 白 / warm canvas bg + soft blue pill active |
| Bottom Nav (Mobile) | 5 项：首页 / 职位 / **AI 助手** (中央 emphasis) / 追踪 / 我的 |

### 8.6 Progress

#### Match Progress Bar
```css
height: 8px; background: var(--jh-light-gray);
border-radius: var(--jh-radius-full);
```
Filled: `linear-gradient(90deg, #5F7CFB 0%, #9BB1FF 100%)`

#### Application Progress（投递追踪）
```
Saved      12
Applied    18
Interview   6
Offered     2
```

### 8.7 Alerts

| Type | Color | Example |
|------|-------|---------|
| Success | Green | 简历解析完成！ |
| Warning | Amber | 未检测到完整 JD 内容 |
| Error | Coral | 链接解析失败，请重试 |
| Info | Blue | AI 正在分析职位匹配度 |

```css
border-radius: var(--jh-radius-md);
padding: 12px 16px;
background: <soft wash>;
border: 1px solid <matching light border>;
```

### 8.8 Modals

- Resume Upload Modal: upload zone + 格式说明 + 隐私 note + Primary 按钮
- Job Analysis Modal: URL input + 支持平台 icons + "开始分析" 按钮

```css
background: white;
border-radius: var(--jh-radius-xxl); /* 28px */
box-shadow: var(--jh-shadow-lg);
padding: 24px;
```

### 8.9 Banner / Promo Card

**主文案**：`AI 助你脱颖而出，拿到理想 Offer！`
**子文案**：`智能分析 · 简历优化 · 面试准备 · 全流程陪伴`

- soft blue 或 soft peach 渐变 bg
- 求职牛 mascot 右侧（offer / cheering 状态）
- 主 CTA 按钮在左侧
- 圆角 `xxxl` (36px)

---

## 9. Voice & Tone

### 9.1 Voice

- Professional 专业
- Encouraging 鼓励
- Direct 直接
- Actionable 可执行
- Friendly 友好
- **比 UniMate AI 更克制**（UniMate 偏 meme，求职匠偏专业）

### 9.2 中文文案范例

| ✅ 这样写 | ❌ 不要这样 |
|----------|-----------|
| 今天想拿下什么工作？ | 今日推荐职位 |
| 这个岗位值得投吗？ | 该职位匹配分析报告 |
| 你的简历还差这 3 个关键词 | 简历优化建议（共 3 条） |
| 高匹配，建议优先投递 | 综合匹配度达到 86% |
| AI 帮你拆解 JD | 智能解析职位描述 |
| 离 Offer 又近一步 | 您的求职进度已更新 |
| 面试前先练这 5 道题 | 已为您生成 5 道面试题 |

### 9.3 英文范例

- Analyze this job
- Optimize my resume
- Prepare for interview
- Track application
- High match
- AI recommended
- Save this job
- Your next best action

### 9.4 永远别用

- "您" — 用"你"
- "亲爱的求职者" — 太教务系统
- "智能化 / 数字化 / 赋能" — SaaS 味
- "Deadline 战神 / 我裂开了" — 那是 UniMate AI 的 meme，求职匠不要
- "考过 / 拿下证书" — 那是 Cert Master 的语境

### 9.5 场景文案

| 场景 | 范例 |
|------|------|
| Hero question | "今天想拿下什么工作？" |
| JD 分析 | "粘贴职位链接，AI 帮你拆解 JD" |
| Resume score | "你的简历还差这 3 个关键词" |
| Interview prep | "面试前先练这 5 道题" |
| Application save | "已帮你保存到职位追踪" |
| Offer 收到 | "离 Offer 又近一步" |
| Loading | "AI 正在分析岗位要求" |
| High match | "高匹配，建议优先投递" |

---

## 10. Motion

### 10.1 Duration

| 用途 | 值 | CSS Var |
|------|-----|---------|
| Button hover | 160ms | `--jh-dur-button` |
| Card hover | 200ms | `--jh-dur-card` |
| Modal open | 240ms | `--jh-dur-modal` |
| Progress update (0→value) | 400ms | `--jh-dur-progress` |
| Mascot reaction | 400ms | `--jh-dur-mascot` |

### 10.2 Easing

| 名称 | 值 | CSS Var |
|------|-----|---------|
| Standard | `cubic-bezier(0.2, 0.8, 0.2, 1)` | `--jh-ease-standard` |
| Spring | `cubic-bezier(0.34, 1.56, 0.64, 1)` | `--jh-ease-spring` — Offer 庆祝 |

### 10.3 关键动效

- **Button hover**：lift 1-2px + 加深 glow
- **Card hover**：lift 2-3px + shadow sm → md
- **Match score**：从 0 动画到目标值（400ms）
- **Mascot 分析完**：nod 或 point 一下
- **Offer 收到**：可加小 confetti（克制 — 别 Duolingo 化）

### 10.4 红线

- ❌ 不要过度卡通弹跳（求职是专业产品）
- ❌ 不要 ≥1s 的动画
- ❌ 不要让 mascot 持续抖 / 转
- ❌ 不要给数据数字加 fade — 用户要快速读数

---

## 11. Do / Don't 红线

### 11.1 视觉

| ✅ Do | ❌ Don't |
|-------|---------|
| 页面 bg = `--jh-warm-white`，卡片 = 白 | bg = `#FFFFFF` |
| 主 CTA = Periwinkle 蓝渐变 | 深蓝企业风按钮 |
| Coral 只用作 Offer / 转化 | Coral 满屏堆 |
| 大数字（匹配度 86%）显眼 | 数字塞在小字角落 |
| Mascot 用 8 标准态 | 自创新表情 |
| 一屏 ≤2 mascot | 满屏求职牛 |
| 卡片圆角 22-28px | 矩形 / 小圆角 |
| 进度条用 Primary grad fill | 用 Coral fill（除非 Offer） |

### 11.2 字体

| ✅ Do | ❌ Don't |
|-------|---------|
| 主字 PingFang SC | 思源宋体 / 楷体 |
| Hero 用 Extrabold 800 | Body 用 800（变广告） |
| 数据用 Mono 等宽 | 数据用 PingFang（对不齐） |
| Body ≥ 14px | < 13px 中文 |
| 用 Caveat 手写体 | ❌（那是 UniMate 的） |

### 11.3 文案

| ✅ Do | ❌ Don't |
|-------|---------|
| 「这个岗位值得投吗？」 | "该职位匹配度分析报告" |
| 「离 Offer 又近一步」 | "您的求职流程已更新" |
| 「高匹配，建议优先投递」 | "推荐指数：⭐⭐⭐⭐⭐" |
| 用「拿下 / 离 Offer」 | 用「冲 deadline / 裂开了」（UniMate 的） |

### 11.4 跟 UniMate AI / Cert Master 别混

| ✅ Job Hunter | ❌ 别用 |
|---------------|---------|
| 求职牛（西装 + 墨镜 + 公文包） | UniMate 普通牛小匠 / Cert Master 企鹅 |
| Periwinkle `#5F7CFB` | UniMate Coral `#FF7A66` / Cert 考证黄 `#FFC52A` |
| 暖白 `#FFFEF7` | 纯白 / Cert 背景灰 `#F5F6F8` |
| PingFang SC | UniMate Plus Jakarta Sans 做中文主字 |
| 数据驱动文案 | UniMate meme / Cert 备考语 |
| CSS 前缀 `--jh-*` | `--um-*` / `--cm-*` |

### 11.5 Code review 自检

PR diff 出现以下立即打回：

- 大块 `bg: #FFFFFF` 没改 → ❌ 必须 `--jh-warm-white`
- 主按钮 background-color 不是渐变 → ❌
- 求职牛没墨镜 / 公文包 → ❌
- 匹配度数字 < 24px → ❌（数字要大）
- 引入 `@mui/material` / `antd` → ❌
- 文案出现"您 / 智能化 / Deadline 战神 / 拿下证书" → ❌
- 出现 UniMate 的 coral / Cert Master 的黄 / 企鹅 → ❌

---

## 12. Asset 目录映射

```
job-hunter/
├── index.html                 ← 视觉品牌手册
├── DESIGN.md                  ← 本文件（完整规范）
├── README.md                  ← 仓库使用说明
├── _source_design.md          ← 原始设计研究稿（存档）
├── tokens/
│   ├── tokens.json            ← W3C Design Tokens 源数据
│   └── tokens.css             ← --jh-* CSS Variables
├── assets/
│   ├── logo/                  ← Logo 5 件套（TODO）
│   ├── mascot/                ← 8 个求职牛状态（TODO）
│   │   └── spec-sheet.png     ← ChatGPT spec 原图 ✅
│   ├── cards/                 ← 6 张卡片插图（TODO）
│   ├── banners/               ← Hero banner（TODO）
│   ├── stickers/              ← 装饰贴纸（TODO）
│   ├── decorations/           ← 装饰素材（TODO）
│   └── _inbox/                ← 待分类区
└── .github/workflows/
    └── deploy.yml             ← GitHub Pages 自动部署
```

---

## 13. 跟 UniMate AI / Cert Master 的隔离规则

Job Hunter 跟 UniMate AI / Cert Master 同属 JR Academy 匠人家族，**严格视觉/品牌隔离**：

| 维度 | UniMate AI (牛小匠) | Cert Master (考证匠) | **Job Hunter (求职匠)** |
|------|---------------------|----------------------|--------------------------|
| Mascot | 普通牛小匠 🐂 | 企鹅 🐧 | **求职牛 (墨镜 + 西装 + 公文包) 🐂🕶** |
| Primary | Coral `#FF7A66` | 考证黄 `#FFC52A` | **Periwinkle `#5F7CFB`** |
| Accent | Bubblegum / Sunshine | 活力橙 | **Coral `#FF8A7A`**（Offer 专用） |
| 主 bg | 暖白 `#FFFEF7` | 背景灰 `#F5F6F8` | **暖白 `#FFFEF7`** |
| 主字体 | Plus Jakarta Sans | PingFang SC | **PingFang SC / 思源黑体** |
| Accent 字体 | Caveat 手写 | 无 | **无**（求职匠克制） |
| 网格 | 8pt | 4pt | **4pt** |
| 圆角偏好 | lg=24, xl=40（最圆） | lg=16, xl=24 | **xl=22, xxxl=36** |
| 渐变 | first-class（5 grad） | 无 | **first-class（4 grad）** |
| 调性 | 学生 meme + 游戏化 | 专业 + 备考严肃 | **专业 + AI 陪伴 + 求职感** |
| Tagline | 陪你冲 deadline | 你的 AI 考证搭子 | **你的 AI 求职助手** |
| CSS 前缀 | `--um-*` | `--cm-*` | **`--jh-*`** |
| 目标用户 | 大学生 | 考证人 | **求职者 / 毕业生 / 转行者** |

### 共用 IP 规则（特殊）

**UniMate 跟 Job Hunter 共用牛形象** — 但通过 outfit 区分：

| | UniMate AI 牛小匠 | **Job Hunter 求职牛** |
|---|---|---|
| Outfit | 卫衣 / 学生装 | **白衬衫 + 橙领带 + 西装** |
| 眼镜 | 圆眼镜（学习中态） | **墨镜（保留家族识别）** |
| 道具 | 笔记本 / 笔 / 书包 | **公文包 / 简历 / 放大镜 / Offer letter** |
| 表情 | 学生 meme（裂开 / 急了） | **职场 cool（专业 cheering）** |

### Cert Master 完全隔离

求职匠跟 Cert Master 没有任何视觉共用：
- ❌ 求职匠 不要出现企鹅
- ❌ 求职匠 不要用考证黄 `#FFC52A`
- ❌ 求职匠 不要用背景灰 `#F5F6F8`

### 隔离实施

- CSS 变量前缀彻底分开（`--um-*` / `--cm-*` / `--jh-*`），同一项目可共 import 无冲突
- Logo / Token / Asset 各自独立 repo（unimate-ai / cert-master / job-hunter）
- Voice 不互抄：UniMate meme / Cert 备考 / Job Hunter 专业职场

---

## 维护

- 每次改 token 必须三处同步：`tokens.json` / `tokens.css` /（如果以后加）`tokens.ts`
- 改了组件规范要在 `index.html` 同步更新视觉示例
- 改了 mascot 或 logo 必须同步更新本文件 §3 / §7 / §12

### Sources of truth 优先级

```
DESIGN.md  ←  最高（决策源头 / 设计意图）
   ↓ 落地
tokens.json  ←  机器可读的真相（Style Dictionary / Figma Tokens）
   ↓ 翻译
tokens.css  ←  CSS Variables 实现
   ↓ 示例
index.html  ←  视觉手册 / 实景演示
```

- **冲突时**：以 DESIGN.md 为准
- **改 DESIGN.md 必须立刻同步**：tokens.json → tokens.css → index.html
- **token 不能擅自改**：手抖把 `#5F7CFB` 写成 `#5F7CFC` → 按 DESIGN.md 改回来
- **DESIGN.md 才是给设计师/PM 改的**；token 是给前端/设计工具读的

---

_v0.1 · 2026-05-12 · JR Academy_
