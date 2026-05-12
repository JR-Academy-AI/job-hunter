# 求职匠 Job Hunter Design System

> **Warm Professional Blue.** 求职匠是与 UniMate AI 并列的 AI App，但定位不同：UniMate AI 是学生的 AI 学习伙伴，求职匠是毕业生、转行者、求职者的 AI 求职助手。视觉上应更专业、更可信，但仍保留匠人系产品的年轻、友好、IP 化风格。

---

## 1. Brand Positioning 品牌定位

### Brand Name

- 中文：**求职匠**
- English：**Job Hunter**
- Product Type：AI 求职助手 / AI Job Search Assistant
- Parent Brand：匠人学院 / JR Academy

### Core Positioning

中文定位：

> 你的 AI 求职助手，帮你分析 JD、优化简历、准备面试、追踪投递进度。

English positioning:

> Your AI job search assistant for smarter applications, better interviews, and faster offers.

### Product Relationship

求职匠与 UniMate AI 是并列产品：

| Product | Audience | Core Scenario | Visual Mood |
|---|---|---|---|
| UniMate AI / 牛小匠课代表 | 大学生 / 留学生 | 学习、课程、复习、AI 课代表 | Warm Coral / Playful Study Companion |
| 求职匠 / Job Hunter | 求职者 / 毕业生 / 转行者 | JD 分析、简历优化、面试准备、投递追踪 | Warm Blue / Professional Career Companion |

### Brand Personality

- Professional 专业
- Trustworthy 可信
- Helpful 实用
- Smart 智能
- Friendly 友好
- Action-oriented 行动导向
- Not corporate 不要过度企业化
- Not childish 不幼稚

### Visual Keywords

- Warm blue 温暖蓝
- Career-focused 求职感
- Professional but friendly 专业但友好
- Rounded 圆润
- Clean 清晰
- Mascot-driven IP 化
- Progress-oriented 进度感
- Data cards 数据卡片
- Job board feeling 招聘平台感

---

## 2. Visual Direction 视觉方向

### Core Visual Language

求职匠应该像：

> **LinkedIn × Canva × Linear × Airbotix × JR Academy Mascot**

但不要像：

- 冷冰冰的 SaaS Dashboard
- 企业 CRM 后台
- 传统招聘网站
- 过度卡通的儿童产品
- 金融产品

### Design North Star

> 让求职这件焦虑的事情，变得清楚、有步骤、有反馈、有陪伴。

The UI should help users quickly understand:

1. 这个职位值不值得投？
2. 我的匹配度是多少？
3. 简历哪里需要优化？
4. 面试该准备什么？
5. 我当前投递进度如何？
6. 下一步该做什么？

---

## 3. Color System 色彩系统

### Chosen Direction

推荐使用第二套蓝色方向：

# **Periwinkle Career Blue / 长春花蓝**

这套蓝色比传统科技蓝更柔和，不会太 SaaS，也不会太冷。它有专业感、年轻感和记忆点。

---

### Core Palette 核心配色

| Token | Hex | Usage |
|---|---:|---|
| Primary Periwinkle | `#5F7CFB` | 主按钮、核心操作、AI 分析 |
| Secondary Periwinkle | `#9BB1FF` | 次级按钮、柔和高亮、图标背景 |
| Accent Coral | `#FF8A7A` | Offer、提醒、CTA 强调 |
| Career Navy | `#182035` | 标题、Logo、重要文本 |
| Medium Gray | `#66728D` | 正文、辅助文字 |
| Light Gray | `#E6E9F2` | 边框、分割线、禁用态 |
| Warm White | `#FFFEF7` | 页面背景 |
| Pure White | `#FFFFFF` | 卡片、弹窗 |

---

### Extended Colors 功能色

