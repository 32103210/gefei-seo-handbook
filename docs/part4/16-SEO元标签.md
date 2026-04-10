# 第 16 章：SEO 元标签完整指南

## 16.1 元标签概述

元标签（Meta Tags）是位于 HTML 文档 `<head>` 区域中的代码片段，用于向搜索引擎和社交平台传递关于网页内容的关键信息。虽然现代 SEO 中元标签的重要性相较于内容质量和外链有所变化，但正确设置元标签仍然是网站技术 SEO 基础中不可忽视的一环。

元标签不会直接显示在页面正文中，但它们对搜索引擎理解页面内容、决定搜索结果展示方式、以及在社交媒体分享时的呈现效果，都起着至关重要的作用。本章将系统讲解每一类元标签的作用、设置方法和常见错误。

**元标签的基本结构：**

```html
<head>
  <!-- 字符编码 -->
  <meta charset="UTF-8">

  <!-- 视口设置（响应式必需） -->
  <meta name="viewport" content="width=device-width, initial-scale=1.0">

  <!-- SEO 元标签开始 -->
  <title>页面标题（显示在浏览器标签和搜索结果中）</title>
  <meta name="description" content="页面描述，出现在搜索结果摘要中">
  <meta name="keywords" content="关键词1, 关键词2, 关键词3">
  <link rel="canonical" href="https://example.com/canonical-url">
  <meta name="robots" content="index, follow">

  <!-- 社交媒体元标签 -->
  <meta property="og:title" content="社交分享标题">
  <meta property="og:description" content="社交分享描述">
  <meta property="og:image" content="https://example.com/share-image.jpg">
  <meta property="og:url" content="https://example.com/page-url">

  <!-- 其他元标签 -->
  <meta name="author" content="作者名">
  <meta name="theme-color" content="#ffffff">
</head>
```

---

## 16.2 Title 标签（标题标签）

### 16.2.1 Title 标签的重要性

Title 标签是 SEO 中权重最高的元标签，没有之一。它同时出现在三个关键位置：
- **浏览器标签页**：用户识别页面身份的依据
- **搜索结果页面（SERP）**：直接决定用户是否点击
- **社交书签和收藏夹**：作为页面标题被保存

谷歌官方明确表示，Title 标签是决定页面在特定关键词下排名的最重要因素之一。同时，研究数据表明，搜索结果中前 50 个字符是用户注意力最集中的区域，Title 标签的质量直接影响点击率（CTR）。

### 16.2.2 Title 标签的设置原则

**原则一：核心关键词靠前**

搜索引擎对 Title 标签中靠前的关键词给予更高的权重。因此，应将最重要的目标关键词放在 Title 的最前面。

```html
<!-- 推荐：核心关键词"SEO教程"在最前面 -->
<title>SEO教程：谷歌 SEO 入门到精通完整指南 | 数字营销博客</title>

<!-- 不推荐：品牌名在最前面，关键词靠后 -->
<title>张三的个人博客 - 最完整的 SEO 教程指南</title>
```

**原则二：品牌名称放在末尾**

品牌名称在 Title 中的作用是品牌辨识和信任背书，不需要占据关键词的宝贵位置。通常用 `|`（竖线）或 `-`（连字符）与主标题分隔。

```html
<!-- 标准格式：关键词 + 分隔符 + 品牌名 -->
<title>关键词核心词 - 修饰词 | 品牌名</title>
<title>关键词 | 品牌名</title>
<title>关键词 - 品牌名</title>

<!-- 具体示例 -->
<title>Python 入门教程（2024最新版） - 编程客</title>
<title>如何写好一份简历 | 猎聘网</title>
<title>iPhone 15 Pro 评测：苹果最强旗舰深度体验 | 极客公园</title>
```

**原则三：控制字符长度在 60 以内**

谷歌在搜索结果中显示的 Title 长度并非固定字符数，而是取决于显示区域的像素宽度。一般建议：
- 英文控制在 60 个字符以内
- 中文控制在 30 个汉字以内
- 移动端的显示空间更窄，需更加精简

```html
<!-- 超长 Title（会被截断） -->
<title>如何通过 SEO 优化让你的网站在谷歌搜索中获得更好的排名：
       完整的 SEO 教程和实战指南，包含技术 SEO、内容 SEO、
       外链建设的全部内容</title>

<!-- 推荐长度 -->
<title>如何通过 SEO 优化提升网站排名：完整实战指南</title>
```

