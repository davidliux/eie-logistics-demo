# Research Report: EIE官网原型完善与图片素材整理

**Generated**: 2025-11-04
**Phase**: Phase 0 - Outline & Research
**Status**: Completed

---

## 📊 Executive Summary

本研究报告针对 EIE 官网项目的原型完善和图片素材需求进行了全面调研。主要发现:

✅ **原型完成度**: 现有原型 `eie-homepage-complete.html` 已包含 PRD 要求的所有 10 个 section,结构完整
✅ **目录结构**: `/page` 目录已存在,包含基本分类结构
✅ **技术栈**: 使用 Tailwind CSS + Vanilla JS,符合 constitution 要求
⚠️ **需要改进**: 色彩方案需调整为 PRD 规定的深蓝色系,图片占位符需替换为实际素材

---

## 🔍 Research Task 1: 现有原型评估

### 原型文件分析

**文件**: `eie-homepage-complete.html`
**总行数**: 802 行
**技术栈**:
- Tailwind CSS (CDN 版本)
- Material Symbols Outlined 图标
- Inter 字体
- Vanilla JavaScript

### Section 覆盖率检查

根据 PRD 要求的 10 个主要 section,现有原型覆盖情况:

| Section | PRD 要求 | 原型状态 | 完成度 | 备注 |
|---------|---------|---------|--------|------|
| S1 - Hero Area | ✅ 必需 | ✅ 已完成 | 90% | 色彩需调整,需替换图片 |
| S2 - Canada Post Partnership | ✅ 必需 | ✅ 已完成 | 80% | Canada Post Logo 为占位符 |
| S3 - Why Choose EIE | ✅ 必需 | ✅ 已完成 | 95% | 四大优势卡片完整 |
| S3.5 - Global Direct Ecommerce | ✅ 必需 | ✅ 已完成 | 75% | 6张核心图片均为占位符 |
| S4 - Service Flow | ✅ 必需 | ✅ 已完成 | 85% | 时间轴结构完整 |
| S5 - Competitive Advantages | ✅ 必需 | ✅ 已完成 | 90% | 文案完整 |
| S6 - By The Numbers | ✅ 必需 | ✅ 已完成 | 95% | 数据展示完整 |
| S7 - Technology | ✅ 必需 | ✅ 已完成 | 90% | 技术能力描述完整 |
| S8 - Network Map | ✅ 必需 | ✅ 已完成 | 70% | 地图为占位符,需实际地图 |
| S9 - Partners | ✅ 必需 | ✅ 已完成 | 60% | 合作伙伴 Logo 为占位符 |
| S10 - CTA | ✅ 必需 | ✅ 已完成 | 95% | CTA 按钮完整 |

**总体完成度**: 85%
**结论**: ✅ 所有 section 结构完整,主要需要替换图片素材和调整色彩

### 色彩方案对比

**原型当前色彩**:
```css
primary: #64B5F6 (浅蓝色)
background-light: #F8F8F8
secondary-element: #BBDEFB (极浅蓝)
```

**PRD 要求色彩**:
```css
--primary-navy: #0A2647 (深海军蓝)
--primary-blue: #144272 (标准蓝)
--accent-orange: #FF9500 (橙色强调)
```

**差异分析**:
- ❌ 当前使用浅蓝色系,PRD 要求深蓝色系
- ❌ 缺少橙色强调色
- ✅ 整体布局和结构符合要求

**修改建议**:
1. 替换 Tailwind 配置中的 `primary` 颜色为 `#0A2647`
2. 添加 `accent-orange: #FF9500` 作为 CTA 按钮颜色
3. 更新所有使用 `bg-primary` 的元素
4. 将 `Get Started` 按钮改为橙色背景

### 图片占位符统计

**占位符数量**: 15 个

**占位符分类**:
1. **Hero 区域**: 1 个 (背景图片,当前使用 Unsplash 链接)
2. **Global Direct Ecommerce**: 6 个 (前段物流3张 + 末端服务3张)
3. **Network Map**: 2 个 (中国地图 + 加拿大地图)
4. **Partners**: 5 个 (Canada Post + 4个派送伙伴)
5. **Logo**: 1 个 (EIE Logo,已使用 SVG 占位符)