| Token | Hex | Usage |
|---|---:|---|
| Success Green | `#35C98B` | 匹配度高、已投递、完成 |
| Warning Amber | `#FFB84D` | 待优化、注意事项 |
| Error Red | `#FF6B6B` | 缺失技能、失败、风险 |
| Purple Insight | `#8B5CF6` | AI insight、智能建议 |
| Soft Peach | `#FFF0E8` | 温暖提示区、banner 背景 |
| Soft Blue | `#EEF3FF` | 信息卡、AI 分析背景 |
| Soft Green | `#EAFBF3` | 高匹配、成功背景 |
| Soft Amber | `#FFF6E0` | 警告、薪资提示背景 |
| Soft Purple | `#F2EDFF` | AI 建议背景 |

---

### Gradient System 渐变系统

#### Primary Blue Gradient

```css
linear-gradient(
  135deg,
  #6F8CFF 0%,
  #4F6EF7 100%
)
```

Use for:

- AI 分析
- 主按钮
- Active bottom nav
- 核心 CTA

#### Soft Blue Gradient

```css
linear-gradient(
  135deg,
  #F3F6FF 0%,
  #EAF0FF 100%
)
```

Use for:

- Hero card
- AI assistant card
- Job analysis background

#### Coral Offer Gradient

```css
linear-gradient(
  135deg,
  #FF9A80 0%,
  #FF6B5F 100%
)
```

Use for:

- Offer
- High urgency CTA
- Banner highlights

#### Success Gradient

```css
linear-gradient(
  135deg,
  #6BE7BF 0%,
  #1FC692 100%
)
```

Use for:

- 高匹配
- 已完成
- Progress success

---

### Color Mapping 功能配色映射

| Feature | Main Color | Support Color |
|---|---|---|
| JD 分析 | Primary Periwinkle | Soft Blue |
| 简历优化 | Success Green | Soft Green |
| 面试准备 | Purple Insight | Soft Purple |
| 公司研究 | Career Navy | Soft Blue |
| 职位追踪 | Primary Periwinkle | Success Green |
| Offer / 成功 | Accent Coral | Success Green |
| 薪资分析 | Warning Amber | Soft Amber |
| 缺失技能 | Error Red | Soft Peach |
| 人脉管理 | Purple Insight | Soft Purple |
| AI 消息起草 | Primary Periwinkle | Soft Blue |

---

### Color Principles

#### Do

- Use blue as a professional base.
- Use warm white canvas to avoid cold SaaS feeling.
- Use coral only as a sharp accent.
- Use green for progress and success.
- Use soft color washes in cards.
- Keep the overall feeling clean and trustworthy.

#### Don’t

- Do not use harsh enterprise blue.
- Do not make everything blue.
- Do not use dark dashboard style as the default.
- Do not overuse gradients.
- Do not use neon cyberpunk colors.
- Do not make it look like a CRM or ATS admin panel.

---

## 4. Typography 字体系统

### Chinese Font

Recommended:

- 思源黑体 / Source Han Sans
- PingFang SC
- HarmonyOS Sans SC
- Microsoft YaHei

### English Font

Recommended:

- Plus Jakarta Sans
- Inter
- Poppins

### Typography Tone

求职匠应更专业，因此字体要比 UniMate AI 更克制：

- 更少手写体
- 更少装饰
- 标题更有力量
- 正文更清晰
- 数字数据更突出

### Type Scale

| Token | Size | Weight | Usage |
|---|---:|---:|---|
| Hero Title | 44–56px | 800 | 首页主标题 |
| Page Title | 32–40px | 700 | 页面标题 |
| Section Title | 22–28px | 700 | 模块标题 |
| Card Title | 17–20px | 700 | 卡片标题 |
| Body | 15–16px | 400/500 | 正文 |
| Body Small | 13–14px | 400/500 | 辅助文字 |
| Caption | 12px | 500 | 标签、metadata |
| Button | 15–16px | 700 | 按钮文字 |
| Data Number | 32–48px | 800 | 匹配度、积分、进度 |

### Typography Rules

- 数字要大，例如 `86%`, `58%`, `120 积分`.
- 中文标题要厚重，体现“匠”的力量。
- 英文职位名要清晰，例如 `Frontend Engineer`.
- 辅助文字不要太淡，求职信息需要可信度。

---

## 5. Logo & Mascot 吉祥物方向