**原则四：每个页面必须有独特的 Title**

网站中每个页面的 Title 都应该是独一无二的。大量页面使用相同的 Title 是最常见的 SEO 错误之一，会导致：
- 搜索引擎难以区分页面主题
- 用户体验差（无法通过浏览器标签区分页面）
- 网站整体 SEO 表现受损

```html
<!-- 网站首页 -->
<title>谷歌 SEO 博客 - 专注数字营销与搜索引擎优化</title>

<!-- 文章页 -->
<title>长尾关键词完整指南：如何找到并优化高转化长尾词 | 谷歌 SEO 博客</title>

<!-- 产品页 -->
<title>Yoast SEO Premium 插件 - 官方授权中文站 | 谷歌 SEO 博客</title>

<!-- 关于页 -->
<title>关于我们 - 团队介绍 | 谷歌 SEO 博客</title>
```

**原则五：包含可识别的符号提升可读性**

适当使用分隔符和特殊符号可以让 Title 在搜索结果中更醒目：

```html
<title>✅ 2024年最新！WordPress SEO 清单（40项全）</title>
<title>🔥 限时免费：SEO 审计工具包下载</title>
<title>? 什么是 SEO？5 分钟带你彻底理解搜索引擎优化</title>
```

> 注：这类特殊符号可能看起来醒目，但不应过度使用。谷歌也会评估 Title 的专业性，过于夸张的写法可能适得其反。

### 16.2.3 Title 标签的常见错误

| 错误类型 | 示例 | 问题 | 修正建议 |
|--------|------|------|---------|
| 关键词堆砌 | `<title>SEO SEO SEO 优化优化优化 服务服务</title>` | 触发算法惩罚 | 精简到自然流畅的句子 |
| 所有页面相同 | 所有页面都是 `<title>我的网站</title>` | 无法区分页面主题 | 每页独立撰写 |
| 过长被截断 | 超过 60 字符 | 信息不完整 | 精简到 60 字符以内 |
| 缺少关键词 | `<title>欢迎访问我们的网站</title>` | 错失排名机会 | 加入目标关键词 |
| 无品牌标识 | `<title>首页</title>` | 无品牌辨识度 | 添加品牌名称 |

---

## 16.3 Meta Description 标签（描述标签）

### 16.3.1 描述标签的作用

虽然 Meta Description（描述标签）本身不是直接的排名因素，但它对 SEO 的间接影响非常显著：

1. **决定搜索结果摘要**：描述内容会作为搜索结果的摘要显示（并非总是，但通常如此），直接影响用户是否点击
2. **影响点击率（CTR）**：一个写得好的描述可以将 CTR 提升数倍
3. **补充关键词信号**：描述中出现的关键词会以高亮形式显示在搜索结果中，强化相关度感知
4. **社交分享默认文本**：在没有 Open Graph 标签时，许多社交平台会使用 Description 作为分享摘要

### 16.3.2 描述标签的撰写技巧

**技巧一：在前 150 字符内包含核心信息**

移动端搜索结果中，描述通常只显示约 120 个字符。因此最核心的信息——页面的独特价值主张——必须放在最前面。

```html
<!-- 推荐写法：核心信息在前 -->
<meta name="description" content="本指南详解谷歌 SEO 的完整流程，从关键词研究、
                                  内容优化到外链建设，提供 50+ 实战技巧。
                                  免费下载 SEO 检查清单，立即提升网站排名！">

<!-- 这个描述的前 50 字："本指南详解谷歌 SEO 的完整流程，从关键词研究、内容优化到外链建设" -->
<!-- 用户在仅看到截断版本时也能理解页面价值 -->
```

**技巧二：包含明确的行动号召（CTA）**

在描述中加入行动号召可以显著提升点击意愿：

```html
<meta name="description" content="想知道你的网站 SEO 健康度？使用我们的免费工具，
                                  60 秒内获得完整审计报告，包含可执行优化建议。立即检测 →">

<meta name="description" content="免费领取！包含 200 个高搜索量长尾关键词的完整清单，
                                  覆盖电商、教育、SaaS 三大行业。下载后可直接用于内容规划。">
```

**技巧三：针对搜索意图定制描述**