**需要替换的图片**: 14 张实际图片 + 1 个 Logo 优化

### 现有目录结构

```
/page/
├── hero/           (Hero 背景图片)
├── logo/           (EIE Logo)
├── network/        (地图素材)
├── partners/       (合作伙伴 Logo)
└── services/       (服务场景图片)
    ├── china-ops/  (前段物流)
    └── canada-ops/ (末端服务)
```

**结构评估**: ✅ 符合要求,分类清晰,不超过 5 个一级目录

---

## 🎨 Research Task 2: 图片素材需求分析

### 图片总需求统计

根据 PRD 和原型分析,总计需要以下图片素材:

| 优先级 | 数量 | 说明 |
|--------|------|------|
| **P0 (必须)** | 10 张 | 核心业务展示图片 |
| **P1 (重要)** | 8 张 | 增强展示效果 |
| **P2 (可选)** | 5 张 | 锦上添花 |
| **总计** | 23 张 | - |

### P0 级别图片清单 (必须,共10张)

#### 1. Hero 背景图片
- **文件名**: `hero-background.webp` (+ `.jpg` fallback)
- **路径**: `/page/hero/`
- **尺寸**: 1920x1080px (16:9)
- **用途**: Hero 区域背景,奠定专业物流形象
- **风格**: 集装箱货轮场景,蓝色调
- **AI 提示词** (见详细清单章节)

#### 2-4. 前段物流场景 (中国运营)

**2. 飞机航空运输**
- **文件名**: `china-ops-aircraft.webp`
- **路径**: `/page/services/china-ops/`
- **尺寸**: 800x600px (4:3)
- **用途**: 展示国际航空运输能力

**3. 航班调度看板**
- **文件名**: `china-ops-schedule.webp`
- **路径**: `/page/services/china-ops/`
- **尺寸**: 800x600px
- **用途**: 体现专业运营管理

**4. 分拣中心场景**
- **文件名**: `china-ops-sorting.webp`
- **路径**: `/page/services/china-ops/`
- **尺寸**: 800x600px
- **用途**: 展现智能分拣能力

#### 5-7. 末端服务场景 (加拿大运营)

**5. 清关文件/CBSA 认证**
- **文件名**: `canada-ops-customs.webp`
- **路径**: `/page/services/canada-ops/`
- **尺寸**: 800x600px
- **用途**: 展示专业清关资质

**6. 末端仓库内景**
- **文件名**: `canada-ops-warehouse.webp`
- **路径**: `/page/services/canada-ops/`
- **尺寸**: 800x600px
- **用途**: 体现本地化服务能力

**7. 派送车辆**
- **文件名**: `canada-ops-delivery.webp`
- **路径**: `/page/services/canada-ops/`
- **尺寸**: 800x600px
- **用途**: 展示多元派送网络

#### 8-9. 地图素材

**8. 中国地图**
- **文件名**: `china-network-map.svg` (或 `.png`)
- **路径**: `/page/network/`
- **尺寸**: 800x600px
- **用途**: 标注 15+ 城市网络

**9. 加拿大地图**
- **文件名**: `canada-network-map.svg`
- **路径**: `/page/network/`
- **尺寸**: 800x600px
- **用途**: 标注服务覆盖范围

#### 10. Canada Post Logo
- **文件名**: `canada-post-logo.png` (+ `.svg` if available)
- **路径**: `/page/partners/`
- **尺寸**: 高度 80px (矢量最佳)
- **用途**: 合作背书展示
- **注意**: ⚠️ 需获得使用授权

### P1 级别图片清单 (重要,共8张)

#### 11. EIE Logo 优化版
- **文件名**: `eie-logo.svg` + `eie-logo.png`
- **路径**: `/page/logo/`
- **尺寸**: 矢量 (导出多尺寸: 32px, 64px, 128px, 256px)
- **用途**: 导航栏、页脚、品牌展示
- **当前状态**: 已有基础 SVG,需优化为品牌色系

#### 12-15. 合作伙伴 Logo

**12. Purolator Logo**
- **文件名**: `partner-purolator.png`
- **路径**: `/page/partners/`
- **尺寸**: 高度 60-80px,透明背景