### Mascot

求职匠仍然使用牛小匠家族的牛形象，但要与 UniMate AI 做区分。

### Mascot Outfit

不一定穿红色 hoodie。推荐：

#### Main Outfit

- 白衬衫
- 橙色领带
- 深色西装裤
- 可选蓝色/深色 blazer
- 墨镜保留，强化家族识别

#### Career Props

用这些元素体现求职：

- Briefcase 公文包
- Resume 简历纸
- Magnifying glass 放大镜
- Offer letter
- Growth arrow 上升箭头
- Company building
- Chat bubble
- Calendar interview
- Bookmark saved job

### Mascot States

| State | Visual |
|---|---|
| 分析中 | 拿放大镜看 JD |
| 面试准备 | 拿小本子 / microphone |
| 修改简历 | 拿简历打勾 |
| 拿到 Offer | 举 offer letter |
| 思考中 | 手托下巴 |
| 加油中 | 拿旗子 / 拳头 |
| 公司研究 | 指向公司图表 |
| 人脉拓展 | 拿聊天气泡 |

### Logo Direction

Logo 应体现：

- 求职
- 匠人
- AI
- 专业成长

Recommended composition:

```text
[ 牛小匠头像 + 放大镜 / 公文包 / 上升箭头 ] + 求职匠
副标题：你的 AI 求职助手
```

### Logo Color

- Main text: `#182035`
- Accent: `#5F7CFB` or `#FF8A7A`
- Small AI text can use Coral or Blue depending on context.

---

## 6. Shape System 圆角系统

求职匠可以比 UniMate AI 略微更克制，但仍然保持友好圆角。

| Token | Radius | Usage |
|---|---:|---|
| XS | 6px | Icon micro elements |
| SM | 10px | Tags |
| MD | 14px | Inputs |
| LG | 18px | Small cards |
| XL | 22px | Standard cards |
| XXL | 28px | Feature cards |
| XXXL | 36px | Hero cards / promo banners |
| Full | 9999px | Buttons / pills |

### Rules

- Main cards use 20–24px.
- Hero cards use 28–36px.
- Buttons use full pill.
- Avoid sharp enterprise rectangles.

---

## 7. Spacing System 间距系统

Base unit: **4px**

| Token | Value |
|---|---:|
| 1 | 4px |
| 2 | 8px |
| 3 | 12px |
| 4 | 16px |
| 5 | 20px |
| 6 | 24px |
| 8 | 32px |
| 10 | 40px |
| 12 | 48px |
| 16 | 64px |
| 20 | 80px |

### Layout Principles

- 数据类页面可以比 UniMate AI 更紧凑。
- 信息必须有层级，不能堆满。
- 卡片之间保持足够呼吸感。
- 移动端重要模块优先展示：搜索 / AI 分析 / 热门职位 / 求职进度。

---

## 8. Shadow & Depth 阴影系统

### Shadow Tokens

| Token | Value | Usage |
|---|---|---|
| Shadow XS | `0 2px 8px rgba(24,32,53,0.04)` | 小按钮 |
| Shadow SM | `0 4px 12px rgba(24,32,53,0.06)` | 输入框 |
| Shadow MD | `0 8px 24px rgba(24,32,53,0.08)` | 卡片 |
| Shadow LG | `0 16px 40px rgba(24,32,53,0.10)` | Hero / Modal |
| Blue Glow | `0 12px 28px rgba(95,124,251,0.28)` | 主按钮 |
| Coral Glow | `0 12px 28px rgba(255,138,122,0.25)` | Offer CTA |

### Rule

- Use clean, soft shadows.
- Avoid heavy glassmorphism.
- Avoid excessive glow.
- 求职匠应更像 professional product，不是游戏 App。

---

## 9. Component System 组件系统

---

## 9.1 Buttons 按钮

### Primary Button

Use for the most important action.

```css
height: 48px;
padding: 0 24px;
border-radius: 9999px;
background: linear-gradient(135deg, #6F8CFF 0%, #4F6EF7 100%);
color: #FFFFFF;
font-size: 15px;
font-weight: 700;
box-shadow: 0 12px 28px rgba(95,124,251,0.28);
```