不同搜索意图下的描述应有不同侧重点：

```html
<!-- 信息型搜索意图 -->
<meta name="description" content="什么是反向链接？本文详细解释外链的定义、类型、
                                  如何获取高质量外链，以及常见的外链陷阱。
                                  附赠 10 个免费外链获取方法。">

<!-- 交易型搜索意图 -->
<meta name="description" content="Shopify SEO 应用商店排名上升 300% 的秘密：
                                  专业 Shopify SEO 服务，月费仅 ¥2999，
                                  无效果不收费。已有 500+ 电商网站选择。立即咨询 →">

<!-- 导航型搜索意图 -->
<meta name="description" content="Google Analytics 4 官方帮助中心：完整的 GA4
                                  安装配置教程、数据分析指南和常见问题解答。">
```

**技巧四：包含关键词但避免堆砌**

描述中的关键词出现会让其在搜索结果中高亮显示，增强视觉吸引力和相关性感知：

```html
<!-- 自然融入关键词 -->
<meta name="description" content="外贸网站 SEO 优化从零开始：涵盖技术 SEO 设置、
                                  Google Search Console 配置、多语言关键词研究，
                                  附赠外贸 SEO 模板和检查清单。">

<!-- 差的写法：生硬堆砌 -->
<meta name="description" content="SEO 优化 SEO 服务 SEO 技巧 SEO 工具 SEO 软件
                                  SEO 教程 SEO 培训 SEO 公司，专业 SEO 优化...">
```

### 16.3.3 描述标签的长度控制

| 平台 | 推荐字符数 |
|------|---------|
| 桌面端搜索结果 | 155-160 字符 |
| 移动端搜索结果 | 120-130 字符 |
| Twitter 卡片摘要 | 200 字符 |

**实用建议**：撰写描述时以 155 字符为目标，同时确保在前 120 字符内传达核心信息。这样无论桌面端还是移动端用户，都能获得完整的信息。

---

## 16.4 Meta Keywords 标签（关键词标签）

### 16.4.1 Keywords 标签的现状

这是一个需要明确的历史知识点：**Meta Keywords 标签在现代 SEO 中已基本失去意义**。

谷歌早在 2009 年就公开声明，Keywords 标签不参与排名计算。Matt Cutts（谷歌前 Webspam 主管）更是在多次公开演讲中表示，Keywords 标签"不值得浪费时间"。

**为什么仍然有一些 SEO 工具显示关键词标签？**
这是工具的遗留功能，并非谷歌的实际排名因素。很多老的 SEO 软件（如一些站长工具）仍然读取并展示这个标签的数据，但这些数据对排名没有任何影响。

```html
<!-- 你仍然可以填写，但不要指望它提升排名 -->
<meta name="keywords" content="SEO, 谷歌优化, 搜索引擎优化, 网站排名">

<!-- 更重要的是：把关键词优化工作放在 URL、正文、H 标签和 Alt 文本中 -->
```

**例外情况**：对于一些小众搜索引擎（如百度、有道的早期版本），Keywords 标签可能仍有一定权重。但对于以谷歌为目标搜索引擎的网站，完全可以忽略此标签。

---

## 16.5 H1 标签

### 16.5.1 H1 标签的权重地位

H1 标签在页面所有可见内容中的权重仅次于 Title 标签，排在第二位。谷歌通过解析 H1 标签快速判断页面的核心主题，因此 H1 标签与 Title 标签在内容上应保持高度一致。

**H1 标签的 SEO 特性：**
- 每个页面只能有一个 H1 标签（标准 HTML 规范）
- H1 中包含的核心关键词被视为页面最重要的关键词信号
- 谷歌会分析 H1 与 Title、URL 之间的语义一致性
- H1 通常是用户在页面上看到的第一行"标题文字"

### 16.5.2 H1 标签的正确设置

```html
<!-- 正确示例：H1 包含核心关键词，与 Title 一致 -->
<title>WordPress SEO 完整教程：10 个步骤让谷歌爱上你的网站</title>
<h1>WordPress SEO 完整教程：10 个步骤让谷歌爱上你的网站</h1>

<!-- 错误示例：H1 与 Title 无关 -->
<title>WordPress SEO 完整教程</title>
<h1>如何搭建一个成功的博客网站</h1>  <!-- 主题不一致！ -->

<!-- 错误示例：多个 H1 -->
<h1>主要标题</h1>
<h1>另一个主要标题</h1>  <!-- 不符合规范！ -->

<!-- 错误示例：H1 中堆砌多个关键词 -->
<h1>SEO | SEO 优化 | SEO 技巧 | SEO 服务 | SEO 公司 | 专业 SEO</h1>
```

