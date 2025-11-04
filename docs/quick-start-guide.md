# 🚀 EIE 官网快速启动指南

## 📋 项目信息

**项目名称**: EIE Logistics 官网重构
**技术栈**: Next.js 15 + React 19 + TypeScript + Tailwind CSS + Framer Motion
**开发端口**: 5001

---

## 🛠️ 开发环境启动

### 1. 进入项目目录
```bash
cd /Users/david/ai开发项目/eiedemo官网/eie-demo
```

### 2. 安装依赖(如果还未安装)
```bash
npm install
# 或
pnpm install
```

### 3. 启动开发服务器
```bash
npm run dev
# 或
pnpm dev
```

### 4. 访问应用
- **本地**: http://localhost:5001
- **网络**: http://192.168.0.147:5001

---

## 📁 项目结构

```
eie-demo/
├── app/
│   ├── page.tsx          # 首页 - 使用新的 HeroSection
│   ├── layout.tsx        # 根布局 - 包含 Header 和 Footer
│   └── globals.css       # 全局样式
│
├── components/
│   ├── home/             # 🆕 Hero 区域组件
│   │   ├── HeroSection.tsx
│   │   ├── HeroContent.tsx
│   │   ├── HeroVisual.tsx
│   │   ├── BookingCard.tsx
│   │   ├── ReviewCard.tsx
│   │   └── TrackingWidget.tsx
│   │
│   ├── layout/           # 布局组件
│   │   ├── Header.tsx    # 🆕 重构的导航栏
│   │   └── Footer.tsx
│   │
│   └── sections/         # 其他页面区块
│       ├── Partnership.tsx
│       ├── Advantages.tsx
│       ├── ServiceFlow.tsx
│       ├── Stats.tsx
│       ├── CompetitiveAdvantages.tsx
│       ├── Network.tsx
│       └── Contact.tsx
│
├── public/
│   └── images/           # 图片资源目录
│       └── (待添加 EIE 货机照片)
│
├── tailwind.config.ts    # 🆕 更新的配色方案
├── package.json
└── tsconfig.json
```

---

## 🎨 设计系统

### 配色方案

#### 主色调 - 深蓝色系
```typescript
navy: {
  900: '#0A2647',  // 导航、标题
  800: '#144272',  // 背景
  700: '#205295',  // 次要元素
  600: '#2C74B3',  // 装饰、图标
}
```

#### 强调色 - 橙色系
```typescript
orange: {
  600: '#E68600',  // Active状态
  500: '#FF9500',  // 主CTA、重要元素
  400: '#FFB340',  // Hover状态
}
```

### 渐变系统
```css
/* Hero 背景 */
bg-gradient-hero

/* 图片叠加 */
bg-gradient-overlay

/* 按钮渐变 */
bg-gradient-button

/* 卡片渐变 */
bg-gradient-card
```

### 阴影系统
```css
/* 卡片阴影 */
shadow-card / shadow-card-hover

/* 按钮阴影 */
shadow-button / shadow-button-hover

/* 深色卡片 */
shadow-dark-card / shadow-dark-card-hover

/* Header */
shadow-header
```

---

## 🎬 动画时间轴

Hero 区域加载动画序列:

```
0.0s  - 背景渐变淡入
0.4s  - Header 导航淡入下滑
0.6s  - 主标题淡入上滑
0.9s  - 副标题淡入
1.2s  - 按钮组淡入
1.2s  - 评价卡片淡入下滑
1.2s  - 物流追踪淡入
1.4s  - 货柜预订卡片淡入上浮
1.8s  - 物流追踪进度条动画
```

---

## 📱 响应式断点

### Tailwind 默认断点
```typescript
sm: '640px'   // 小型设备
md: '768px'   // 平板
lg: '1024px'  // 桌面
xl: '1280px'  // 大桌面
2xl: '1536px' // 超大屏
```

### 我们的使用策略
- **Mobile** (<768px): 单列布局, 全宽按钮
- **Tablet** (768-1023px): 调整间距和字体
- **Desktop** (≥1024px): 完整的左右分栏布局

---

## 🔧 常用命令

### 开发
```bash
npm run dev          # 启动开发服务器(端口 5001)
npm run build        # 构建生产版本
npm run start        # 启动生产服务器
npm run lint         # 运行 ESLint
```

### Git 工作流
```bash
git status           # 查看状态
git add .            # 添加所有更改
git commit -m "feat: 实现 Hero 区域重构"
git push            # 推送到远程
```

---

## 📝 开发注意事项

### 1. 组件导入路径
使用 `@/` 别名导入:
```typescript
import HeroSection from "@/components/home/HeroSection";
import { Button } from "@/components/ui/button";
```

### 2. 图片处理
使用 Next.js Image 组件:
```typescript
import Image from "next/image";

<Image
  src="/images/eie-cargo-plane.webp"
  alt="EIE Cargo Plane"
  fill
  priority
  quality={85}
/>
```

### 3. Framer Motion 使用
```typescript
import { motion } from "framer-motion";

<motion.div
  initial={{ opacity: 0, y: 20 }}
  animate={{ opacity: 1, y: 0 }}
  transition={{ duration: 0.6, delay: 0.6 }}
>
  内容
</motion.div>
```

### 4. Tailwind 自定义类
优先使用配置中的自定义类:
- `bg-navy-900` 而不是 `bg-[#0A2647]`
- `shadow-card` 而不是自定义 shadow
- `rounded-xl` 而不是 `rounded-[20px]`

---

## 🐛 常见问题

### Q: 服务器无法启动?
**A**: 检查端口 5001 是否被占用:
```bash
lsof -i :5001
kill -9 [PID]
```

### Q: Tailwind 样式不生效?
**A**: 确保文件在 `content` 配置中:
```typescript
// tailwind.config.ts
content: [
  "./app/**/*.{js,ts,jsx,tsx,mdx}",
  "./components/**/*.{js,ts,jsx,tsx,mdx}",
]
```

### Q: 动画不流畅?
**A**: 检查浏览器性能,确保使用 `transform` 和 `opacity`:
```css
/* 好的做法 */
transform: translateY(-2px);
opacity: 0.8;

/* 避免 */
top: -2px;
background-color: rgba(...);
```

---

## 📚 相关文档

- [设计方案](./homepage-redesign-plan.md) - 完整设计规范
- [实施进度](./implementation-progress.md) - 开发进度追踪
- [Next.js 文档](https://nextjs.org/docs)
- [Tailwind CSS 文档](https://tailwindcss.com/docs)
- [Framer Motion 文档](https://www.framer.com/motion/)

---

## 🎯 下一步待办

### 高优先级
- [ ] 添加 EIE 货机背景图片
- [ ] 完善移动端菜单
- [ ] 准备用户头像和图标资源

### 中优先级
- [ ] 性能优化(图片压缩、代码分割)
- [ ] SEO 元数据配置
- [ ] 跨浏览器测试

### 低优先级
- [ ] 添加 Loading 状态
- [ ] 错误边界处理
- [ ] 单元测试

---

## 💡 提示

1. **保持代码风格一致**: 使用 ESLint 和 Prettier
2. **组件化思维**: 每个组件职责单一
3. **性能优先**: 使用 Next.js Image 和 dynamic import
4. **可访问性**: 添加 aria-label 和 alt 属性
5. **移动优先**: 先实现移动端,再扩展桌面端

---

**创建日期**: 2025-11-03
**维护者**: EIE 开发团队