Example labels:

- AI 分析
- 一键优化简历
- 开始分析
- 保存职位
- 查看报告

### Coral CTA Button

Use for offer / conversion / urgency.

```css
background: linear-gradient(135deg, #FF9A80 0%, #FF6B5F 100%);
box-shadow: 0 12px 28px rgba(255,138,122,0.25);
```

Example labels:

- 立即体验
- 开启 AI 求职助手
- 生成面试题

### Secondary Button

```css
height: 44px;
padding: 0 22px;
border-radius: 9999px;
background: #FFFFFF;
border: 1.5px solid #DCE4FF;
color: #5F7CFB;
font-size: 14px;
font-weight: 700;
```

Example labels:

- 公司研究
- 保存草稿
- 查看报告
- 了解更多

### Ghost Button

```css
background: transparent;
color: #5F7CFB;
font-weight: 600;
```

### Button Rules

- Main button should be blue.
- Coral only for conversion or high energy moments.
- Include icon when it improves clarity.
- Avoid plain rectangular buttons.
- Hover state: lift 1–2px.
- Pressed state: scale 0.98.

---

## 9.2 Inputs 输入框

### Job URL Input

For importing LinkedIn / Seek / Indeed / Glassdoor job links.

```css
height: 52px;
border-radius: 18px;
background: #FFFFFF;
border: 1.5px solid #DCE4FF;
box-shadow: 0 4px 12px rgba(24,32,53,0.06);
padding: 0 16px;
```

Placeholder examples:

- 粘贴职位链接，如 LinkedIn / Seek / Indeed / Glassdoor
- 输入职位、公司或技能关键词
- 搜索公司、职位或关键词

### Focus State

```css
border-color: #5F7CFB;
box-shadow: 0 0 0 4px rgba(95,124,251,0.12);
```

### Upload Field

Use for resume upload.

- Dashed border
- Upload cloud icon
- Clear format notes
- Main action button below

Example copy:

```text
点击或拖拽上传简历
支持 PDF / DOCX，最大 10MB
```

---

## 9.3 Cards 卡片

### Job Card

Use for job listing.

Content:

- Company logo
- Job title
- Company name
- Location / Remote / Hybrid
- Match score
- Salary range
- Bookmark

Style:

```css
background: #FFFFFF;
border-radius: 22px;
border: 1px solid #E6E9F2;
box-shadow: 0 8px 24px rgba(24,32,53,0.08);
padding: 18px;
```

### Match Score Card

Use for JD analysis result.

- Large score number
- Progress bar
- Match tag
- Skills summary

Example:

```text
86%
很匹配
```

Color logic:

- 80–100: green
- 60–79: blue
- 40–59: amber
- <40: coral/red

### Interview Prep Card

Content:

- Question count
- Category
- Progress
- Practice button

### Company Research Card

Content:

- Company name
- Company size
- Rating
- Culture notes
- Salary insight

### Job Progress Card

Track:

- Saved
- Applied
- Interview
- Offered

Use stepper or stacked progress rows.

---

## 9.4 Chips & Tags 标签

### Job Feature Tags

Examples:

- Remote
- Hybrid
- React
- TypeScript
- Python
- Sponsor
- Junior Friendly
- High Match

### Status Tags

| Status | Color |
|---|---|
| Saved | Gray |
| Applied | Blue |
| Interview | Coral |
| Offered | Green |
| Rejected | Gray / muted |
| Urgent | Coral |
| High Match | Green |
| AI Recommended | Blue / Purple |

### Tag Style

```css
height: 28px;
padding: 0 12px;
border-radius: 9999px;
font-size: 12px;
font-weight: 600;
```

---

## 9.5 Navigation 导航

### Top Navigation

- Logo on left
- Main nav: 首页 / 职位 / AI 助手 / 消息 / 我的
- Points or credits pill on right
- Active item uses Primary Periwinkle

### Side Navigation Web