**H1 标签的字符数建议**：通常不超过 70 个字符（或 35 个汉字）。过长的 H1 在移动端显示时会被截断，影响用户体验和关键词强调效果。

### 16.5.3 H1 与 Title 的协同策略

| 场景 | Title | H1 |
|------|-------|-----|
| 博客文章 | `标题 + 品牌名` | `标题`（不含品牌） |
| 首页 | `品牌口号` | `品牌名` 或 `品牌口号` |
| 产品页 | `产品名 + 型号 + 品牌` | `产品名` |
| 分类页 | `分类名 + 产品数量 + 品牌` | `分类名` |

```html
<!-- 博客文章的 Title 和 H1 配合示例 -->
<title>如何做关键词竞争分析（附免费工具）| SEO 研究所</title>
<body>
  <h1>如何做关键词竞争分析（附免费工具）</h1>
  <!-- 注意：H1 中不需要重复品牌名，Title 中已包含 -->
</body>
```

---

## 16.6 H2/H3 层级标签

### 16.6.1 层级标签的 SEO 作用

H2 和 H3 标签构成了页面的次级内容结构，它们向搜索引擎传达：
- 页面内容的主要子主题是什么
- 各子主题之间的逻辑关系和层次
- 哪些内容片段与特定关键词相关

**标签层级的数学关系**：H1 > H2 > H3 > H4 > H5 > H6
- H1 是最高级别，每页仅一个
- H2 是 H1 的子主题，可以有多个
- H3 是 H2 的子主题，依此类推
- 谷歌期望看到层级关系是连续的（不要跳级）

### 16.6.2 层级标签的使用规范

```html
<h1>独立站 SEO 完整指南（2024）</h1>

<!-- H2 定义主要章节 -->
<h2>一、独立站 SEO 与平台电商 SEO 的区别</h2>

  <!-- H3 定义子章节 -->
  <h3>1.1 独立站 SEO 的独特挑战</h3>
  <h3>1.2 为什么独立站更需要 SEO</h3>

<h2>二、技术 SEO 基础设置</h2>

  <h3>2.1 网站速度优化</h3>
  <h3>2.2 移动端适配</h3>
  <h3>2.3 HTTPS 与安全证书</h3>

  <h3>2.4 结构化数据标记</h3>
  <!-- H3 嵌套在 H2 之下，正确 -->

<!-- 错误示例：跳级使用标签 -->
<h1>主标题</h1>
<h3>直接使用 H3，没有 H2</h3>  <!-- 错误：跳过了 H2 -->

<!-- 错误示例：H4 比 H3 更重要 -->
<h1>主标题</h1>
<h2>第二章</h2>
<h4>比第二章更重要的内容</h4>  <!-- 错误：层级混乱 -->
```

### 16.6.3 在子标题中自然融入关键词

H2/H3 子标题是布局长尾关键词的绝佳位置。每个子标题应围绕一个具体的子主题展开，同时自然包含相关的关键词变体：

```html
<h1>外贸网站 SEO 优化指南</h1>

<h2>外贸网站关键词研究方法</h2>
  <h3>如何用 Google Keyword Planner 找到高价值关键词</h3>
  <h3>外贸长尾关键词挖掘的 5 个技巧</h3>

<h2>B2B 外贸网站内容营销策略</h2>
  <h3>如何撰写符合国外买家习惯的产品描述</h3>
  <h3>外贸博客内容规划：月度日历模板分享</h3>
```

---

## 16.7 图片 Alt 文本

### 16.7.1 Alt 文本的多重价值

图片的 Alt 属性（Alternative Text）在 SEO 中具有不可替代的作用，它服务于三个不同的目的：

1. **无障碍访问（Accessibility）**：屏幕阅读器会朗读 Alt 文本，帮助视障用户理解图片内容。这是《Web Content Accessibility Guidelines》（WCAG）2.1 标准的基本要求。
2. **图片搜索排名**：谷歌通过 Alt 文本来理解图片内容，从而决定图片在 Google Images 中的排名。
3. **SEO 关键词补充**：Alt 文本是页面内容中自然融入关键词的辅助渠道。

