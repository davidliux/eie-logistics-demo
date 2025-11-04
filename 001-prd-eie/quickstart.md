# Quick Start Guide: EIE官网原型完善与图片素材整理

**Generated**: 2025-11-04
**Feature**: 001-prd-eie
**Estimated Time**: 2-3 天

---

## 📋 概述

本指南提供了完成 EIE 官网原型的分步说明,包括图片素材制作、原型修改和最终部署。按照本指南,您可以在 2-3 天内完成所有工作。

---

## 🎯 前置准备

### 必需工具

| 工具 | 用途 | 获取方式 | 成本 |
|------|------|---------|------|
| **Midjourney** | AI 图片生成 (主力) | midjourney.com | $30/月 |
| **ChatGPT Plus** | AI 图片生成 (备选 DALL-E 3) | openai.com | $20/月 |
| **TinyPNG** | 图片压缩优化 | tinypng.com | 免费 |
| **VS Code** | 代码编辑器 | code.visualstudio.com | 免费 |
| **Chrome DevTools** | 测试和调试 | chrome.google.com | 免费 |
| **Git** | 版本控制 | git-scm.com | 免费 |

### 可选工具

- **Figma**: 设计预览和协作 (免费版足够)
- **Squoosh**: 图片格式转换 (app.squoosh.app, 免费)
- **ImageOptim**: Mac 图片批量优化 (免费)

### 环境检查

```bash
# 检查 Git 是否安装
git --version

# 检查 Node.js 是否安装 (可选,用于未来优化)
node --version

# 检查当前项目目录
pwd
# 应该输出: /Users/david/ai开发项目/eiedemo官网
```

---

## 📂 项目结构

```
eiedemo官网/
├── 001-prd-eie/                    # 项目文档目录
│   ├── spec.md                     # 功能规格
│   ├── plan.md                     # 实施计划
│   ├── research.md                 # 研究报告
│   ├── data-model.md               # 数据模型
│   ├── quickstart.md               # 本文档
│   ├── IMAGE_REQUIREMENTS.md       # 图片需求清单 ⭐
│   └── PROTOTYPE_MODIFICATIONS.md  # 原型修改指南 ⭐
│
├── page/                           # 图片存储目录 ⭐
│   ├── hero/                       # Hero 背景图
│   ├── logo/                       # Logo 资产
│   ├── services/                   # 服务场景图
│   │   ├── china-ops/              # 前段物流 (3张)
│   │   └── canada-ops/             # 末端服务 (3张)
│   ├── network/                    # 地图素材
│   └── partners/                   # 合作伙伴 Logo
│
├── eie-homepage-complete.html      # 原型文件 ⭐
├── EIE_Website_PRD.md              # 产品需求文档
└── README.md                       # 项目说明

⭐ = 核心文件,需频繁访问
```

---

## 🚀 三天工作流程

### 📅 Day 1: 图片素材制作 (8 小时)

#### **上午 (4h): P0 级别图片生成**

**步骤 1: 准备 AI 提示词** (30 分钟)

1. 打开 `001-prd-eie/IMAGE_REQUIREMENTS.md`
2. 复制 P0 级别的 10 个 AI 提示词到笔记本
3. 按优先级排序 (Hero 背景 → 前段物流 → 末端服务)

**步骤 2: Midjourney 批量生成** (3 小时)

1. 登录 Midjourney Discord
2. 使用 `/imagine` 命令,逐个输入提示词
3. 对于每张图片:
   - 生成 4 个变体
   - 选择最佳版本 (U1-U4)
   - Upscale 到高分辨率
   - 下载原图

**示例命令**:
```
/imagine A modern container ship at sea during golden hour, deep navy blue ocean #0A2647, cargo containers in blue and orange tones #FF9500, professional maritime photography, wide angle view, 16:9 aspect ratio, cinematic lighting, photorealistic, 8K quality, no text overlays --ar 16:9 --v 6
```

**输出**: 10 张原始图片 (保存到临时文件夹)

**步骤 3: 图片优化** (30 分钟)

