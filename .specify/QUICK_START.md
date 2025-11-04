# SpecKit 快速开始指南

> 针对 EIE 官网项目的 SpecKit 使用说明

## 🎯 核心命令（8个）

### 1. `/speckit.constitution`
**用途**: 查看项目宪章
**使用场景**: 了解项目的核心原则和技术约束
**示例**:
```bash
/speckit.constitution
```

### 2. `/speckit.specify`
**用途**: 创建功能规范
**使用场景**: 开发新功能、优化现有功能、逆向工程分析
**示例**:
```bash
# 开发新页面
/speckit.specify 创建国内物流力量页面，包括航权资源、揽收网络、分拣能力和查验流程四个板块

# 优化现有页面
/speckit.specify [优化] 提升首页 Lighthouse 性能评分到95+，优化图片加载和CSS

# 分析现有代码
/speckit.specify [逆向工程] 分析当前网站的 SEO 优化和可访问性合规情况
```

### 3. `/speckit.clarify`
**用途**: 澄清需求
**使用场景**: 需求不明确时，提出问题进行澄清
**示例**:
```bash
# 在创建规范后，如有疑问
/speckit.clarify
```

### 4. `/speckit.plan`
**用途**: 创建实施计划
**使用场景**: 将规范转化为具体的实施步骤
**示例**:
```bash
# 在规范明确后
/speckit.plan
```

### 5. `/speckit.tasks`
**用途**: 生成任务列表
**使用场景**: 创建详细的任务清单，便于跟踪进度
**示例**:
```bash
# 在计划确定后
/speckit.tasks
```

### 6. `/speckit.implement`
**用途**: 实施功能
**使用场景**: 开始实际的代码编写工作
**示例**:
```bash
# 在任务清单准备好后
/speckit.implement
```

### 7. `/speckit.checklist`
**用途**: 生成质量检查清单
**使用场景**: 验证功能质量，确保符合项目标准
**示例**:
```bash
# 在实施完成后
/speckit.checklist
```

### 8. `/speckit.analyze`
**用途**: 分析代码质量
**使用场景**: 评估代码质量，发现潜在问题
**示例**:
```bash
# 对任何代码进行质量分析
/speckit.analyze
```

## 📋 标准工作流程

### 场景 A: 开发新页面/功能
```bash
1. /speckit.specify 创建[功能名称]，包括[功能描述]
2. /speckit.clarify  （如有疑问）
3. /speckit.plan
4. /speckit.tasks
5. /speckit.implement
6. /speckit.checklist
```

### 场景 B: 优化现有页面
```bash
1. /speckit.specify [优化] 提升[页面名称]的[优化目标]
2. /speckit.plan
3. /speckit.implement
4. /speckit.checklist
```

### 场景 C: 质量检查和分析
```bash
1. /speckit.specify [逆向工程] 分析[目标内容]
2. /speckit.analyze
3. /speckit.checklist
```

## 🎨 EIE 官网特定规则

### 设计规范
- **主色调**: 蓝色渐变 (#1e3a8a → #3b82f6)
- **强调色**: 橙色 (#f97316)
- **字体**: Inter 或 Open Sans
- **布局**: 左文右图

### 性能要求
- 页面加载 < 3秒
- Lighthouse 分数 > 90
- 图片大小 < 200KB
- 总页面大小 < 3MB

### 质量门控
1. W3C HTML/CSS 验证通过（零错误）
2. Lighthouse 评分 > 90（性能、可访问性、最佳实践、SEO）
3. 移动友好测试通过
4. 多浏览器测试通过（Chrome, Safari, Firefox）

## 💡 实用提示

### 提示 1: 使用描述性的规范标题
✅ 好的示例:
```bash
/speckit.specify 创建"关于我们"页面，包括公司简介、设施展示、资质认证和联系方式四个板块
```

❌ 不好的示例:
```bash
/speckit.specify 做一个页面
```

### 提示 2: 善用标签
- `[优化]` - 性能或质量优化
- `[重构]` - 代码重构
- `[逆向工程]` - 分析现有代码
- `[修复]` - Bug 修复

### 提示 3: 逐步推进
不要跳过步骤，按照标准流程逐步推进：
规范 → 计划 → 任务 → 实施 → 检查

### 提示 4: 参考宪章
遇到疑问时，随时查看项目宪章：
```bash
/speckit.constitution
```

## 🔗 相关文档

- **完整说明**: `.specify/README.md`
- **更新日志**: `.specify/CHANGELOG.md`
- **项目宪章**: `.specify/memory/constitution.md`
- **PRD 文档**: `EIE_Website_PRD.md`

## ❓ 常见问题

**Q: 什么时候使用 `/speckit.clarify`？**
A: 当规范创建后，如果有任何不清楚的地方，立即使用此命令。

**Q: 是否必须按顺序执行所有命令？**
A: 对于新功能开发，建议按标准流程。对于小优化，可以跳过某些步骤。

**Q: 如何确保符合项目质量标准？**
A: 始终运行 `/speckit.checklist` 进行质量验证。

**Q: 可以同时处理多个功能吗？**
A: 可以，但建议一次专注一个功能，确保质量。

---

**需要帮助？** 查看 `.specify/README.md` 获取更详细的说明。