### 16.7.2 Alt 文本的书写规范

```html
<!-- 优秀 Alt 文本：描述图片内容 + 包含关键词 -->
<img src="/images/seo-checklist-2024.jpg"
     alt="2024年 SEO 检查清单，包含技术 SEO、内容 SEO、外链建设
          三大模块共 50 个检查项，可免费下载 PDF 版本"
     width="800" height="600">

<!-- 可接受的 Alt 文本：描述图片内容，不含营销语气 -->
<img src="/images/team-photo.jpg"
     alt="SEO 研究所团队合影，左起：张三（SEO 总监）、李四（内容总监）、
          王五（技术负责人）"
     width="600" height="400">

<!-- 装饰性图片：空 Alt -->
<img src="/images/decorative-divider.svg" alt="">
<!-- 注意：空 Alt（alt=""）表示这张图片是纯装饰性的，不需要被朗读 -->

<!-- Logo：品牌名 + 页面关系 -->
<img src="/images/company-logo.svg" alt="SEO 研究所 Logo">
<img src="/images/nav-logo.png" alt="返回 SEO 研究所首页">
```

### 16.7.3 Alt 文本的常见错误

| 错误类型 | 示例 | 问题 | 正确写法 |
|---------|------|------|--------|
| 关键词堆砌 | `alt="SEO SEO 优化 服务 公司 专业"` | 触发垃圾内容识别 | 描述图片内容 |
| 与图片无关 | 图片是产品图，Alt 是公司名称 | 误导用户和搜索引擎 | 描述图片中的内容 |
| 使用文件名代替 | `alt="DSC_00123.jpg"` | 文件名无意义 | 描述图片内容 |
| 过长描述 | 超过 125 个字符的详细描述 | 不必要的冗长 | 简洁明了，125 字以内 |
| 图片无 Alt | `<img src="...">` 无 alt 属性 | 可访问性问题，图片无法被理解 | 添加描述性 alt 属性 |

---

## 16.8 Canonical 标签（规范链接标签）

### 16.8.1 Canonical 标签的作用与原理

Canonical 标签（`<link rel="canonical">`）是解决重复内容问题最强大的工具。当一个页面可以通过多个不同的 URL 访问时（比如带 www 和不带 www、带 session ID、带 UTM 参数等），Canonical 标签告诉搜索引擎："这些不同的 URL 实际上都指向同一个内容，请将排名权重集中在这个规范 URL 上。"

```html
<!-- 在页面的 <head> 中添加 -->
<link rel="canonical" href="https://example.com/canonical-page-url">

<!-- 示例：一个产品在分类页和搜索结果页都能访问 -->
<!-- https://example.com/product/blue-widget          （规范版本）-->
<!-- https://example.com/product/blue-widget?ref=newsletter -->
<!-- https://example.com/product/blue-widget?utm_source=email -->

<!-- 在后两个 URL 的页面中，应加入： -->
<link rel="canonical" href="https://example.com/product/blue-widget">
```

### 16.8.2 常见需要使用 Canonical 的场景

| 场景 | 示例 | Canonical 设置 |
|------|------|--------------|
| HTTP 和 HTTPS 版本 | `http://example.com` 和 `https://example.com` | HTTPS 版本设为规范 |
| www 和非 www | `www.example.com` 和 `example.com` | 选择一个作为规范 |
| 带/不带尾部斜杠 | `example.com/page` 和 `example.com/page/` | 选择一个作为规范 |
| 打印版页面 | `example.com/article` 和 `example.com/article/print` | 主版本设为规范 |
| 分页内容 | `example.com/category/seo?page=1/2/3` | 首页设为规范 |
| AMP 版本 | `example.com/article` 和 `example.com/article/amp` | 通常指向主版本 |
| 带追踪参数 | `example.com/page?utm_source=...` | 原始 URL 设为规范 |

### 16.8.3 Canonical 标签的错误使用及后果

**错误一：将 Canonical 指向不相关的页面**

```html
<!-- 错误示例：将产品页的 Canonical 指向首页 -->
<link rel="canonical" href="https://example.com/">
<!-- 这会导致产品页失去自己的排名能力 -->

<!-- 正确做法 -->
<link rel="canonical" href="https://example.com/product/widget-blue">
```