**13. DHL Logo**
- **文件名**: `partner-dhl.png`
- **路径**: `/page/partners/`

**14. UPS Logo**
- **文件名**: `partner-ups.png`
- **路径**: `/page/partners/`

**15. FedEx Logo**
- **文件名**: `partner-fedex.png`
- **路径**: `/page/partners/`

#### 16-18. 设施照片

**16. 中国仓库外观**
- **文件名**: `facility-china-warehouse.webp`
- **路径**: `/page/services/china-ops/`
- **尺寸**: 1200x800px
- **用途**: About 页面展示

**17. 加拿大清关中心**
- **文件名**: `facility-canada-clearance.webp`
- **路径**: `/page/services/canada-ops/`
- **尺寸**: 1200x800px

**18. Eagleship 配送车辆**
- **文件名**: `eagleship-vehicle.webp`
- **路径**: `/page/partners/`
- **尺寸**: 800x600px
- **用途**: 突出自营派送网络

### P2 级别图片清单 (可选,共5张)

19-23. 团队照片、办公环境、其他装饰性图片

(详细清单见 IMAGE_REQUIREMENTS.md)

---

## 🤖 Research Task 3: AI 图片生成工具选择

### 工具对比分析

| 工具 | 优点 | 缺点 | 适用场景 | 推荐度 |
|------|------|------|----------|--------|
| **Midjourney** | • 图片质量最高<br>• 风格多样<br>• 物流场景效果好 | • 需付费 ($10-30/月)<br>• 需 Discord 操作 | 高质量商业图片 | ⭐⭐⭐⭐⭐ |
| **DALL-E 3** | • ChatGPT Plus 内置<br>• 操作简单<br>• 文字渲染准确 | • 创意性稍弱<br>• 需 GPT Plus ($20/月) | 快速原型制作 | ⭐⭐⭐⭐ |
| **Stable Diffusion** | • 完全免费<br>• 高度可控 | • 需本地部署<br>• 学习曲线陡 | 技术用户 | ⭐⭐⭐ |
| **Firefly (Adobe)** | • 商业授权明确<br>• 与 Adobe 生态整合 | • 创意性一般<br>• 需 Adobe 订阅 | 企业合规需求 | ⭐⭐⭐⭐ |

### 推荐方案

#### **主力工具: Midjourney**

**理由**:
1. ✅ 图片质量最高,物流行业场景渲染逼真
2. ✅ 支持高分辨率输出 (适合 web 使用)
3. ✅ 风格一致性好,适合成套制作
4. ✅ 商业授权明确 (付费版本可商用)

**成本**: $30/月 (标准计划,约 15 小时 GPU 时间)

#### **备选工具: DALL-E 3**

**理由**:
1. ✅ 快速迭代,适合原型测试
2. ✅ 文字提示词理解准确
3. ✅ 如果已有 ChatGPT Plus 无额外成本

**适用**: 快速生成概念图、占位符优化

### AI 提示词编写规范

根据物流行业特点,提示词应包含以下要素:

**1. 主题描述** (What)
- 明确说明场景内容
- 示例: "A modern air cargo loading scene at an international airport"

**2. 风格要求** (Style)
- 专业商业摄影风格
- 示例: "professional corporate photography, high quality, sharp focus"

**3. 色彩方案** (Color)
- 符合品牌色系
- 示例: "blue tones, #0A2647 navy blue gradient, orange accents #FF9500"

**4. 关键元素** (Elements)
- 必须包含的视觉元素
- 示例: "cargo plane, shipping containers, workers in safety vests"

**5. 构图比例** (Composition)
- 指定画面比例和角度
- 示例: "16:9 aspect ratio, wide angle view, horizontal composition"

**6. 氛围与情感** (Mood)
- 传达的专业感和可信度
- 示例: "professional, trustworthy, modern, efficient, clean"

### 提示词模板示例

```
[Subject]: A modern air cargo loading scene at an international airport
[Details]: Large cargo aircraft being loaded with shipping containers,
professional ground crew in safety vests, modern airport facilities
[Style]: professional corporate photography, high quality commercial shoot,
sharp focus, natural lighting
[Color]: blue tones matching #0A2647 navy blue, clean whites,
subtle orange accents #FF9500
[Composition]: 16:9 aspect ratio, wide angle view showing scale of operations,
horizontal composition
[Mood]: professional, trustworthy, modern, efficient, dynamic
[Technical]: 8K resolution, photorealistic, detailed textures,
no text overlays, cinematic lighting
```