For web dashboard:

- White / warm canvas background
- Active item with soft blue pill
- Icon + text
- Avoid heavy dark sidebar

### Bottom Navigation Mobile

Items:

1. 首页
2. 职位
3. AI 助手
4. 追踪
5. 我的

Center AI button can be emphasized with circle gradient.

---

## 9.6 Progress & Data 进度与数据

### Match Progress Bar

```css
height: 8px;
border-radius: 9999px;
background: #E6E9F2;
```

Filled:

```css
background: linear-gradient(90deg, #5F7CFB 0%, #9BB1FF 100%);
```

### Application Progress

Use either:

- Ring chart
- Stepper
- Status rows

Example:

```text
Saved      12
Applied    18
Interview   6
Offered     2
```

### Data Card Rules

- Big numbers
- Clear labels
- Use blue/green/coral to encode status
- Avoid complicated charts unless necessary

---

## 9.7 Alerts 提示组件

| Type | Color | Example |
|---|---|---|
| Success | Green | 简历解析完成！ |
| Warning | Amber | 未检测到完整 JD 内容 |
| Error | Coral | 链接解析失败，请重试 |
| Info | Blue | AI 正在分析职位匹配度 |

Alert style:

```css
border-radius: 16px;
padding: 12px 16px;
background: color wash;
border: 1px solid matching light border;
```

---

## 9.8 Modals 弹窗

### Resume Upload Modal

Contains:

- Upload zone
- Supported formats
- Privacy note
- Primary button

### Job Analysis Modal

Contains:

- Job URL input
- Platform support icons
- “开始分析” button

### Modal Style

```css
background: #FFFFFF;
border-radius: 28px;
box-shadow: 0 16px 40px rgba(24,32,53,0.10);
padding: 24px;
```

---

## 9.9 Banner / Promo Card

### Main Promo Banner

Use for:

- 免费体验
- AI 求职助手
- Offer campaign
- Resume analysis

Style:

- Soft blue or soft peach gradient
- Mascot on right
- CTA button
- Clear benefit list

Example copy:

```text
AI 助你脱颖而出，拿到理想 Offer！
智能分析 · 简历优化 · 面试准备 · 全流程陪伴
```

---

## 10. Iconography 图标系统

Recommended:

- Lucide
- Phosphor
- Custom rounded career icons

### Icon Style

- 1.75px–2px stroke
- Rounded caps
- Friendly but professional
- Can use soft colored square backgrounds

### Core Icons

- Briefcase 职位
- Building 公司
- Calendar 面试
- Document 简历
- Chat 消息
- Bookmark 收藏
- User 个人
- Trend 趋势
- Bot AI 助手
- Target 匹配
- Upload 上传
- Check 完成
- Star 推荐
- Bell 提醒

---

## 11. Product Feature Mapping

| Feature | UI Style | Color |
|---|---|---|
| AI 职位分析 | Score card + progress | Blue |
| 技能匹配 | Checklist / tag matrix | Green / Amber / Coral |
| 简历优化 | Upload + score card | Green |
| 面试准备 | Question list + practice card | Purple |
| 公司研究 | Research card | Navy / Blue |
| 消息起草 | Chat card | Blue / Purple |
| 职位收藏 | Job card + bookmark | Blue |
| 投递追踪 | Kanban / status rows | Blue / Green |
| 人脉管理 | Contact cards | Purple |
| 学习资源推荐 | Course cards | Mint / Blue |

---

## 12. Page-Level Design Rules

### Mobile Home Page

Priority order:

1. Header with mascot + points
2. Hero question: “今天想拿下什么工作？”
3. Job URL input + AI 分析 CTA
4. Four core actions:
   - JD 分析
   - 面试准备
   - Profile 优化
   - 公司研究
5. Hot jobs
6. Interview prep questions
7. Application progress
8. Recent activity
9. Promo banner
10. Bottom navigation

### Web Landing Page

Priority order:

1. Hero with plugin/product positioning
2. Supported platforms
3. 9 core features
4. How it works
5. Use cases
6. Privacy / security
7. CTA

