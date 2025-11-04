# Implementation Plan: EIE官网原型完善与图片素材整理

**Feature Branch**: `001-prd-eie`
**Created**: 2025-11-04
**Based on**: spec.md (v1.0)

---

## 📋 Technical Context

### Project Overview
本项目需要基于现有的 `eie-homepage-complete.html` 原型,对照 PRD 文档进行完善,并生成详细的图片素材需求清单。项目的核心目标是为 Canada Post 全球邮政联盟会议准备展示材料。

### Technology Stack
- **Frontend Framework**: 静态 HTML/CSS/JavaScript (根据 constitution 要求)
- **UI Framework**: 自定义组件,参考 Global Freight Solutions 设计风格
- **图片格式**: WebP (主) + JPEG (备用)
- **图标系统**: SVG 图标或 Lucide/Font Awesome
- **部署**: 静态托管 (Netlify/Vercel/GitHub Pages)

### Key Dependencies
- 现有原型文件: `eie-homepage-complete.html`
- 图片存储路径: `/Users/david/ai开发项目/eiedemo官网/page`
- PRD 文档: `EIE_Website_PRD.md`
- 品牌色彩系统: 蓝色渐变 (#1e3a8a to #3b82f6) + 橙色强调 (#f97316)

### Integration Points
- 无外部 API 集成 (当前阶段为静态展示)
- 图片路径需指向 `/page` 目录结构
- 后续可能需要集成 Google Analytics

### Unknown/Needs Clarification
- ✅ 是否已有 EIE Logo 和 Canada Post Logo 授权文件?
- ✅ 现有原型 `eie-homepage-complete.html` 的完成度如何?
- ✅ 是否需要中英文双语版本? (根据 PRD 需要)
- ✅ 图片素材制作工具偏好? (AI 生成工具选择: Midjourney/DALL-E/Stable Diffusion)
- ✅ 部署域名是否已确定?

---

## ✅ Constitution Check

### Core Principles Alignment

#### I. Professional Presentation First (NON-NEGOTIABLE) ✅
- **符合度**: 本项目完全符合专业展示要求
- **验证要点**:
  - ✅ 基于 PRD 的专业设计规范 (蓝色渐变 + 橙色强调)
  - ✅ 数据驱动展示 (500万包裹/年, 99%+ 清关率等)
  - ✅ 移动端响应式设计要求已明确
  - ✅ 跨浏览器兼容性将在实施阶段验证
  - ✅ SEO 优化要求已包含在 PRD 中

#### II. Clear Communication of Capabilities ✅
- **符合度**: PRD 明确定义了所有展示内容
- **验证要点**:
  - ✅ 明确的数据展示要求 (40,000+包裹/日)
  - ✅ 可视化服务流程设计
  - ✅ Canada Post 合作背书突出展示
  - ✅ 清晰的 CTA (Call-to-Action) 按钮设计

#### III. Technical Excellence ✅
- **符合度**: 遵循 constitution 技术约束
- **验证要点**:
  - ✅ 使用静态 HTML/CSS/JavaScript (符合 constitution)
  - ✅ 语义化 HTML5 标记
  - ✅ WebP 图片格式优化
  - ✅ W3C 标准合规性将在验证阶段确认

#### IV. Fast Iteration & Deployment ✅
- **符合度**: 4天交付时间线可行
- **验证要点**:
  - ✅ 静态网站架构,无复杂构建流程
  - ✅ 简单的内容更新机制
  - ✅ 易于部署到静态托管平台

#### V. Content Accuracy (NON-NEGOTIABLE) ⚠️
- **符合度**: 需要在实施阶段验证数据准确性
- **行动项**:
  - ⚠️ 确认所有业务数据与实际运营匹配
  - ⚠️ 验证 Canada Post 合作关系的准确表述
  - ⚠️ 核实所有服务承诺(2-9天妥投等)

### Technology Constraints Compliance ✅

#### Approved Technology Stack
- ✅ **Markup**: HTML5 with semantic elements
- ✅ **Styling**: CSS3 with Grid, Flexbox, Custom Properties
- ✅ **Framework**: Vanilla JavaScript (无 React/Vue/Angular)
- ✅ **Images**: WebP format with JPEG fallback
- ✅ **Icons**: SVG icons or icon fonts
- ✅ **Deployment**: Static hosting (Netlify/Vercel/GitHub Pages)

### Quality Gates Status
**当前阶段**: Phase 1 - 设计与规划

**必须通过的质量门**:
1. ⏳ W3C HTML/CSS validation (将在实施阶段验证)
2. ⏳ Lighthouse score >90 (将在实施阶段验证)
3. ⏳ Mobile-friendly test (将在实施阶段验证)
4. ⏳ 跨浏览器测试 (将在实施阶段验证)
5. ⏳ 内容准确性验证 (需在设计阶段确认)
6. ✅ PRD 要求覆盖率 (本计划已覆盖)

---

## 🔬 Phase 0: Outline & Research

### Research Tasks Identified

基于 Technical Context 中的"NEEDS CLARIFICATION"项,需要进行以下研究:

#### Research Task 1: 现有原型评估
**目标**: 评估 `eie-homepage-complete.html` 的完成度和需要修改的部分
**方法**:
1. 读取并分析现有 HTML 文件
2. 对照 PRD 的 10 个主要 section 检查覆盖率
3. 识别缺失的 section 和需要修改的内容

**预期输出**:
- 现有原型完成度评估报告
- 需要补充的 section 清单
- 需要修改的内容列表

#### Research Task 2: 图片素材需求分析
**目标**: 从 PRD 提取所有图片需求,分类整理
**方法**:
1. 分析 PRD 中所有提及图片的章节
2. 提取图片规格、用途、优先级
3. 为每张图片生成 AI 提示词

**预期输出**:
- 图片需求清单表格 (Markdown 格式)
- 每张图片的 AI 生成提示词
- 图片目录结构设计

#### Research Task 3: 静态网站最佳实践
**目标**: 研究静态 HTML 网站的性能优化和 SEO 最佳实践
**方法**:
1. 研究 WebP 图片优化方案
2. 研究 CSS/JavaScript 压缩最佳实践
3. 研究静态网站 SEO 优化技巧

**预期输出**:
- 性能优化建议清单
- SEO 优化 checklist
- 图片优化工作流程

#### Research Task 4: AI 图片生成工具选择
**目标**: 推荐合适的 AI 图片生成工具
**方法**:
1. 对比 Midjourney, DALL-E 3, Stable Diffusion 的优劣
2. 评估物流行业场景图片生成效果
3. 考虑成本和便利性

**预期输出**:
- AI 工具推荐 (含理由)
- 提示词编写规范
- 示例提示词模板

---

## 📐 Phase 1: Design & Contracts

### Data Model Design

#### Entity 1: 图片素材项 (ImageAsset)

```markdown
**实体名称**: ImageAsset

**字段**:
- id: 唯一标识符 (P0-001, P1-001 等)
- filename: 文件名 (hero-background.webp)
- category: 分类 (hero/services/partners/facilities)
- purpose: 用途说明
- dimensions: 尺寸要求 (1920x1080px)
- format: 格式 (WebP + JPEG fallback)
- priority: 优先级 (P0/P1/P2)
- aiPrompt: AI 生成提示词 (中英文)
- status: 状态 (待制作/已完成/已优化)
- altText: 替代文本 (用于 SEO 和可访问性)

**关系**:
- 属于某个 Section (一对多)
- 可能有多个尺寸变体 (1x, 2x, 3x)

**验证规则**:
- 文件名必须符合命名规范 (小写, 连字符分隔)
- 尺寸必须适配响应式断点
- P0 图片必须优先完成
- AI 提示词必须包含风格、色彩、元素描述
```

#### Entity 2: 网站 Section (WebSection)

```markdown
**实体名称**: WebSection

**字段**:
- id: Section 编号 (S1-Hero, S2-Partnership 等)
- name: Section 名称
- priority: 重要性 (P0/P1/P2)
- status: 完成状态 (缺失/部分完成/已完成)
- requiredImages: 所需图片列表
- contentStatus: 文案状态 (已完成/待补充)
- layoutType: 布局类型 (左文右图/2x2网格/时间轴等)

**关系**:
- 包含多个 ImageAsset
- 属于某个页面 (Home/About/Services 等)

**状态流转**:
- 缺失 → 设计中 → 开发中 → 测试中 → 已完成
```

#### Entity 3: 页面目录结构 (PageDirectory)

```markdown
**实体名称**: PageDirectory

**字段**:
- path: 目录路径 (/page/hero, /page/services 等)
- purpose: 用途说明
- imageCount: 包含图片数量
- totalSize: 预估总大小 (MB)
- structure: 子目录结构

**关系**:
- 包含多个 ImageAsset
- 按类型组织 (logo/hero/services/partners 等)

**组织原则**:
- 按功能分类,不超过 5 个一级目录
- 每个目录包含同一用途的图片
- 命名清晰,便于维护
```

### API Contracts

本项目为静态网站,当前阶段无 API 端点。未来可能添加的 API:

```markdown
### Future API (Phase 2)

**POST /api/contact**
- 功能: 提交商务咨询表单
- 请求体:
  {
    "name": "string",
    "company": "string",
    "email": "string",
    "phone": "string",
    "service": "string[]",
    "volume": "string",
    "message": "string"
  }
- 响应:
  {
    "success": boolean,
    "messageId": "string"
  }

**GET /api/tracking/{trackingNumber}**
- 功能: 查询包裹轨迹
- 响应:
  {
    "trackingNumber": "string",
    "status": "string",
    "timeline": [...]
  }
```

### Generated Artifacts

**本阶段将生成以下文档**:

1. **research.md** - 研究成果汇总
   - 现有原型评估报告
   - 图片素材最佳实践
   - AI 工具选择建议
   - 性能优化方案

2. **data-model.md** - 数据模型定义
   - 图片素材实体模型
   - Section 实体模型
   - 目录结构模型

3. **IMAGE_REQUIREMENTS.md** - 图片需求清单
   - 完整图片需求表格
   - AI 提示词集合
   - 优先级排序
   - 目录结构设计

4. **PROTOTYPE_MODIFICATIONS.md** - 原型修改建议
   - 需要补充的 section
   - 需要修改的内容
   - 路径配置说明
   - 实施步骤指南

5. **quickstart.md** - 快速开始指南
   - 项目设置步骤
   - 图片制作流程
   - 原型修改流程
   - 部署步骤

---

## 🎯 Success Criteria Mapping

### From spec.md

#### Measurable Outcome: SC-001
**要求**: 原型完善后包含 PRD 要求的所有 10 个 section,无遗漏
**验证方式**:
- Phase 0: 生成 section 覆盖率检查清单
- Phase 1: 标注每个 section 的完成状态
**目标值**: 100% 覆盖率

#### Measurable Outcome: SC-002
**要求**: 图片需求清单涵盖至少 18 张核心图片 (P0+P1 级别)
**验证方式**:
- Phase 1: 生成图片需求清单,统计 P0+P1 数量
**目标值**: ≥ 18 张

#### Measurable Outcome: SC-003
**要求**: 每张图片的 AI 提示词长度在 100-300 字之间
**验证方式**:
- Phase 1: 检查每个提示词的字数
**目标值**: 100% 的提示词符合字数要求

#### Measurable Outcome: SC-004
**要求**: 清单以 Markdown 表格格式交付,可直接复制使用
**验证方式**:
- Phase 1: 生成 Markdown 表格,验证格式正确性
**目标值**: Markdown 格式正确,表格完整

#### Measurable Outcome: SC-005
**要求**: page 目录结构清晰,图片分类不超过 5 个一级目录
**验证方式**:
- Phase 1: 设计目录结构,统计一级目录数量
**目标值**: ≤ 5 个一级目录

#### Measurable Outcome: SC-006
**要求**: 原型修改建议具体可操作,开发者可直接实施
**验证方式**:
- Phase 1: 生成修改建议文档,包含具体步骤
**目标值**: 每条建议包含明确的操作步骤

#### Measurable Outcome: SC-007
**要求**: 优先级标注清晰,P0 图片不超过 12 张
**验证方式**:
- Phase 1: 统计 P0 图片数量
**目标值**: P0 ≤ 12 张

#### Measurable Outcome: SC-008
**要求**: 所有图片尺寸规格符合 web 标准,适配响应式设计
**验证方式**:
- Phase 1: 定义响应式断点和图片尺寸规格
**目标值**: 所有尺寸规格明确定义

---

## 🚀 Next Steps

### Immediate Actions (Phase 0)

1. **启动研究任务**
   - [ ] 读取并分析 `eie-homepage-complete.html`
   - [ ] 提取 PRD 中所有图片需求
   - [ ] 研究 AI 图片生成工具
   - [ ] 研究静态网站优化最佳实践

2. **生成研究报告**
   - [ ] 创建 `research.md`
   - [ ] 解决所有 NEEDS CLARIFICATION 项
   - [ ] 记录技术决策和理由

### Phase 1 Preparation

1. **设计数据模型**
   - [ ] 创建 `data-model.md`
   - [ ] 定义图片素材实体
   - [ ] 定义 Section 实体
   - [ ] 设计目录结构

2. **生成需求文档**
   - [ ] 创建 `IMAGE_REQUIREMENTS.md` (图片需求清单)
   - [ ] 创建 `PROTOTYPE_MODIFICATIONS.md` (原型修改建议)
   - [ ] 创建 `quickstart.md` (快速开始指南)

3. **更新 Agent Context**
   - [ ] 运行 `.specify/scripts/bash/update-agent-context.sh claude`
   - [ ] 添加项目特定的技术栈信息
   - [ ] 保留手动添加的内容

---

## 📊 Risk Assessment

### High Priority Risks

#### Risk 1: 图片素材制作时间不足
**可能性**: 中
**影响**: 高
**缓解措施**:
- 优先制作 P0 级别图片
- 使用 AI 生成工具加快制作速度
- 准备占位符图片作为备选

#### Risk 2: 原型与 PRD 差异过大
**可能性**: 中
**影响**: 中
**缓解措施**:
- Phase 0 先评估差异程度
- 识别必须补充的 section
- 制定清晰的修改优先级

#### Risk 3: 图片优化影响性能
**可能性**: 低
**影响**: 中
**缓解措施**:
- 严格遵循图片尺寸规范
- 使用 WebP 格式压缩
- 实施懒加载策略

---

## 🔄 Constitution Re-evaluation (Post-Design)

**将在 Phase 1 完成后重新评估**:

- ✅ 是否所有设计决策符合 Constitution 原则?
- ✅ 是否遵守了技术约束?
- ✅ 质量门标准是否清晰定义?
- ✅ 是否有任何需要例外处理的情况?

---

**Plan Version**: 1.0
**Last Updated**: 2025-11-04
**Next Review**: Phase 0 完成后