---

## ⚡ Research Task 4: 静态网站性能优化最佳实践

### 图片优化方案

#### 1. 格式选择策略

**优先级顺序**:
1. **WebP**: 主格式 (体积减少 25-35%)
2. **JPEG**: 备用格式 (兼容性最佳)
3. **SVG**: 矢量图形 (Logo、图标)

**实施方案**:
```html
<picture>
  <source srcset="hero-background.webp" type="image/webp">
  <img src="hero-background.jpg" alt="描述文本">
</picture>
```

#### 2. 响应式图片

**断点定义**:
```
Mobile:  < 640px  → 提供 800px 宽度图片
Tablet:  640-1024px → 提供 1200px 宽度图片
Desktop: > 1024px → 提供 1920px 宽度图片
```

**实施方案**:
```html
<img srcset="image-800.webp 800w,
             image-1200.webp 1200w,
             image-1920.webp 1920w"
     sizes="(max-width: 640px) 800px,
            (max-width: 1024px) 1200px,
            1920px"
     src="image-1200.jpg"
     alt="描述">
```

#### 3. 压缩规格

| 图片类型 | 压缩目标 | 质量设置 |
|---------|---------|---------|
| Hero 背景 | < 200KB | 80-85% |
| 服务场景 | < 150KB | 80% |
| Logo/图标 | < 50KB | 90% (SVG 优先) |
| 合作伙伴 | < 30KB | 85% |

**推荐工具**:
- **在线**: TinyPNG, Squoosh
- **本地**: ImageOptim (Mac), XnConvert
- **批量**: `imagemin` (Node.js)

#### 4. 懒加载策略

**原生懒加载**:
```html
<img src="image.webp" loading="lazy" alt="描述">
```

**关键规则**:
- ✅ 首屏图片 (Hero): `loading="eager"`
- ✅ 折叠下方图片: `loading="lazy"`
- ✅ 关键 Logo: 不使用懒加载

### CSS 优化

#### 1. 关键 CSS 内联

**策略**: 将首屏渲染必需的 CSS 内联到 `<head>` 中

**Tailwind CSS 优化**:
- 生产环境使用本地构建版本 (而非 CDN)
- 启用 PurgeCSS 移除未使用的样式
- 预计体积: 从 ~3MB CDN → ~50KB 优化版

#### 2. 字体优化

**当前使用**: Google Fonts - Inter
**优化方案**:
```html
<!-- 预连接 -->
<link rel="preconnect" href="https://fonts.googleapis.com">
<link rel="preconnect" href="https://fonts.gstatic.com" crossorigin>

<!-- 仅加载必需字重 -->
<link href="https://fonts.googleapis.com/css2?family=Inter:wght@400;500;700;900&display=swap" rel="stylesheet">
```

**或使用系统字体**:
```css
font-family: -apple-system, BlinkMacSystemFont, "Segoe UI", ...
```

### JavaScript 优化

#### 当前状态
- Tailwind CSS 从 CDN 加载 (~200KB)
- Material Symbols 图标 (~50KB)

#### 优化建议
1. **生产构建**: 使用本地 Tailwind 构建
2. **图标**: 仅内联使用的 SVG 图标
3. **延迟加载**: 非关键 JS 使用 `defer` 或 `async`

### SEO 优化清单

#### 1. Meta 标签

```html
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">

  <!-- SEO 核心标签 -->
  <title>EIE Logistics - Canada Post Strategic Partner | Cross-border Ecommerce Solutions</title>
  <meta name="description" content="EIE Logistics, Canada Post's trusted partner, handles 5M+ parcels annually. Professional customs clearance, 99%+ success rate, 2-9 days delivery. Contact us today.">

  <!-- Open Graph (社交分享) -->
  <meta property="og:title" content="EIE Logistics - Global Direct Ecommerce Solutions">
  <meta property="og:description" content="Trusted by Canada Post. 5 Million parcels annually.">
  <meta property="og:image" content="/page/hero/og-image.jpg">
  <meta property="og:url" content="https://www.eie-logistics.com">

  <!-- Twitter Card -->
  <meta name="twitter:card" content="summary_large_image">
</head>
```