1. 访问 tinypng.com
2. 上传所有图片,压缩到 WebP 格式
3. 下载压缩后的图片
4. 使用 Squoosh 转换为 WebP + JPEG 双格式

#### **下午 (4h): P1 级别图片 + Logo 优化**

**步骤 4: 合作伙伴 Logo 收集** (1 小时)

1. 搜索各公司官方 Logo 下载页面:
   - Canada Post: canadapost.ca (需授权)
   - Purolator: purolator.com/media
   - DHL: dhl.com/press
   - UPS: ups.com/media
   - FedEx: fedex.com/brand

2. 下载 PNG 格式 (透明背景)
3. 统一调整高度为 80px

**步骤 5: 地图素材制作** (1 小时)

使用以下工具之一:
- **选项 A**: mapchart.net (在线地图编辑器,免费)
- **选项 B**: DALL-E 3 生成简化地图
- **选项 C**: 手绘 + Figma 标注

**步骤 6: EIE Logo 优化** (30 分钟)

1. 打开现有 `/page/logo.png`
2. 使用 Figma 或 Illustrator:
   - 调整色彩为品牌深蓝 #0A2647
   - 导出 SVG 格式
   - 导出多尺寸 PNG (32, 64, 128, 256px)

**步骤 7: 图片组织** (1.5 小时)

1. 按照 `data-model.md` 定义的目录结构组织文件
2. 重命名文件为规范名称 (小写+连字符)
3. 生成响应式变体 (800w, 1200w, 1920w)
4. 验证文件大小符合限制

```bash
# 检查图片大小
ls -lh page/services/china-ops/

# 应该看到类似输出:
# -rw-r--r--  1 user  staff   145K  china-ops-aircraft.webp
# -rw-r--r--  1 user  staff   180K  china-ops-aircraft.jpg
```

---

### 📅 Day 2: 原型修改 (8 小时)

#### **上午 (4h): 色彩方案调整**

**步骤 8: 修改 Tailwind 配置** (1 小时)

打开 `eie-homepage-complete.html`,找到 `<script id="tailwind-config">`:

```javascript
// 替换原有配置
tailwind.config = {
    darkMode: "class",
    theme: {
        extend: {
            colors: {
                // 深蓝色系 (主色调)
                'primary-navy': '#0A2647',
                'primary-blue': '#144272',
                'primary-light': '#205295',
                'primary-sky': '#2C74B3',

                // 橙色系 (强调色)
                'accent-orange': '#FF9500',
                'accent-orange-light': '#FFB340',
                'accent-orange-dark': '#E68600',

                // 保留原有辅助色
                'background-light': '#F8F8F8',
                'secondary-element': '#BBDEFB',
                'dark-gray-text': '#333333',
                'medium-gray-text': '#555555',
            },
            fontFamily: {
                display: "Inter"
            },
            borderRadius: {
                DEFAULT: "0.25rem",
                lg: "0.5rem",
                xl: "0.75rem",
                full: "9999px"
            }
        }
    }
};
```

**步骤 9: 替换颜色类名** (2 小时)

使用 VS Code 全局替换:

1. `bg-primary` → `bg-primary-navy` (导航栏、深色背景)
2. `text-primary` → `text-primary-blue` (标题、重点文字)
3. 所有 "Get Started" 按钮:
   - `bg-primary` → `bg-accent-orange`
   - `hover:bg-primary/90` → `hover:bg-accent-orange-light`

**步骤 10: Hero 区域渐变背景** (1 小时)

找到 Hero Section,添加渐变背景:

```html
<section class="relative py-16 sm:py-20 lg:py-24 px-4 sm:px-6 lg:px-8 xl:px-40"
         style="background: linear-gradient(135deg, #0A2647 0%, #144272 50%, #205295 100%);">
    <!-- Hero 内容 -->
</section>
```

#### **下午 (4h): 图片路径替换**

**步骤 11: 替换 Hero 背景图** (30 分钟)