### Dashboard Page

Priority order:

1. Search / import job URL
2. Saved jobs
3. Match analysis
4. Resume score
5. Application tracker
6. Interview preparation
7. Company research

---

## 13. Voice & Microcopy 文案语气

### Voice

- Professional
- Encouraging
- Direct
- Actionable
- Friendly
- Less playful than UniMate AI

### Chinese Examples

- 今天想拿下什么工作？
- 粘贴职位链接，AI 帮你拆解 JD
- 一键分析匹配度
- 这个岗位值得投吗？
- 你的简历还差这 3 个关键词
- 面试前先练这 5 道题
- 已帮你保存到职位追踪
- 离 Offer 又近一步
- AI 正在分析岗位要求
- 高匹配，建议优先投递

### English Examples

- Analyze this job
- Optimize my resume
- Prepare for interview
- Track application
- High match
- AI recommended
- Save this job
- Your next best action

---

## 14. Motion 动效原则

### Timing

| Use | Duration |
|---|---:|
| Button hover | 160ms |
| Card hover | 180–220ms |
| Modal open | 240ms |
| Progress update | 400ms |
| Mascot reaction | 300–500ms |

### Motion Rules

- Buttons lift slightly.
- Score progress animates from 0 to value.
- Mascot can nod or point after analysis.
- Avoid excessive cartoon bounce.
- Offer success can have small confetti.

---

## 15. Do’s and Don’ts

### Do

- Use Periwinkle Blue as the main identity.
- Use Warm White background.
- Use coral as career energy / offer accent.
- Use mascot with career props.
- Make data readable.
- Use big match scores.
- Keep UI clean and credible.
- Show clear next actions.

### Don’t

- Don’t use cold enterprise blue everywhere.
- Don’t make it look like a CRM.
- Don’t overuse mascot.
- Don’t use too many colors in one card.
- Don’t use childish copy.
- Don’t hide important data in tiny text.
- Don’t make job cards overly decorative.

---

## 16. Implementation Tokens

### CSS Variables

```css
:root {
  --jh-primary: #5F7CFB;
  --jh-secondary: #9BB1FF;
  --jh-accent-coral: #FF8A7A;
  --jh-navy: #182035;
  --jh-gray: #66728D;
  --jh-light-gray: #E6E9F2;
  --jh-warm-white: #FFFEF7;
  --jh-white: #FFFFFF;

  --jh-success: #35C98B;
  --jh-warning: #FFB84D;
  --jh-error: #FF6B6B;
  --jh-purple: #8B5CF6;

  --jh-soft-blue: #EEF3FF;
  --jh-soft-green: #EAFBF3;
  --jh-soft-amber: #FFF6E0;
  --jh-soft-purple: #F2EDFF;
  --jh-soft-peach: #FFF0E8;

  --jh-gradient-primary: linear-gradient(135deg, #6F8CFF 0%, #4F6EF7 100%);
  --jh-gradient-coral: linear-gradient(135deg, #FF9A80 0%, #FF6B5F 100%);

  --jh-radius-card: 22px;
  --jh-radius-feature: 28px;
  --jh-radius-hero: 36px;
  --jh-radius-pill: 9999px;

  --jh-shadow-sm: 0 4px 12px rgba(24,32,53,0.06);
  --jh-shadow-md: 0 8px 24px rgba(24,32,53,0.08);
  --jh-shadow-lg: 0 16px 40px rgba(24,32,53,0.10);
  --jh-shadow-blue: 0 12px 28px rgba(95,124,251,0.28);
}
```

---

## 17. Final Summary

求职匠不是一个普通招聘工具，也不是企业 ATS。

它应该是：

> 一个懂澳洲华人求职场景的 AI 求职助手。

视觉上要：

- 比 UniMate AI 更专业
- 比传统招聘网站更年轻
- 比 SaaS Dashboard 更温暖
- 比纯工具产品更有陪伴感

最终感觉：

> 清晰、可信、专业、友好，让用户觉得“我知道下一步该怎么做了”。