#### 2. 语义化 HTML

- ✅ 使用 `<header>`, `<main>`, `<section>`, `<footer>`
- ✅ `<h1>` 仅一次,`<h2>`-`<h6>` 层级清晰
- ✅ 所有图片包含 `alt` 属性
- ✅ 链接包含描述性文字 (避免"点击这里")

#### 3. Schema Markup

```html
<script type="application/ld+json">
{
  "@context": "https://schema.org",
  "@type": "Organization",
  "name": "EIE Logistics",
  "url": "https://www.eie-logistics.com",
  "logo": "https://www.eie-logistics.com/page/logo/eie-logo.png",
  "description": "Cross-border logistics solutions, Canada Post strategic partner",
  "address": {
    "@type": "PostalAddress",
    "addressCountry": "CA"
  },
  "sameAs": [
    "https://www.linkedin.com/company/eie-logistics"
  ]
}
</script>
```

### 性能目标

根据 Constitution 要求:

| 指标 | 目标值 | 当前评估 |
|------|--------|---------|
| Page Load Time | < 3s (4G) | ⏳ 待测试 |
| First Contentful Paint | < 1.5s | ⏳ 待测试 |
| Largest Contentful Paint | < 2.5s | ⏳ 待测试 |
| Cumulative Layout Shift | < 0.1 | ⏳ 待测试 |
| Total Page Size | < 3MB | ⏳ 待测试 |
| Lighthouse Score | > 90 (各项) | ⏳ 待测试 |

**优化后预估**:
- HTML: ~50KB
- CSS: ~50KB (优化后的 Tailwind)
- JavaScript: ~20KB
- 图片: ~1.5MB (10张优化后的 WebP)
- **总计**: ~1.6MB ✅ 低于 3MB 目标

---

## 📋 决策记录

### Decision 1: 色彩方案调整
**决策**: 将原型色彩从浅蓝色系调整为 PRD 规定的深蓝色系
**理由**: 符合专业物流形象,增强视觉冲击力
**实施**: 修改 Tailwind 配置,替换所有 `bg-primary` 类

### Decision 2: AI 图片生成工具
**决策**: 主力使用 Midjourney,备选 DALL-E 3
**理由**: 质量最高,适合商业展示
**成本**: $30/月 (可接受)

### Decision 3: 图片格式
**决策**: WebP (主) + JPEG (备用)
**理由**: 平衡性能和兼容性
**实施**: 使用 `<picture>` 标签渐进式增强

### Decision 4: 静态托管
**决策**: 推荐 Vercel 或 Netlify
**理由**:
- 免费额度充足
- 自动 HTTPS
- 全球 CDN
- 简单部署

---

## ✅ 研究成果总结

### 已解决的 NEEDS CLARIFICATION

1. ✅ **原型完成度**: 85% 完成,所有 section 结构完整
2. ✅ **目录结构**: 已存在,符合要求
3. ✅ **双语版本**: 当前为英文,中文版本需后续添加
4. ✅ **AI 工具**: 推荐 Midjourney + DALL-E 3 组合
5. ✅ **部署方案**: Vercel/Netlify 静态托管

### 关键发现

1. **原型质量高**: 结构完整,布局合理,仅需素材替换和色彩调整
2. **图片需求明确**: 10 张 P0 图片,18 张 P0+P1 图片,符合 SC-002 要求
3. **性能优化路径清晰**: WebP 格式 + 懒加载 + Tailwind 优化
4. **SEO 基础良好**: 语义化 HTML 已就位,需补充 meta 标签

### 下一步行动

1. ✅ 生成详细的图片需求清单 (IMAGE_REQUIREMENTS.md)
2. ✅ 生成原型修改建议 (PROTOTYPE_MODIFICATIONS.md)
3. ✅ 生成数据模型文档 (data-model.md)
4. ✅ 生成快速开始指南 (quickstart.md)

---

**Research Completed**: 2025-11-04
**Next Phase**: Phase 1 - Design & Contracts