找到:
```html
<div class="w-full h-full bg-center bg-no-repeat bg-cover rounded-xl"
     style='background-image: url("https://images.unsplash.com/photo-1566576721346-d4a3b4eaeb55?w=800");'>
</div>
```

替换为:
```html
<picture>
    <source srcset="page/hero/hero-background-800.webp 800w,
                    page/hero/hero-background-1200.webp 1200w,
                    page/hero/hero-background-1920.webp 1920w"
            type="image/webp">
    <div class="w-full h-full bg-center bg-no-repeat bg-cover rounded-xl"
         style='background-image: url("page/hero/hero-background-1920.jpg");'>
    </div>
</picture>
```

**步骤 12: 替换服务场景图片** (2 小时)

Global Direct Ecommerce Section (S3.5):

前段物流 3 张图:
```html
<!-- 飞机航空运输 -->
<div class="aspect-video bg-gray-300">  <!-- 删除这行 -->
    <span class="text-gray-600">Aircraft Loading</span>  <!-- 删除这行 -->
</div>

<!-- 替换为: -->
<picture>
    <source srcset="page/services/china-ops/china-ops-aircraft.webp" type="image/webp">
    <img src="page/services/china-ops/china-ops-aircraft.jpg"
         alt="Modern air cargo loading scene - EIE international air transport"
         class="w-full h-full object-cover rounded-xl"
         loading="lazy">
</picture>
```

对另外 5 张图片重复此操作。

**步骤 13: 替换 Logo** (1 小时)

1. **Canada Post Logo** (S2):
```html
<div class="h-16 w-48 bg-gray-300 rounded flex items-center justify-center">
    <span class="text-dark-gray-text font-bold">Canada Post Logo</span>
</div>

<!-- 替换为: -->
<img src="page/partners/canada-post-logo.png"
     alt="Canada Post Logo"
     class="h-16 w-auto"
     loading="eager">
```

2. **EIE Logo** (Header):
```html
<!-- 替换现有 SVG 为实际 Logo -->
<img src="page/logo/eie-logo.svg"
     alt="EIE Logistics Logo"
     class="h-6 w-auto">
```

3. **合作伙伴 Logo 墙** (S9):
```html
<!-- 替换所有占位符为实际 Logo -->
<div class="flex justify-center gap-8 flex-wrap">
    <img src="page/partners/partner-purolator.png" alt="Purolator" class="h-12">
    <img src="page/partners/partner-dhl.png" alt="DHL" class="h-12">
    <img src="page/partners/partner-ups.png" alt="UPS" class="h-12">
    <img src="page/partners/partner-fedex.png" alt="FedEx" class="h-12">
</div>
```

**步骤 14: 地图替换** (30 分钟)

Network Section (S8):
```html
<img src="page/network/china-network-map.svg"
     alt="EIE China network coverage - 15+ cities"
     class="w-full h-auto">

<img src="page/network/canada-network-map.svg"
     alt="EIE Canada service coverage"
     class="w-full h-auto">
```

---

### 📅 Day 3: 测试与部署 (6 小时)

#### **上午 (3h): 质量检查**

**步骤 15: 本地测试** (1 小时)

1. 打开 `eie-homepage-complete.html` 在浏览器
2. 检查清单:
   - [ ] 所有图片正常加载 (无 404)
   - [ ] 色彩符合 PRD 要求 (深蓝色系 + 橙色)
   - [ ] CTA 按钮为橙色
   - [ ] Hero 背景渐变正确
   - [ ] 所有 Logo 清晰显示

**步骤 16: 响应式测试** (1 小时)

使用 Chrome DevTools (F12 → Toggle Device Toolbar):
- [ ] Mobile (375px): 单列布局正常
- [ ] Tablet (768px): 2 列布局正常
- [ ] Desktop (1280px): 完整布局正常
- [ ] Large (1920px): 无横向滚动

**步骤 17: 性能测试** (1 小时)

1. 打开 Chrome DevTools → Lighthouse
2. 运行测试 (Desktop + Mobile)
3. 检查指标:
   - [ ] Performance > 90
   - [ ] Accessibility > 90
   - [ ] Best Practices > 90
   - [ ] SEO > 90