**错误二：Canonical 自我引用时指向错误 URL**

```html
<!-- 错误：页面 Canonical 指向自己，但 URL 本身有大小写问题 -->
<!-- 页面 URL: https://Example.com/Page -->
<!-- Canonical: <link rel="canonical" href="https://example.com/page"> -->
<!-- 问题：自我引用的 URL 与实际 URL 不一致 -->

<!-- 正确：确保 Canonical 与页面实际 URL 完全一致 -->
<link rel="canonical" href="https://example.com/page">
```

**错误三：在已被 robots 禁止抓取的页面上设置 Canonical**

```html
<!-- 错误组合 -->
<meta name="robots" content="noindex, nofollow">
<link rel="canonical" href="https://example.com/page">

<!-- robots 告诉搜索引擎不要索引此页面 -->
<!-- 同时又用 Canonical 说"这个页面是规范页面" -->
<!-- 这两个指令相互矛盾，Canonical 会被忽略 -->
```

**错误四：混合使用 Canonical 和 301 重定向**

```html
<!-- 如果页面有多个 URL 版本 -->
<!-- https://www.example.com/page  (有 www) -->
<!-- https://example.com/page      (无 www) -->

<!-- 不应该同时做两件事： -->
<!-- 1. 设置 Canonical 指向无 www 版本 -->
<!-- 2. 对有 www 版本做 301 重定向到无 www 版本 -->

<!-- 应该只选择一种方案：优先使用 301 重定向（更明确）-->
```

### 16.8.4 Canonical 与 Hreflang 的配合

对于多语言网站，Canonical 需要与 Hreflang 标签配合使用：

```html
<link rel="canonical" href="https://example.com/zh-cn/seo-guide">
<link rel="alternate" hreflang="zh-CN" href="https://example.com/zh-cn/seo-guide">
<link rel="alternate" hreflang="en-US" href="https://example.com/en-us/seo-guide">
<link rel="alternate" hreflang="zh-TW" href="https://example.com/zh-tw/seo-guide">
```

---

## 16.9 Nofollow 标签

### 16.9.1 Nofollow 的发展历史与现状

Nofollow 标签经历了从诞生到演变的完整历程，理解这段历史有助于正确使用这一标签。

**2005 年**：谷歌、微软和雅虎联合推出了 `rel="nofollow"` 属性，作为对抗垃圾评论链接（Comment Spam）的工具。

**2019 年**：谷歌将 Nofollow 升级为"提示"（Hints），而非严格的指令。这意味着谷歌可能仍然会参考 Nofollow 链接的内容，只是权重传递效果有限。

**2024 年**：在新的链接属性体系中，Nofollow 有三种相关属性：
- `rel="nofollow"`：不要将这个链接视为投票
- `rel="sponsored"`：这是一个付费或赞助的链接（替代原来的 UGC 值）
- `rel="ugc"`：这是用户生成内容中的链接（如评论区、论坛帖子）
- `rel="noopener"`：安全属性，防止新页面访问 window.opener

```html
<!-- 标准 Nofollow：不要传递权重 -->
<a href="https://example.com/external-page" rel="nofollow">这是一个nofollow链接</a>

<!-- Sponsored：付费/赞助内容 -->
<a href="https://partner.com/product" rel="sponsored">赞助商产品</a>

<!-- UGC：用户生成内容 -->
<a href="https://forum.example.com/topic/123" rel="ugc">论坛帖子中的链接</a>

<!-- 组合使用 -->
<a href="https://example.com" rel="nofollow sponsored">这是一个付费链接且不传递权重</a>

<!-- Noopener：安全属性（通常与 Nofollow/Novistor 组合使用）-->
<a href="https://external-site.com" target="_blank" rel="noopener noreferrer">打开外部链接</a>
```

### 16.9.2 Nofollow 在权重分配中的实际作用

**重要认知**：Nofollow 链接并非"毫无价值"。在现代 SEO 实践中，Nofollow 链接在权重分配和爬虫引导方面仍然发挥着重要作用。

**场景一：控制内部权重流动**

在某些情况下，你不希望所有页面都获得均等的内部链接权重。通过给低价值页面添加 Nofollow，可以将爬虫的抓取预算引导到更重要的页面：

```html
<!-- 示例：隐私政策页和条款页不需要获得排名 -->
<nav>
  <a href="/">首页</a>
  <a href="/about">关于我们</a>
  <a href="/products">产品</a>
  <a href="/blog">博客</a>
  <a href="/privacy-policy" rel="nofollow">隐私政策</a>   <!-- Nofollow -->
  <a href="/terms" rel="nofollow">使用条款</a>            <!-- Nofollow -->
</nav>
```

**场景二：付费合作的链接处理**

所有付费链接（无论是直接的购买链接还是付费评论、赞助内容）都必须添加 `rel="sponsored"` 属性。不添加将直接触发谷歌的手动惩罚：

```html
<!-- 付费合作文章中的外链 -->
<p>我在测评中使用的是 <a href="https://affiliate-tool.com" rel="sponsored">这款 SEO 工具</a>，
   这是我多年的主力工具。</p>
```

**场景三：Nofollow 作为内部链接策略的一部分**

在某些 SEO 策略中，给特定类型的内部链接加 Nofollow，可以集中权重到目标页面：

```html
<!-- 示例：用户注册/登录页面不参与整体权重流动 -->
<a href="/login" rel="nofollow">登录</a>
<a href="/register" rel="nofollow">注册</a>
<a href="/cart">购物车</a>   <!-- 电商站，购物车页通常是转化页 -->
```

### 16.9.3 正确的 Nofollow 使用场景

| 是否使用 Nofollow | 场景 | 原因 |
|:----------------:|------|------|
| 是 | 付费/赞助链接 | 谷歌明确要求，否则面临惩罚 |
| 是 | 用户生成内容（评论、论坛、社交帖子） | 防止垃圾内容操控排名 |
| 是 | 登录/注册页面 | 不需要搜索排名，节省抓取预算 |
| 是 | 低价值页面（隐私政策、条款声明） | 将权重集中在高价值内容上 |
| 是 | 同一网站内的重复内容页面 | 集中权重到主版本 |
| 否 | 真实编辑推荐（合作伙伴、专业引用） | 正常的编辑判断，应传递权重 |
| 否 | 高价值的内容页面 | 争取排名机会 |

---

## 16.10 综合元标签检查清单

完成所有元标签设置后，使用以下清单进行最终审查：

```html
<head>
  <!-- [ ] Title 标签：包含核心关键词，不超过 60 字符，每页唯一 -->
  <title>核心关键词 - 修饰词 | 品牌名</title>

  <!-- [ ] Meta Description：包含关键词和 CTA，不超过 155 字符，每页唯一 -->
  <meta name="description" content="描述内容...">

  <!-- [ ] Keywords 标签：可选填写，不作为主要优化依据 -->
  <meta name="keywords" content="关键词1, 关键词2">

  <!-- [ ] Canonical 标签：所有页面都要有 -->
  <link rel="canonical" href="https://example.com/canonical-url">

  <!-- [ ] Robots 标签：通常默认 index, follow -->
  <meta name="robots" content="index, follow">

  <!-- [ ] Viewport 标签：响应式设计必需 -->
  <meta name="viewport" content="width=device-width, initial-scale=1.0">

  <!-- [ ] Open Graph 标签：社交分享优化 -->
  <meta property="og:title" content="分享标题">
  <meta property="og:description" content="分享描述">
  <meta property="og:image" content="https://example.com/share-image.jpg">
  <meta property="og:url" content="https://example.com/page-url">

  <!-- [ ] Twitter Card 标签 -->
  <meta name="twitter:card" content="summary_large_image">
  <meta name="twitter:title" content="分享标题">
  <meta name="twitter:description" content="分享描述">
  <meta name="twitter:image" content="https://example.com/share-image.jpg">

  <!-- [ ] 字符编码 -->
  <meta charset="UTF-8">
</head>
```

**关键提醒**：
1. 元标签设置是基础中的基础，错误设置会导致整个 SEO 策略失效
2. Canonical 和 Title 是最容易出错且后果最严重的两个标签，需要特别仔细检查
3. 元标签需要随内容更新而同步更新，保持一致性
4. 定期使用 Google Search Console 检测元标签相关的警告和建议

下一章我们将深入探讨内部链接的艺术，这是决定网站整体 SEO 表现的核心技术环节。