如果未达标,参考 `research.md` 的优化建议。

#### **下午 (3h): 部署准备**

**步骤 18: 添加 SEO Meta 标签** (1 小时)

在 `<head>` 中添加:

```html
<!-- 基础 SEO -->
<title>EIE Logistics - Canada Post Strategic Partner | Cross-border Ecommerce Solutions</title>
<meta name="description" content="EIE Logistics, Canada Post's trusted partner, handles 5M+ parcels annually. Professional customs clearance, 99%+ success rate, 2-9 days delivery.">
<meta name="keywords" content="cross-border logistics, Canada Post, customs clearance, ecommerce shipping, China to Canada">

<!-- Open Graph -->
<meta property="og:title" content="EIE Logistics - Global Direct Ecommerce Solutions">
<meta property="og:description" content="Trusted by Canada Post. 5 Million parcels annually. 99%+ customs clearance success rate.">
<meta property="og:image" content="page/hero/hero-background-1920.jpg">
<meta property="og:url" content="https://www.eie-logistics.com">
<meta property="og:type" content="website">

<!-- Twitter Card -->
<meta name="twitter:card" content="summary_large_image">
<meta name="twitter:title" content="EIE Logistics - Global Ecommerce Solutions">
<meta name="twitter:description" content="Canada Post strategic partner. 5M parcels/year.">
<meta name="twitter:image" content="page/hero/hero-background-1920.jpg">
```

**步骤 19: 创建 Git 仓库** (30 分钟)

```bash
cd /Users/david/ai开发项目/eiedemo官网

# 初始化 Git (如果尚未初始化)
git init

# 添加所有文件
git add .

# 创建首次提交
git commit -m "feat: 完成 EIE 官网原型 - 包含所有图片素材和色彩调整"

# 连接到远程仓库 (可选)
git remote add origin https://github.com/your-username/eie-website.git
git push -u origin main
```

**步骤 20: 部署到 Vercel** (1.5 小时)

1. 访问 vercel.com,使用 GitHub 账号登录
2. 点击 "New Project"
3. 导入 Git 仓库
4. 配置设置:
   - **Framework Preset**: Other (静态 HTML)
   - **Build Command**: (留空)
   - **Output Directory**: . (项目根目录)
5. 点击 "Deploy"

等待部署完成 (~2 分钟)

**步骤 21: 绑定自定义域名** (可选)

1. 在 Vercel 项目设置 → Domains
2. 添加域名: `www.eie-logistics.com`
3. 按照指示配置 DNS (CNAME 记录)
4. 等待 SSL 证书自动配置

---

## ✅ 最终检查清单

### 图片素材 (23 张)

**P0 级别 (10 张)** ✅
- [ ] P0-001: hero-background.webp + .jpg
- [ ] P0-002: china-ops-aircraft.webp + .jpg
- [ ] P0-003: china-ops-schedule.webp + .jpg
- [ ] P0-004: china-ops-sorting.webp + .jpg
- [ ] P0-005: canada-ops-customs.webp + .jpg
- [ ] P0-006: canada-ops-warehouse.webp + .jpg
- [ ] P0-007: canada-ops-delivery.webp + .jpg
- [ ] P0-008: china-network-map.svg
- [ ] P0-009: canada-network-map.svg
- [ ] P0-010: canada-post-logo.png

**P1 级别 (8 张)** ✅
- [ ] P1-011: eie-logo.svg + .png
- [ ] P1-012: partner-purolator.png
- [ ] P1-013: partner-dhl.png
- [ ] P1-014: partner-ups.png
- [ ] P1-015: partner-fedex.png
- [ ] P1-016: facility-china-warehouse.webp
- [ ] P1-017: facility-canada-clearance.webp
- [ ] P1-018: eagleship-vehicle.webp

### 原型修改

**色彩方案** ✅
- [ ] Tailwind 配置更新为深蓝色系
- [ ] 所有 CTA 按钮使用橙色
- [ ] Hero 区域渐变背景应用
- [ ] 导航栏深色主题

**图片路径** ✅
- [ ] 所有占位符替换为实际图片
- [ ] 图片路径指向 `/page` 目录
- [ ] 使用 `<picture>` 标签渐进式增强
- [ ] 所有图片包含 `alt` 属性

**SEO 优化** ✅
- [ ] Meta 标签完整
- [ ] Open Graph 标签添加
- [ ] Twitter Card 配置
- [ ] 语义化 HTML 正确

### 性能与质量

**Lighthouse 分数** ✅
- [ ] Performance > 90
- [ ] Accessibility > 90
- [ ] Best Practices > 90
- [ ] SEO > 90

**跨浏览器测试** ✅
- [ ] Chrome 最新版本
- [ ] Safari 最新版本
- [ ] Firefox 最新版本
- [ ] Edge 最新版本

**响应式设计** ✅
- [ ] Mobile (< 640px)
- [ ] Tablet (640-1024px)
- [ ] Desktop (> 1024px)

### 部署

**Vercel 部署** ✅
- [ ] 项目成功部署
- [ ] HTTPS 自动配置
- [ ] 自定义域名绑定 (可选)
- [ ] 所有页面可访问

---

## 🆘 常见问题

### Q1: Midjourney 生成的图片不符合要求怎么办?

**A**: 尝试以下方法:
1. 调整提示词,增加更具体的描述
2. 使用 `--seed` 参数保持风格一致
3. 使用 Remix 模式微调
4. 备选: 使用 DALL-E 3 或购买 Unsplash+ 商业图片

### Q2: 图片文件太大怎么办?

**A**: 优化步骤:
1. 使用 TinyPNG 压缩 (通常减少 50-70%)
2. 降低 JPEG 质量到 80-85%
3. 调整图片尺寸 (不超过实际显示尺寸的 2 倍)
4. 使用 WebP 格式 (比 JPEG 小 25-35%)

### Q3: 本地测试正常,部署后图片不显示?

**A**: 检查以下项:
1. 图片路径是否正确 (相对路径 `page/...`)
2. 文件名大小写是否一致 (Linux 区分大小写)
3. 图片文件是否已提交到 Git
4. Vercel 部署日志是否有错误

### Q4: Lighthouse 性能分数低于 90?

**A**: 优化建议:
1. 进一步压缩图片 (目标: 总大小 < 1.5MB)
2. 添加懒加载 `loading="lazy"`
3. 使用本地 Tailwind 构建 (代替 CDN)
4. 延迟加载 Material Icons (仅内联使用的图标)

### Q5: 没有 Canada Post Logo 授权怎么办?

**A**: 临时解决方案:
1. 使用文字代替: "Canada Post" (大字体)
2. 联系 Canada Post 品牌部门申请授权
3. 会议演示时口头说明 (Logo 待授权)
4. 使用模糊处理的 Logo (临时)

---

## 📚 参考文档

- **完整图片需求清单**: `001-prd-eie/IMAGE_REQUIREMENTS.md`
- **原型修改详细指南**: `001-prd-eie/PROTOTYPE_MODIFICATIONS.md`
- **研究报告**: `001-prd-eie/research.md`
- **数据模型**: `001-prd-eie/data-model.md`
- **PRD 文档**: `EIE_Website_PRD.md`

---

## 🎉 完成后

恭喜! 您已经完成了 EIE 官网原型的完善。

**下一步**:
1. 📧 通知团队查看部署版本
2. 📊 监控 Google Analytics (如已配置)
3. 📝 收集反馈并记录改进建议
4. 🚀 准备 Canada Post 会议演示

**会议演示技巧**:
- 提前打开网站,确保加载速度快
- 准备备用方案 (录屏视频 / 本地 HTML)
- 重点展示: 数据看板、合作背书、服务流程
- 强调: 5M 包裹、99% 清关率、2-9 天妥投

---

**Quick Start Version**: 1.0
**Last Updated**: 2025-11-04
**Estimated Completion**: 2-3 days
