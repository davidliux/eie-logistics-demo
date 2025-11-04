# EIE 官网产品需求文档 (PRD)

## 📋 项目概述

### 项目背景
EIE作为Canada Post战略合作伙伴，受邀参加全球邮政联盟会议。需要通过官网展示公司在中加跨境邮政物流领域的专业能力，以争取更深度的合作机会和优惠政策支持。

### 核心目标
- **主要目标**：向全球邮政联盟展示EIE的业务承接能力和服务优势
- **次要目标**：作为后续商务洽谈的数字名片，支持业务拓展
- **战略意图**：获得Canada Post低价清关账号，扩大邮政清关业务份额

### 目标受众
- **主受众**：Canada Post高层、全球邮政联盟（UPU）成员
- **次受众**：潜在邮政客户、B2B跨境物流客户
- **决策关注点**：可靠性、规模化能力、成本优势、系统对接能力

### 项目时间线
- **交付时间**：4天（会议前上线）
- **开发周期**：Day1设计 → Day2-3开发 → Day4测试部署

---

## 🎯 核心卖点提炼

### 1. 规模化运营能力
- **年处理量**：500万包裹（Canada Post合作数据）
- **日处理能力**：40,000+包裹
- **规模优势**：证明有能力承接邮政级别业务量

### 2. 端到端服务链路
- **前段**：覆盖中国15+一二线城市直营揽收
- **中段**：多航司资源，灵活调配，无排仓等待
- **后段**：自有清关行（A2Z CUSTOMS）+ 多元派送网络（含自营Eagleship）

### 3. 专业清关实力
- **CBSA认证**清关行
- **99%+**清关通过率
- **2-9天**清关后妥投时效
- **三国团队**：中国+印度+加拿大

### 4. 差异化竞争优势
✓ 价格优势（无DHL/FedEx的旺季附加费和隐藏杂费）  
✓ 灵活性（定制化方案，非标准产品）  
✓ 无排仓等待（自有资源调配）  
✓ 强大分拣能力（应对邮政小包业务）  
✓ 系统对接能力（支持EDI/API，自有tracking系统）

### 5. 服务质量保障
- **客户满意度**：94%+
- **准时妥投**：可追踪承诺
- **24小时客服**：人工+AI混合支持

---

## 🏗️ 网站架构

### 站点地图（新版）
```
Home（首页）★★★★★
│
├── Domestic Logistics（国内物流力量）★★★★★ 【核心板块1】
│   ├── Air Transport Rights（航权资源）
│   ├── Nationwide Collection（揽收网络）
│   ├── Smart Sorting（分拣能力）
│   └── Quality Inspection（查验流程）
│
├── Customs Clearance（清关服务）★★★★★ 【核心板块2】
│   ├── Export Declaration（出口报关）
│   ├── Import Clearance（进口清关）
│   ├── CBSA Certification（CBSA认证）
│   └── Customs Processes（清关流程）
│
├── After-Sales Service（售后服务）★★★★★ 【核心板块3】
│   ├── 24/7 Customer Support（24小时客服）
│   ├── China Warehouse Services（国内仓库服务）
│   ├── Canada Warehouse Services（国外仓库服务）
│   └── Value-Added Services（附加服务）
│
└── About & Contact（关于我们与联系）★★★★ 【核心板块4】
    ├── Company Profile（公司简介）
    ├── Our Facilities（设施展示）
    ├── Certifications（资质认证）
    ├── Contact Information（联系方式）
    └── Business Inquiry（商务咨询）
```

**导航结构说明**：
- **4个主导航标签**：对应4大核心业务板块
- **下拉菜单**：每个标签展开显示子页面
- **星级说明**：★★★★★ 核心页面，★★★★ 重要页面

---

## 📐 首页详细设计（新版设计）

### 整体布局参考
**设计灵感**：参考 Global Freight Solutions 网站设计
- **视觉风格**：专业物流风格，蓝色渐变背景 + 橙色强调
- **布局特点**：左文右图，信息层次清晰，视觉冲击力强

---

### 顶部导航栏（Header）
```
┌────────────────────────────────────────────────────────────────┐
│  [EIE Logo]  [Domestic Logistics ↓] [Customs Clearance ↓]     │
│              [After-Sales ↓] [About & Contact]  [Get a Quote] │
└────────────────────────────────────────────────────────────────┘
```

**设计规范**：
- **Logo位置**：左上角，点击返回首页
- **导航菜单**：4个主标签，带下拉箭头表示有子菜单
- **CTA按钮**：右上角橙色"Get a Quote"按钮（#FF9500）
- **背景色**：深蓝色渐变或半透明（覆盖在Hero背景上）
- **固定导航**：滚动时固定在顶部

---

### Section 1: Hero Area（英雄区）- 新版设计
**布局方式**：左右分栏，左侧文字+按钮，右侧视觉元素

```
┌────────────────────────────────────────────────────────────────┐
│  [顶部导航栏 - 见上方]                     [Get a Quote 按钮]  │
├────────────────────────────────────────────────────────────────┤
│                                                                │
│  [左侧 60%]                          [右侧 40%]               │
│  ┌───────────────────────┐          ┌──────────────────┐     │
│  │  Global Direct        │          │  ┌──────────┐    │     │
│  │  Ecommerce Solution   │          │  │👤👤👤      │    │     │
│  │  by Postal Service    │          │  │Leave Review│    │     │
│  │                       │          │  ├──────────┤    │     │
│  │  [副标题文字]          │          │  │   4.8 ⭐   │    │     │
│  │  Seamless cross-      │          │  │ Trusted by │    │     │
│  │  border logistics...  │          │  │ businesses │    │     │
│  │                       │          │  └──────────┘    │     │
│  │  [Get Started 橙色]   │          │                  │     │
│  │  [Track Package 透明] │          │  [货轮图片背景]   │     │
│  │                       │          │                  │     │
│  │  ┌─────────────────┐ │          │  [物流追踪可视化] │     │
│  │  │📦 UNLOADING     │ │          │  CN SHG ═══► US │     │
│  │  │Book Container   │ │          │  May 3  →  May 9│     │
│  │  │Unloading Today  │ │          │                  │     │
│  │  │[Book Now]       │ │          │                  │     │
│  │  └─────────────────┘ │          │                  │     │
│  └───────────────────────┘          └──────────────────┘     │
│                                                                │
│  [背景：蓝色渐变 + 集装箱货轮照片]                              │
└────────────────────────────────────────────────────────────────┘
```

**左侧内容区（60%宽度）**：
1. **主标题** (H1)：
   ```
   Global Direct Ecommerce Solution
   by Postal Service
   ```
   - 字体：Inter Bold, 48-60px
   - 颜色：白色 (#FFFFFF)
   - 行高：1.2

2. **副标题/描述**：
   ```
   Seamless cross-border logistics powered by
   Canada Post partnership - from China collection
   to Canada delivery
   ```
   - 字体：Inter Regular, 18-20px
   - 颜色：浅灰/白色 80%透明度
   - 最大宽度：600px

3. **双CTA按钮组**：
   - **主按钮**："Get Started"
     - 背景：橙色 (#FF9500)
     - 文字：白色
     - 圆角：8px
     - 尺寸：160x48px
   - **次按钮**："Track Package"
     - 背景：透明，白色边框
     - 文字：白色
     - 圆角：8px
     - 尺寸：160x48px

4. **左下角预订卡片**（3D浮动效果）：
   ```
   📦 UNLOADING
   Book Container Unloading Today
   [Book Now →]
   ```
   - 背景：深蓝色卡片，带阴影
   - 配合3D货柜图标
   - Hover时轻微上浮

**右侧视觉区（40%宽度）**：
1. **顶部评价卡片**（浮动）：
   ```
   ┌──────────────────┐
   │ 👤👤👤 Leave Review│
   ├──────────────────┤
   │      4.8 ⭐      │
   │  Trusted by      │
   │  businesses of   │
   │  all sizes       │
   └──────────────────┘
   ```
   - 白色卡片，圆角16px
   - 阴影效果
   - 用户头像重叠排列

2. **背景图片**：
   - 集装箱货轮照片
   - 从右下角进入画面
   - 应用蓝色叠加层（60%透明度）

3. **底部物流追踪可视化**：
   ```
   CN SHG ════════════► US OAK
     ●                     ○
   May 3, 23:27      09:00 May 9
   ```
   - 动画连线效果
   - 橙色进度线
   - 时间戳显示

**背景设计**：
- 深蓝到浅蓝的渐变（从左上到右下）
- 叠加集装箱货轮照片（右侧）
- 整体色调统一为蓝色系

**关键设计元素**：
- ✅ 左文右图的经典布局
- ✅ 橙色CTA按钮吸引注意力
- ✅ 评价卡片建立信任
- ✅ 物流追踪可视化展示专业性
- ✅ 3D货柜预订卡片增加互动感

---

### Section 2: Canada Post Partnership（合作背书）
**目的**：立即建立信任，突出战略合作关系

```
┌─────────────────────────────────────────────────────────┐
│        Proud Strategic Partner of Canada Post          │
│                                                         │
│         [Canada Post Logo - 大尺寸展示]                │
│                                                         │
│   "5 Million Parcels Annually | Trusted Since 202X"   │
│                                                         │
│   [小字说明：我们是Canada Post认可的跨境物流服务商]    │
└─────────────────────────────────────────────────────────┘
```

**设计要点**：
- 简洁的区块设计
- Canada Post Logo突出显示
- 用数据强化合作深度

---

### Section 3: Why Choose EIE（四大核心优势）
**布局**：2x2卡片网格，带图标和动画

```
┌──────────────────┬──────────────────┐
│  🌐 Complete     │  ✈️ Flexible     │
│  China Network   │  Air Resources   │
│                  │                  │
│ • 15+ Cities     │ • Multi-carrier  │
│ • Direct Pickup  │ • No Warehouse   │
│ • Multi-warehouse│   Waiting        │
├──────────────────┼──────────────────┤
│  📋 Professional │  🚚 Diversified  │
│  Customs Clear   │  Last Mile       │
│                  │                  │
│ • CBSA Certified │ • Canada Post    │
│ • 99%+ Success   │ • Eagleship      │
│ • 2-9 Days       │ • Multi-carrier  │
└──────────────────┴──────────────────┘
```

**每个卡片包含**：
- 图标动画
- 标题
- 3个关键点
- Hover效果展开更多信息

---

### Section 3.5: Global Direct Ecommerce Solution（全球直邮电商解决方案）
**核心定位**：By Postal Service - 基于邮政网络的跨境电商解决方案

**视觉布局**：分段式展示，配合实景图片

```
┌─────────────────────────────────────────────────────────────────┐
│    Global Direct Ecommerce Solution by Postal Service          │
│           从商家到消费者的全链路邮政直邮服务                    │
│                                                                 │
│  ┌──────────────────────────────────────────────────────────┐  │
│  │  【前段物流】China Operations & Air Transport            │  │
│  │                                                          │  │
│  │  [飞机图片]        [航班时刻表]       [分拣中心图片]    │  │
│  │  ↓                 ↓                  ↓                  │  │
│  │  • 国际航空运输    • 定期航班保障     • 智能分拣系统    │  │
│  │  • 多航司合作      • 灵活舱位调配     • 邮编精准分类    │  │
│  │  • 快速出境        • 优先保障         • 高效处理能力    │  │
│  └──────────────────────────────────────────────────────────┘  │
│                                                                 │
│  ┌──────────────────────────────────────────────────────────┐  │
│  │  【末端服务】Customs & Last Mile Delivery                │  │
│  │                                                          │  │
│  │  [清关文件]      [末端仓库]       [派送公司车辆]        │  │
│  │  ↓               ↓                ↓                      │  │
│  │  • CBSA清关认证  • 本地化仓储     • 多元派送网络        │  │
│  │  • 专业报关服务  • 快速处理中心   • 灵活派送方案        │  │
│  │  • 99%通过率     • 包裹再分拣     • 2-9天妥投           │  │
│  └──────────────────────────────────────────────────────────┘  │
│                                                                 │
│            [立即咨询]  [下载解决方案手册]                      │
└─────────────────────────────────────────────────────────────────┘
```

**关键卖点**：
1. **邮政级别服务**：依托邮政网络的可靠性和规模化能力
2. **端到端可控**：从中国揽收到加拿大派送的全链路掌控
3. **成本优势明显**：无传统快递的高额附加费用
4. **系统化运营**：标准化流程 + 智能化管理

**图片配置说明**：

**前段物流场景（3张核心图片）**：
```
1. 飞机航空运输场景
   - 展示内容：货机起飞/装载场景
   - 用途：体现国际航空运输能力
   - 配文："Multi-carrier Air Resources | 多航司灵活调配"
   - 尺寸：800x600px，高质量实景照片

2. 航班时刻表/运营看板
   - 展示内容：航班调度屏幕或运营数据看板
   - 用途：体现专业运营管理能力
   - 配文："Daily Flight Guarantee | 定期航班保障"
   - 尺寸：800x600px，可用数据可视化图表

3. 仓库分拣中心
   - 展示内容：自动化分拣线/包裹处理场景
   - 用途：体现高效处理和邮编分拣能力
   - 配文："Smart Sorting System | 智能邮编分类"
   - 尺寸：800x600px，展现规模化作业能力
```

**末端服务场景（3张核心图片）**：
```
1. 海关清关文件/清关流程
   - 展示内容：CBSA 认证文件、清关报关单据
   - 用途：体现专业清关资质和能力
   - 配文："CBSA Certified | 99%+ Clear Rate"
   - 尺寸：800x600px，可用证书+流程图组合

2. 末端仓库/配送中心
   - 展示内容：加拿大本地仓库内景/包裹整理
   - 用途：展示本地化服务能力
   - 配文："Local Warehouse Network | 本地化运营"
   - 尺寸：800x600px，整洁专业的仓储环境

3. 派送公司车辆/配送团队
   - 展示内容：Canada Post/Purolator/Eagleship 配送车
   - 用途：展示多元化最后一公里派送
   - 配文："Multi-carrier Delivery | 2-9 Days"
   - 尺寸：800x600px，品牌化配送车辆
```

**动画交互**：
- 鼠标悬停图片时：显示详细说明文字
- 时间轴连线动画：从左到右流动效果
- 数据节点：跳动展示关键数字（航班数量、处理量等）

---

### Section 4: Service Flow（服务流程）
**视觉**：横向时间轴，每步带图标和数据

```
中国揽收 → 质检查验 → 航空运输 → 海关清关 → 末端派送 → 售后服务
  │          │          │          │          │          │
15+城市    多仓协同    多航司     CBSA认证   多元网络   24h客服
直营团队   PostCode   灵活调配    99%通过   2-9天妥投  AI助手
```

**交互**：点击每个步骤展开详细说明

---

### Section 5: Competitive Advantages（对比优势）
**布局**：对比表格或优势列表

```
Why EIE vs. Traditional Carriers (DHL/FedEx/UPS)?

✓ Transparent Pricing        No hidden peak season fees
✓ Flexible Solutions         Customized for your needs  
✓ Fast Processing            No warehouse queue waiting
✓ Strong Sorting Capacity    Ideal for postal parcels
✓ System Integration         EDI/API support ready
✓ Real-time Tracking         Self-developed + 3rd party
```

---

### Section 6: By The Numbers（数据看板）
**视觉**：仪表盘风格，数字大而醒目

```
┌────────────┬────────────┬────────────┬────────────┐
│ 40,000+    │   15+      │   99%+     │   94%+     │
│ Daily      │  Cities    │  Customs   │ Customer   │
│ Parcels    │  Coverage  │  Clear     │ Satisfac.  │
└────────────┴────────────┴────────────┴────────────┘

┌─────────────────────────────────────────────────────┐
│  Delivery Time Performance                          │
│  [条形图：2-9天时效分布]                            │
└─────────────────────────────────────────────────────┘
```

---

### Section 7: Technology Capabilities（技术能力）
**展示系统对接和tracking能力**

```
┌─────────────────────────────────────────┐
│  System Integration Ready               │
│                                         │
│  • EDI/API Interface Support           │
│  • Self-developed Tracking Platform    │
│  • Real-time Data Push                 │
│  • Multi-format Data Exchange          │
│  • Third-party Query Integration       │
│                                         │
│  [查询演示：输入单号→实时轨迹展示]     │
└─────────────────────────────────────────┘
```

---

### Section 8: Our Network（网络展示）
**视觉**：交互式地图

```
┌─────────────────────────────────────────┐
│  [中国地图]                             │
│  15+城市揽收点标注（可点击查看详情）    │
│                                         │
│  [加拿大地图]                           │
│  清关口岸 + 派送网络（含Eagleship）     │
└─────────────────────────────────────────┘
```

---

### Section 9: Partners（合作伙伴）
**Logo墙**：分三类展示

```
Postal Partner:
[Canada Post Logo - 突出显示]

Air Carriers:
[航司Logos - 如果有授权的话]

Last Mile Partners:
[Purolator] [DHL] [UPS] [FedEx] [Eagleship自有品牌]
```

---

### Section 10: Call to Action（行动号召）
```
┌─────────────────────────────────────────────────────┐
│     Ready to Expand Postal Business in China?      │
│                                                     │
│         Let's discuss how we can help              │
│                                                     │
│      [Schedule a Meeting] [Download Brochure]      │
└─────────────────────────────────────────────────────┘
```

---

## 📄 主导航页面设计（新版结构）

### 导航1: Domestic Logistics（国内物流力量）

**页面定位**：展示EIE在中国的前端物流能力和资源优势

**内容板块**：

#### 1.1 Air Transport Rights（航权资源）
```
Multi-Carrier Airline Partnerships

✈️ Comprehensive Air Network
• Partnership with 5+ major airlines
• Daily flight capacity guarantee
• Direct routes: China → Canada
• Priority boarding during peak season

📊 Capacity Management
• Flexible space allocation
• Real-time capacity monitoring
• No warehouse queue waiting
• Guaranteed departure times

🌍 Coverage Routes
[地图展示：主要航线 - 北京/上海/深圳 → 温哥华/多伦多]

Key Advantages:
✓ Competitive pricing vs. traditional carriers
✓ Reliable capacity even in peak season
✓ Fast transit time (3-5 days)
✓ Flexible booking options
```

#### 1.2 Nationwide Collection（揽收网络）
```
15+ Cities Direct Pickup Network

🏙️ Major Coverage Cities
• Tier 1: Beijing, Shanghai, Guangzhou, Shenzhen
• Tier 2: Hangzhou, Chengdu, Chongqing, Wuhan, Xi'an
• And 6+ more cities

👥 Dedicated Collection Teams
• Local teams in each city
• Same-day/next-day pickup
• Professional handling training
• Real-time collection tracking

📦 Collection Services
• Door-to-door pickup
• Scheduled collection
• Emergency collection available
• Bulk collection support

[Interactive Map: 点击城市查看详细信息]
```

#### 1.3 Smart Sorting（分拣能力）
```
Intelligent Postal Code Sorting System

🤖 Automation Technology
• High-speed sorting lines
• Postal code recognition (99.9% accuracy)
• Barcode scanning integration
• Weight & dimension measurement

📊 Processing Capacity
• 40,000+ parcels per day
• 24/7 operation during peak season
• Multi-warehouse coordination
• Real-time inventory management

✅ Quality Control
• Multi-point inspection
• Export documentation verification
• Packaging compliance check
• Dangerous goods screening

[Video/Photos: 分拣中心实景]
```

#### 1.4 Quality Inspection（查验流程）
```
Comprehensive Quality Assurance

🔍 Inspection Standards
• Content verification
• Packaging quality check
• Weight & dimension validation
• Prohibited items screening

📋 Documentation Review
• Export declaration documents
• Commercial invoice verification
• Packing list accuracy
• Customs compliance check

✓ Quality Metrics
• 99.8% inspection accuracy
• <2 hours average processing time
• Zero tolerance for prohibited items
• Full traceability system

Process Flow:
[图表：揽收 → 初检 → 分拣 → 复核 → 出库 → 出境]
```

---

### 导航2: Customs Clearance（清关服务）

**页面定位**：突出EIE的专业清关能力和CBSA认证资质

**内容板块**：

#### 2.1 Export Declaration（出口报关）
```
Professional Export Services from China

📄 Documentation Services
• Export declaration preparation
• HS code classification
• Commercial invoice generation
• Certificate of origin (if required)

✓ Compliance Assurance
• China Customs regulations
• Export license verification
• Restricted items screening
• Anti-smuggling compliance

⚡ Fast Processing
• 24-hour documentation review
• Same-day submission to customs
• Real-time status updates
• Issue resolution support

Export Process:
[Flow Chart: 文件准备 → 海关申报 → 查验放行 → 出境]
```

#### 2.2 Import Clearance（进口清关）
```
CBSA-Certified Customs Broker in Canada

🏛️ A2Z CUSTOMS INC
• Licensed CBSA customs broker
• 5+ years of clearance experience
• Trilingual team (EN/CN/HI)
• 99%+ clearance success rate

📋 Import Services
• Customs declaration filing
• Duty & tax calculation
• CBSA examination support
• Release notification

⏱️ Fast Clearance Timeline
• 1-3 days: Standard clearance
• Same day: Express clearance option
• 2-9 days: Post-clearance delivery
• Real-time tracking updates

[Infographic: 到达加拿大 → 清关申报 → CBSA审核 → 放行 → 派送]
```

#### 2.3 CBSA Certification（CBSA认证）
```
Our Professional Credentials

🏆 Official Certifications
• CBSA Licensed Customs Broker
• Bonded Warehouse License
• ACI Participant
• CSA Trusted Trader (if applicable)

📜 Certificate Display
[High-resolution images of certificates]

👨‍💼 Expert Team
• 10+ certified customs brokers
• Specialized in ecommerce imports
• Multi-language support
• 24/7 availability

Why CBSA Certification Matters:
✓ Direct submission to CBSA systems
✓ Priority processing eligibility
✓ Reduced examination rates
✓ Faster clearance times
✓ Lower compliance risks
```

#### 2.4 Customs Processes（清关流程）
```
End-to-End Clearance Process

Step-by-Step Guide:

1️⃣ Pre-Clearance (Before Arrival)
   • Document preparation
   • Data submission to CBSA
   • Duty & tax calculation
   • Risk assessment

2️⃣ Arrival Processing
   • Flight arrival notification
   • Cargo unloading
   • Transfer to bonded warehouse
   • CBSA examination (if required)

3️⃣ Clearance & Release
   • CBSA review & approval
   • Duty & tax payment
   • Release authorization
   • Delivery to carrier

4️⃣ Post-Clearance
   • Final delivery to recipient
   • POD confirmation
   • Invoice reconciliation
   • Issue resolution (if any)

[Interactive Timeline: 可视化时间轴展示每个步骤]

Common Clearance Issues & Solutions:
• Incomplete documentation → Document support
• HS code disputes → Classification expertise
• Valuation questions → Appraisal service
• Examination hold → CBSA liaison
```

---

### 导航3: After-Sales Service（售后服务）

**页面定位**：展示全方位的客户服务和增值服务能力

**内容板块**：

#### 3.1 24/7 Customer Support（24小时客服）
```
Round-the-Clock Professional Support

🌐 Multi-Channel Support
• Phone: +1-XXX-XXX-XXXX (Canada)
         +86-XXX-XXXX-XXXX (China)
• Email: support@eie-logistics.com
• Live Chat: Website & WeChat
• WhatsApp: +1-XXX-XXX-XXXX

👥 Support Team
• Dedicated account managers
• Trilingual support (EN/CN/FR)
• Average response time: <2 hours
• 24/7/365 availability

🤖 AI-Powered Assistance
• Instant tracking queries
• Common questions answered
• Multi-language support
• Seamless human handoff

Support Scope:
✓ Shipment tracking & status
✓ Documentation assistance
✓ Customs clearance inquiries
✓ Delivery coordination
✓ Issue resolution & claims
✓ Account management

[Live Chat Demo Widget]
```

#### 3.2 China Warehouse Services（国内仓库服务）
```
Comprehensive Warehousing in China

📦 Warehouse Network
• 15+ cities with warehouse facilities
• Total storage: 50,000+ sqm
• Temperature-controlled zones (if applicable)
• 24/7 security & monitoring

🔧 Value-Added Services
• Storage & inventory management
• Product inspection & QC
• Labeling & repackaging
• Consolidation services
• Order fulfillment
• Photo inspection reports

📊 Inventory Management
• Real-time inventory tracking
• Automated alerts & notifications
• FIFO/LIFO options
• Batch management
• Expiry date tracking

Warehouse Features:
✓ Modern facilities with advanced equipment
✓ Strict quality control procedures
✓ Flexible storage solutions
✓ Easy online inventory access
✓ Scalable capacity

[Photos: Warehouse facilities]
```

#### 3.3 Canada Warehouse Services（国外仓库服务）
```
Local Warehousing & Distribution in Canada

🏢 Canada Facilities
• Vancouver distribution center
• Toronto service point
• Montreal warehouse (planned)
• Nationwide coverage

📦 Services Offered
• Import receiving & inspection
• Short-term & long-term storage
• Order picking & packing
• Kitting & assembly
• Return processing
• Cross-docking services

🚚 Distribution Services
• Same-day/next-day delivery
• Scheduled deliveries
• White-glove service
• Reverse logistics
• Multi-carrier integration

Benefits:
✓ Reduced shipping costs
✓ Faster delivery times
✓ Better inventory control
✓ Returns management
✓ Local customer service

[Interactive Map: 加拿大仓库位置和覆盖范围]
```

#### 3.4 Value-Added Services（附加服务）
```
Beyond Standard Logistics

🎁 Additional Services
• Custom packaging & branding
• Gift wrapping & inserts
• COD (Cash on Delivery)
• Insurance coverage
• Special handling (fragile, high-value)
• Returns management

📸 Enhanced Services
• Product photography
• Pre-shipment inspection
• Quality control reports
• Video inspection
• Damage assessment

📄 Documentation Services
• Certificate of origin
• Commercial invoice preparation
• Packing list generation
• Export/import documentation
• Compliance consulting

💡 Special Solutions
• Subscription box fulfillment
• Promotional campaigns support
• Seasonal surge handling
• Custom integration projects
• Dedicated account management

[Service Request Form]
```

---

### 导航4: About & Contact（关于我们与联系）

**页面定位**：公司介绍、资质展示和联系方式

**内容板块**：

#### 4.1 Company Profile（公司简介）
```
EIE LOGISTICS - Your Trusted Postal Partner

📖 Our Story
Founded in 202X, EIE Logistics has grown to become a leading
cross-border logistics provider specializing in China-Canada
postal services. As a strategic partner of Canada Post, we
handle over 5 million parcels annually with industry-leading
efficiency and reliability.

🎯 Mission
To provide seamless, cost-effective cross-border logistics
solutions that empower businesses to succeed in international
ecommerce.

🌟 Vision
To become the most trusted postal logistics partner connecting
Asia-Pacific markets with North America.

💪 Core Values
• Customer First: Your success is our priority
• Professional Excellence: Expertise in every step
• Reliable Service: Consistent quality you can trust
• Innovation: Continuous improvement in technology
• Integrity: Transparent and honest operations

📊 Key Achievements
• 5,000,000+ Annual parcels handled
• 40,000+ Daily processing capacity
• 99%+ Customs clearance success rate
• 94%+ Customer satisfaction score
• 15+ Cities direct coverage in China
• 5+ Years partnership with Canada Post

[Company Timeline Infographic]
```

#### 4.2 Our Facilities（设施展示）
```
World-Class Logistics Infrastructure

🏭 China Operations
📍 Beijing Sorting Center
   • 10,000 sqm facility
   • 15,000 parcels/day capacity
   • Automated sorting lines

📍 Shanghai Warehouse
   • 15,000 sqm storage
   • Temperature-controlled zones
   • Advanced security systems

📍 Shenzhen Hub
   • 20,000 sqm facility
   • Direct airport access
   • 24/7 operations

[+ 12 more locations across China]

🇨🇦 Canada Operations
📍 Vancouver Clearance Center
   • CBSA-bonded warehouse
   • 5,000 sqm facility
   • A2Z Customs office

📍 Toronto Distribution
   • 3,000 sqm warehouse
   • Multi-carrier integration
   • Returns processing

[Photo Gallery: High-quality facility images]
[Virtual Tour: 360° facility walkthrough]
```

#### 4.3 Certifications（资质认证）
```
Professional Credentials & Certifications

🏆 Official Certifications
✓ CBSA Licensed Customs Broker (Canada)
✓ Canada Post Verified Partner
✓ ISO 9001:2015 Quality Management (if applicable)
✓ IATA Cargo Agent (if applicable)
✓ WCA Membership (if applicable)

📜 Business Licenses
• China Freight Forwarding License
• International Trade License
• Dangerous Goods Handling Permit (if applicable)
• Bonded Warehouse License (Canada)

🔒 Compliance & Security
• AEO Certified (if applicable)
• C-TPAT Certified (if applicable)
• Data Privacy Compliance (GDPR, PIPEDA)
• Insurance Coverage: $X Million

[High-Resolution Certificate Images]
[Download: Certification Package PDF]
```

#### 4.4 Contact Information（联系方式）
```
Get in Touch with Our Team

🇨🇳 China Headquarters
Address: [完整地址]
City: Shenzhen, Guangdong, China
Phone: +86-XXX-XXXX-XXXX
Email: china@eie-logistics.com
WeChat: EIE_Logistics
Hours: Mon-Fri 9:00-18:00 CST

🇨🇦 Canada Office - A2Z CUSTOMS INC
Address: [完整地址]
City: Vancouver, BC, Canada
Phone: +1-XXX-XXX-XXXX
Email: canada@eie-logistics.com
WhatsApp: +1-XXX-XXX-XXXX
Hours: Mon-Fri 9:00-17:00 PST

📧 General Inquiries
Sales: sales@eie-logistics.com
Support: support@eie-logistics.com
Careers: hr@eie-logistics.com

🌐 Follow Us
• LinkedIn: linkedin.com/company/eie-logistics
• WeChat Official Account: [QR Code]
• Facebook: facebook.com/eielogistics (if applicable)

[Office Location Maps - Interactive]
```

#### 4.5 Business Inquiry（商务咨询）
```
Start Your Partnership with EIE

📝 Contact Form

Name: ___________________
Company: ________________
Email: __________________
Phone: __________________

Service Interest:
[ ] Domestic Logistics
[ ] Customs Clearance
[ ] Warehousing
[ ] Full Service Solution
[ ] Other: ______________

Estimated Monthly Volume:
[ ] < 1,000 parcels
[ ] 1,000 - 5,000 parcels
[ ] 5,000 - 20,000 parcels
[ ] > 20,000 parcels

Message:
_________________________
_________________________

[ ] I agree to the privacy policy

[Submit Inquiry]

Response Time: Within 24 hours
Account Manager Assignment: Within 48 hours
Custom Quote: Within 3-5 business days

[Quick Links]
• Download Service Brochure (PDF)
• Request Rate Card (requires email)
• Schedule Video Call
• Visit Our Facilities
```

---

## 📄 老版其他页面设计（保留参考）

### About Us（关于我们）- 老版内容

**Company Overview**
```
Founded: 202X
Mission: Connecting China and Canada with reliable postal logistics
Vision: Become the leading postal logistics partner in Asia-Pacific

Key Milestones:
• 202X - Established partnership with Canada Post
• 2024 - Founded A2Z Customs Inc in Canada
• 202X - Launched Eagleship delivery service
• 202X - Achieved 5M annual parcel volume
```

**Our Facilities**
- 中国仓库照片（15+城市网络）
- 加拿大清关中心照片
- 分拣中心照片
- 配送车队照片

**Certifications**
- CBSA认证证书
- ISO质量认证（如果有）
- 其他资质展示

---

### Services（服务详情）

#### 1. China Operations
```
Nationwide Collection Network
• Direct pickup in 15+ major cities
• Dedicated collection team
• Same-day/next-day pickup available

Quality Control
• Multi-warehouse inspection
• Post code sorting
• Export documentation

Coverage Cities:
[地图标注] 北京/上海/深圳/广州/杭州...
```

#### 2. International Transport
```
Flexible Air Resources
• Partnership with multiple airlines
• Daily flights available
• No warehouse queue waiting
• Priority boarding during peak season

Advantages:
✓ Competitive pricing
✓ Fast transit time
✓ Reliable capacity guarantee
```

#### 3. Customs Clearance
```
A2Z CUSTOMS INC (CANADA)
• CBSA Certified
• 99%+ clearance success rate
• 2-9 days post-clearance delivery
• Expert team in China, India & Canada

Services Include:
• Import documentation
• Customs declaration
• Tax calculation & payment
• Issue resolution
• Compliance consulting
```

#### 4. Last Mile Delivery
```
Multi-Carrier Network
• Canada Post
• Purolator
• DHL / UPS / FedEx
• Eagleship (Self-operated)

Eagleship - Our Advantage
• Direct control over delivery quality
• Flexible delivery options
• Real-time tracking
• Lower cost for clients
```

---

### Our Network（网络页面）

**交互式地图**：
- 中国地图：标注15+城市，点击显示仓库地址和联系方式
- 加拿大地图：标注清关口岸和派送范围
- 连线动画：显示典型路线（如深圳→温哥华）

**数据展示**：
```
China Coverage:
• 15+ Cities Direct Pickup
• 50+ Partner Warehouses
• 24-hour Response Time

Canada Network:
• Vancouver Customs Hub
• Toronto Distribution Center
• Montreal Service Point
• Nationwide Delivery Coverage
```

---

### Technology（技术页面）

**System Integration**
```
We Support:
• EDI (Electronic Data Interchange)
• API Integration
• FTP/SFTP Data Transfer
• Webhook Real-time Push

Data Formats:
• JSON / XML / CSV
• Custom format support available
```

**Tracking System**
```
Features:
• Real-time status updates
• Multi-platform access (Web/App)
• Batch query support
• Third-party query integration
• Automated notifications (Email/SMS)

[Live Demo: 单号查询演示]
```

**Data Services**
```
Reports Available:
• Daily/Weekly/Monthly summary
• Performance analytics
• Custom reports
• API access for data export
```

---

### Why EIE（优势页面）

**Cost Advantage**
```
Transparent Pricing Model
✓ No hidden fees
✓ No peak season surcharges
✓ No fuel surcharges fluctuation
✓ Volume discounts available

[对比图表：EIE vs. Traditional Carriers]
```

**Operational Advantage**
```
Faster Processing
• No warehouse queue waiting
• Priority handling for partners
• Flexible capacity allocation
• 24/7 operations during peak season

Quality Control
• Post code sorting accuracy: 99%+
• Customs clearance rate: 99%+
• On-time delivery: 94%+
```

**Customer Service**
```
24/7 Support
• Dedicated account manager
• 24-hour hotline
• AI customer service assistant
• Multi-language support (EN/CN/FR)
```

---

### Contact Us（联系页面）

**Contact Form**
```
Name: ___________
Company: ___________
Email: ___________
Phone: ___________
Service Interest: [下拉选择]
Message: ___________
[Submit Inquiry]
```

**Office Information**
```
China Headquarters:
[地址]
Phone: +86 XXX
Email: china@eie-logistics.com

Canada Office:
A2Z CUSTOMS INC
[地址]
Phone: +1 XXX
Email: canada@eie-logistics.com

Business Hours:
China: Monday-Friday 9:00-18:00 CST
Canada: Monday-Friday 9:00-17:00 PST
```

---

## 🎨 设计规范（新版 - 参考GFS风格）

### 品牌颜色方案

**设计风格定位**：专业物流行业风格
**参考对象**：Global Freight Solutions (GFS) 网站配色
**核心配色**：蓝色系（主色调）+ 橙色（强调色）

```css
/* === 主色调 - 蓝色系（物流专业感）=== */
--primary-navy: #0A2647;      /* 深海军蓝 - 顶部导航、标题 */
--primary-blue: #144272;      /* 标准蓝 - 背景、大面积使用 */
--primary-light: #205295;     /* 亮蓝 - 次要元素 */
--primary-sky: #2C74B3;       /* 天蓝 - 装饰、图标 */

/* Hero区域专用渐变 */
--gradient-hero: linear-gradient(135deg, #0A2647 0%, #144272 50%, #205295 100%);
--gradient-hero-overlay: linear-gradient(90deg,
  rgba(10, 38, 71, 0.95) 0%,
  rgba(20, 66, 114, 0.85) 50%,
  rgba(32, 82, 149, 0.70) 100%
);

/* === 强调色 - 橙色系（行动号召）=== */
--accent-orange: #FF9500;     /* 主橙色 - CTA按钮、重要元素 */
--accent-orange-light: #FFB340; /* 浅橙 - Hover状态 */
--accent-orange-dark: #E68600;  /* 深橙 - Active状态 */

/* === 辅助色系 === */
/* 成功/状态色 */
--success: #10B981;           /* 绿色 - 成功状态、在途 */
--warning: #F59E0B;           /* 黄色 - 警告、待处理 */
--error: #EF4444;             /* 红色 - 错误、异常 */
--info: #3B82F6;              /* 信息蓝 - 提示信息 */

/* 中性色 */
--white: #FFFFFF;             /* 纯白 */
--gray-50: #F9FAFB;           /* 极浅灰 - 背景 */
--gray-100: #F3F4F6;          /* 浅灰 - 卡片背景 */
--gray-200: #E5E7EB;          /* 边框灰 */
--gray-400: #9CA3AF;          /* 次要文字 */
--gray-600: #4B5563;          /* 常规文字 */
--gray-800: #1F2937;          /* 深色文字 */
--gray-900: #111827;          /* 标题文字 */

/* === 渐变系统 === */
--gradient-card: linear-gradient(180deg, #FFFFFF 0%, #F9FAFB 100%);
--gradient-header: linear-gradient(90deg,
  rgba(10, 38, 71, 0.98) 0%,
  rgba(20, 66, 114, 0.95) 100%
);
--gradient-button: linear-gradient(135deg, #FF9500 0%, #FFB340 100%);

/* === 阴影系统 === */
--shadow-sm: 0 1px 2px 0 rgba(0, 0, 0, 0.05);
--shadow-md: 0 4px 6px -1px rgba(0, 0, 0, 0.1);
--shadow-lg: 0 10px 15px -3px rgba(0, 0, 0, 0.1);
--shadow-xl: 0 20px 25px -5px rgba(0, 0, 0, 0.1);
--shadow-orange: 0 8px 16px -4px rgba(255, 149, 0, 0.3); /* 橙色按钮阴影 */

/* === 特殊效果 === */
--overlay-blue: rgba(10, 38, 71, 0.6);  /* 蓝色叠加层 */
--glass-effect: rgba(255, 255, 255, 0.1); /* 玻璃态效果 */
```

**配色应用规则**：

**Hero 区域**：
- 背景：`--gradient-hero` + 货轮照片
- 叠加层：`--gradient-hero-overlay`（图片上方）
- 主标题：`--white`
- 副标题：`--white` 80% 透明度
- 主CTA按钮：`--accent-orange` 背景 + `--white` 文字
- 次CTA按钮：透明背景 + `--white` 边框和文字

**导航栏**：
- 背景：`--gradient-header` 或半透明深蓝
- 文字：`--white`
- Hover：`--accent-orange`
- CTA按钮：`--accent-orange`

**卡片组件**：
- 背景：`--white` 或 `--gradient-card`
- 边框：`--gray-200`
- 阴影：`--shadow-lg`
- 橙色强调元素：`--accent-orange`

**按钮系统**：
- **主按钮**：橙色背景 + 白色文字 + 橙色阴影
- **次按钮**：透明背景 + 蓝色边框 + 蓝色文字
- **文字按钮**：无背景 + 橙色文字

**状态颜色**：
- 在途/进行中：`--info` 或 `--primary-sky`
- 已完成：`--success`
- 待处理：`--warning`
- 异常/错误：`--error`

### 字体系统

```css
/* 英文字体 */
--font-display: 'Inter', sans-serif;      /* 标题、数字 */
--font-body: 'Inter', sans-serif;         /* 正文 */

/* 中文字体 */
--font-cn-display: 'Noto Sans SC', sans-serif;
--font-cn-body: 'Noto Sans SC', sans-serif;

/* 字体大小 */
--text-xs: 0.75rem;     /* 12px */
--text-sm: 0.875rem;    /* 14px */
--text-base: 1rem;      /* 16px */
--text-lg: 1.125rem;    /* 18px */
--text-xl: 1.25rem;     /* 20px */
--text-2xl: 1.5rem;     /* 24px */
--text-3xl: 1.875rem;   /* 30px */
--text-4xl: 2.25rem;    /* 36px */
--text-5xl: 3rem;       /* 48px */
--text-6xl: 3.75rem;    /* 60px */

/* 字重 */
--font-normal: 400;
--font-medium: 500;
--font-semibold: 600;
--font-bold: 700;
```

### 间距系统

```css
--spacing-1: 0.25rem;   /* 4px */
--spacing-2: 0.5rem;    /* 8px */
--spacing-3: 0.75rem;   /* 12px */
--spacing-4: 1rem;      /* 16px */
--spacing-6: 1.5rem;    /* 24px */
--spacing-8: 2rem;      /* 32px */
--spacing-12: 3rem;     /* 48px */
--spacing-16: 4rem;     /* 64px */
--spacing-24: 6rem;     /* 96px */
```

### 圆角和阴影

```css
/* 圆角 */
--radius-sm: 0.25rem;   /* 4px - 按钮、小卡片 */
--radius-md: 0.5rem;    /* 8px - 卡片 */
--radius-lg: 1rem;      /* 16px - 大卡片 */
--radius-xl: 1.5rem;    /* 24px - Hero区块 */

/* 阴影 */
--shadow-sm: 0 1px 2px 0 rgb(0 0 0 / 0.05);
--shadow-md: 0 4px 6px -1px rgb(0 0 0 / 0.1);
--shadow-lg: 0 10px 15px -3px rgb(0 0 0 / 0.1);
--shadow-xl: 0 20px 25px -5px rgb(0 0 0 / 0.1);
```

### 设计原则

**1. 专业可信**
- 使用大量留白
- 简洁的布局
- 高质量图片和图标
- 数据可视化展示

**2. 视觉层次**
- 清晰的信息架构
- 标题层级明显（H1-H6）
- 关键信息突出显示
- 引导视线流向CTA

**3. 动画效果**
- 数字跳动（CountUp.js）
- Fade In/Slide In（Intersection Observer）
- Hover微交互
- 地图连线动画
- 控制动画时长（200-400ms）

**4. 响应式设计**
- Mobile First
- 断点：640px / 768px / 1024px / 1280px / 1536px
- 触摸友好（按钮最小44x44px）
- 移动端优化图片

---

## 💻 技术栈

### 前端框架
```
Framework: Next.js 14 (App Router)
语言: TypeScript
UI库: Shadcn/ui + Radix UI
样式: Tailwind CSS
图标: Lucide React / Heroicons
```

**为什么选择Next.js？**
- ✅ SEO友好（SSR/SSG）
- ✅ 性能优异（自动代码分割）
- ✅ 开发速度快（热重载、TypeScript支持）
- ✅ 部署简单（Vercel一键部署）
- ✅ 图片优化（Next/Image自动优化）

**为什么选择Shadcn/ui？**
- ✅ 组件丰富且高质量
- ✅ 完全可定制
- ✅ TypeScript原生支持
- ✅ 无运行时依赖（复制到项目）
- ✅ 美观的默认样式

### 核心依赖

```json
{
  "dependencies": {
    "next": "^14.0.0",
    "react": "^18.2.0",
    "react-dom": "^18.2.0",
    "typescript": "^5.0.0",
    
    // UI组件
    "@radix-ui/react-*": "latest",
    "class-variance-authority": "^0.7.0",
    "clsx": "^2.0.0",
    "tailwind-merge": "^2.0.0",
    
    // 动画
    "framer-motion": "^10.16.0",
    
    // 图表
    "recharts": "^2.10.0",
    
    // 地图
    "leaflet": "^1.9.4",
    "react-leaflet": "^4.2.1",
    
    // 表单
    "react-hook-form": "^7.48.0",
    "zod": "^3.22.0",
    
    // 国际化
    "next-intl": "^3.0.0",
    
    // 工具
    "date-fns": "^2.30.0",
    "react-countup": "^6.5.0"
  },
  "devDependencies": {
    "tailwindcss": "^3.3.0",
    "postcss": "^8.4.31",
    "autoprefixer": "^10.4.16",
    "eslint": "^8.54.0",
    "eslint-config-next": "^14.0.0"
  }
}
```

### 项目结构

```
eie-website/
├── app/
│   ├── [locale]/              # 国际化路由
│   │   ├── page.tsx           # 首页
│   │   ├── about/
│   │   ├── services/
│   │   ├── network/
│   │   ├── technology/
│   │   ├── why-eie/
│   │   └── contact/
│   ├── api/                   # API路由（表单提交）
│   ├── layout.tsx
│   └── globals.css
├── components/
│   ├── ui/                    # Shadcn UI组件
│   ├── sections/              # 首页各section组件
│   │   ├── Hero.tsx
│   │   ├── Partnership.tsx
│   │   ├── Advantages.tsx
│   │   ├── ServiceFlow.tsx
│   │   ├── DataDashboard.tsx
│   │   ├── Network.tsx
│   │   └── CTA.tsx
│   ├── layout/
│   │   ├── Header.tsx
│   │   ├── Footer.tsx
│   │   └── Navigation.tsx
│   └── shared/                # 共享组件
│       ├── CountUpNumber.tsx
│       ├── AnimatedSection.tsx
│       └── InteractiveMap.tsx
├── lib/
│   ├── utils.ts
│   └── constants.ts
├── public/
│   ├── images/
│   ├── icons/
│   └── videos/
├── messages/                  # 国际化文案
│   ├── en.json
│   └── zh.json
├── tailwind.config.ts
├── next.config.js
└── package.json
```

### 部署方案

**推荐：Vercel（免费计划）**
```bash
# 连接GitHub仓库后自动部署
# 每次git push自动触发部署
# 自动HTTPS
# 全球CDN
# 自动图片优化
```

**域名绑定**
```
主域名：www.eie-logistics.com
或使用：eie.vercel.app（临时域名）
```

**环境变量**
```env
NEXT_PUBLIC_SITE_URL=https://www.eie-logistics.com
NEXT_PUBLIC_GA_ID=G-XXXXXXXXXX  # Google Analytics
RESEND_API_KEY=re_xxxx          # 邮件服务（表单提交）
```

---

## 📝 完整文案内容

### 首页 - 英文版（新版文案）

#### Hero Section（新版）
```
Global Direct Ecommerce Solution
by Postal Service

Seamless cross-border logistics powered by Canada Post partnership -
from China collection to Canada delivery, we handle every step with
professional expertise and reliable service.

[Get Started]  [Track Package]

━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━
Left Bottom Card:
📦 UNLOADING
Book Container Unloading Today
[Book Now →]

Right Top Card (Review):
👤👤👤 Leave a Review
⭐ 4.8
Trusted by businesses of all sizes.
See why businesses trust our unloading services.

Right Bottom (Tracking Visual):
CN SHG ════════════► US OAK
   ●                     ○
May 3, 23:27      09:00 May 9
━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━
```

#### Partnership Banner
```
Proud Strategic Partner of Canada Post

5 Million Parcels Annually | Trusted Excellence Since 2020

As a verified partner of Canada Post, we deliver postal logistics
solutions that meet the highest international standards
```

#### Why Choose EIE
```
Why Global Postal Networks Choose EIE

Complete China Network
• Direct pickup coverage in 15+ major cities
• Dedicated collection teams for one-on-one service
• Multi-warehouse coordination for efficient processing

Flexible Air Resources
• Partnership with multiple leading airlines
• No warehouse queue waiting
• Guaranteed capacity even during peak seasons

Professional Customs Clearance
• CBSA-certified customs broker (A2Z CUSTOMS INC)
• 99%+ clearance success rate
• 2-9 days post-clearance delivery time

Diversified Last Mile
• Partnership with Canada Post, Purolator, DHL, UPS, FedEx
• Self-operated Eagleship delivery network
• Flexible delivery solutions for any requirement
```

#### Global Direct Ecommerce Solution
```
Global Direct Ecommerce Solution by Postal Service

Your Complete Cross-border Ecommerce Logistics Partner
From merchant to consumer, powered by postal network reliability

━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━

【 CHINA OPERATIONS & AIR TRANSPORT 】

✈️ International Air Transport
   • Multi-carrier airline partnerships
   • Daily flight capacity guarantee
   • Fast customs clearance and export

📊 Flight Schedule Management
   • Regular flight schedule assurance
   • Flexible capacity allocation
   • Priority guarantee during peak season

📦 Smart Sorting System
   • Automated sorting lines
   • Precise postal code classification
   • High-efficiency processing capability

━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━

【 CUSTOMS & LAST MILE DELIVERY 】

📋 Professional Customs Clearance
   • CBSA certified customs broker
   • Expert customs declaration service
   • 99%+ clearance success rate

🏢 Local Warehouse Network
   • Canada local warehouse facilities
   • Fast processing center
   • Package re-sorting and distribution

🚚 Multi-carrier Delivery
   • Partnership with Canada Post, Purolator, and more
   • Self-operated Eagleship delivery
   • Flexible delivery solutions
   • 2-9 days delivery guarantee

━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━

Why Choose Our Ecommerce Solution?

✓ Postal-grade Service Quality
  Leveraging postal network reliability and scalability

✓ End-to-End Control
  Full visibility from China collection to Canada delivery

✓ Significant Cost Advantage
  No traditional courier high surcharges

✓ Systematic Operations
  Standardized processes + intelligent management

[Contact Our Team]  [Download Solution Guide]
```

#### Service Flow
```
Our End-to-End Service Excellence

Collection → Inspection → Air Transport → Customs → Delivery → Support
   ↓            ↓              ↓            ↓          ↓          ↓
15+ Cities   Post Code     Multi-carrier   CBSA      2-9 Days   24/7
Direct Team   Sorting       Resources     Certified  Delivery   Service
```

#### Competitive Advantages
```
The EIE Advantage: Beyond Traditional Carriers

✓ Transparent Pricing
  No hidden peak season fees or unexpected surcharges

✓ Flexible Solutions
  Customized service plans tailored to your specific needs

✓ Fast Processing
  No warehouse queue waiting means faster transit times

✓ Strong Sorting Capacity
  Advanced post code sorting ideal for postal parcel volumes

✓ System Integration Ready
  Full EDI/API support for seamless system connectivity

✓ Real-time Tracking
  Self-developed platform integrated with third-party queries
```

#### By The Numbers
```
Performance That Speaks for Itself

40,000+          15+            99%+           94%+
Daily Parcels    Cities         Customs        Customer
Processed        Covered        Clear Rate     Satisfaction

2-9 Days
Average delivery time after customs clearance

5 Million
Annual parcels handled for Canada Post
```

#### Technology
```
Advanced Technology Infrastructure

System Integration
Complete EDI and API support for seamless connectivity with
postal systems worldwide

Real-time Tracking
Self-developed tracking platform with third-party integration
and automated status updates

Data Services
Comprehensive reporting and analytics with customizable
data export options
```

#### Call to Action
```
Ready to Expand Your Postal Business in China?

Let's discuss how EIE can help you achieve
operational excellence and cost efficiency

[Schedule a Meeting]  [Download Brochure]
```

---

### 首页 - 中文版

#### Hero Section
```
EIE 国际物流

连接中加的邮政物流专家

从揽收到派送，一站式跨境解决方案
专业、可靠、高效

[联系我们]  [了解服务]
```

#### Partnership Banner
```
Canada Post 战略合作伙伴

年均处理500万包裹 | 值得信赖的专业服务

作为Canada Post认证合作伙伴，我们提供符合国际最高标准的
邮政物流解决方案
```

#### Why Choose EIE
```
为什么全球邮政网络选择EIE

完整的中国网络
• 覆盖全国15+个一二线城市直营揽收
• 专属揽收团队，一对一贴心服务
• 多仓协同，灵活高效处理

灵活的航空资源
• 与多家主流航司深度合作
• 无排仓等待，保障时效
• 旺季也能确保舱位

专业的清关能力
• CBSA认证清关行（A2Z CUSTOMS INC）
• 99%以上清关通过率
• 清关后2-9天妥投

多元化末端派送
• 合作Canada Post、Purolator、DHL、UPS、FedEx
• 自营Eagleship配送团队
• 灵活的派送方案满足各类需求
```

#### 全球直邮电商解决方案
```
Global Direct Ecommerce Solution by Postal Service
基于邮政网络的全球跨境电商物流解决方案

从商家到消费者的全链路邮政直邮服务
依托邮政网络的可靠性，为您的跨境业务保驾护航

━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━

【 前段物流 - 中国运营 & 航空运输 】

✈️ 国际航空运输
   • 与多家主流航司深度合作
   • 每日航班运力保障
   • 快速通关出境

📊 航班调度管理
   • 定期航班时刻保障
   • 灵活舱位调配能力
   • 旺季优先保障机制

📦 智能分拣系统
   • 自动化分拣流水线
   • 精准邮编分类能力
   • 高效处理大批量包裹

━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━

【 末端服务 - 清关 & 派送 】

📋 专业清关服务
   • CBSA 认证清关行资质
   • 专业报关申报服务
   • 99%+ 清关通过率

🏢 本地仓储网络
   • 加拿大本地化仓库设施
   • 快速处理分拣中心
   • 包裹二次分拣配送

🚚 多元派送网络
   • 合作 Canada Post、Purolator 等
   • 自营 Eagleship 配送团队
   • 灵活派送方案选择
   • 2-9 天妥投保障

━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━

为什么选择我们的电商解决方案？

✓ 邮政级别服务品质
  依托邮政网络的可靠性和规模化运营能力

✓ 端到端全程掌控
  从中国揽收到加拿大派送的全链路可视化管理

✓ 显著成本优势
  无传统快递的高额附加费用和隐藏成本

✓ 系统化规范运营
  标准化流程配合智能化管理系统

[立即咨询]  [下载解决方案手册]
```

[其余中文内容类似结构...]

---

## 🎬 动画效果规范

### 页面加载动画
```javascript
// Hero区域
- Logo: Fade In + Scale (0.3s)
- 标题: Slide Up (0.5s, delay 0.2s)
- 数据: Count Up动画 (2s)
- 按钮: Fade In (0.3s, delay 0.8s)

// 滚动触发动画
- 卡片: Fade In + Slide Up (0.5s)
- 数字: Count Up（进入视口时触发）
- 地图: 连线动画（进入视口后开始）
```

### 交互动画
```javascript
// 按钮
- Hover: Scale(1.05) + Shadow增强 (0.2s)
- Click: Scale(0.95) (0.1s)

// 卡片
- Hover: translateY(-8px) + Shadow (0.3s)

// 导航
- 菜单展开: Slide Down (0.3s)
- 语言切换: Fade (0.2s)
```

---

## 📱 响应式设计要点

### 断点策略
```
Mobile:    < 640px
Tablet:    640px - 1024px
Desktop:   > 1024px
Large:     > 1280px
```

### 关键适配
```
Hero区域：
- Mobile: 单列布局，数据堆叠
- Desktop: 数据横排展示

优势卡片：
- Mobile: 1列
- Tablet: 2列
- Desktop: 2x2网格

导航：
- Mobile: 汉堡菜单
- Desktop: 横向导航栏

表单：
- Mobile: 全宽输入框
- Desktop: 两列布局
```

---

## 🚀 开发计划（4天冲刺）

### Day 1 - 今天（设计+准备）
**上午（4h）**
- ✅ PRD确认
- 🎨 首页视觉设计稿（Figma/Sketch）
- 📝 收集所有素材（Logo、照片）

**下午（4h）**
- 💻 搭建Next.js项目
- 📦 安装依赖，配置Tailwind
- 🎯 创建项目结构
- 🌍 配置国际化框架

**晚上（2h）**
- 📝 完成所有文案（中英文）
- 🎨 确定最终配色和字体

---

### Day 2 - 明天（核心开发）
**上午（4h）**
- 🏗️ 搭建Layout（Header/Footer）
- 🎨 开发首页Hero区域
- 💳 开发Canada Post合作区
- 📊 开发四大优势卡片

**下午（4h）**
- 📈 开发服务流程时间轴
- 🎯 开发数据看板（CountUp动画）
- 🗺️ 开发网络地图（Leaflet）
- 🤝 开发合作伙伴Logo墙

**晚上（2h）**
- ✨ 添加滚动动画（Framer Motion）
- 🔧 首页细节优化

---

### Day 3 - 后天（完善+其他页面）
**上午（4h）**
- 📄 开发About Us页面
- 🛠️ 开发Services页面（4个子页面）
- 🗺️ 开发Network页面（交互地图）

**下午（4h）**
- 💻 开发Technology页面
- 🏆 开发Why EIE页面
- 📮 开发Contact Us页面（表单）
- 🔗 内部链接完善

**晚上（2h）**
- 🌍 完成中英文切换
- 📱 移动端适配检查

---

### Day 4 - 会议前一天（测试+部署）
**上午（3h）**
- 🐛 功能测试（所有页面、所有链接）
- 📱 跨设备测试（iPhone/iPad/Desktop）
- 🌐 跨浏览器测试（Chrome/Safari/Firefox）
- ♿ 可访问性检查

**中午（1h）**
- 🚀 部署到Vercel
- 🔗 绑定域名（如有）
- 🔍 SEO优化（meta标签、sitemap）

**下午（2h）**
- 📊 Google Analytics配置
- 💾 备份和文档
- 🎤 准备演示说明（如何展示网站）
- ✅ 最终检查清单

**晚上（1h）**
- 😴 休息！准备会议

---

## ✅ 上线前检查清单

### 内容检查
- [ ] 所有文案已确认（无错别字）
- [ ] 所有数据准确（500万、40,000、99%等）
- [ ] Logo清晰显示
- [ ] 联系方式正确
- [ ] Canada Post Logo获得授权

### 功能检查
- [ ] 所有页面可访问
- [ ] 所有链接有效
- [ ] 表单提交正常
- [ ] 中英文切换正常
- [ ] 动画流畅不卡顿

### 性能检查
- [ ] 首屏加载<3秒
- [ ] 图片已优化（WebP格式）
- [ ] Lighthouse分数>90
- [ ] 移动端性能良好

### SEO检查
- [ ] Title和Description已设置
- [ ] Open Graph标签已添加
- [ ] Sitemap已生成
- [ ] robots.txt已配置
- [ ] Google Analytics已配置

### 兼容性检查
- [ ] Chrome ✓
- [ ] Safari ✓
- [ ] Firefox ✓
- [ ] Edge ✓
- [ ] iPhone Safari ✓
- [ ] iPad Safari ✓
- [ ] Android Chrome ✓

---

## 📎 附加资源

### 图片需求列表

#### 核心品牌资产
```
1. EIE Logo：
   - 格式：SVG + PNG（透明背景）
   - 尺寸：原始矢量 + 多尺寸导出
   - 用途：导航栏、页脚、品牌展示
   - 颜色方案：已提取（见设计规范部分）

2. Canada Post Logo：
   - 需获得使用授权
   - 高清 PNG/SVG 格式
   - 用于合作背书区域展示
```

#### 首页 Hero 区域
```
1. Hero 背景图/视频：
   - 推荐：航空物流场景/包裹流转动画
   - 尺寸：1920x1080px（图片）或 1920x1080 @ 30fps（视频）
   - 来源：高质量实景拍摄或 Unsplash/Pexels
   - 备选方案：使用渐变背景 + 动态图标
```

#### Global Direct Ecommerce Solution 业务板块（新增）
```
【前段物流场景 - 3张必备图片】

1. 飞机航空运输场景
   - 内容：货机起飞/机场货运装载场景
   - 尺寸：800x600px（16:9 比例）
   - 要求：展现国际航空运输能力和规模
   - 配文："Multi-carrier Air Resources"
   - 可选元素：包含多个航司标识更佳

2. 航班时刻表/运营看板
   - 内容：航班调度大屏或运营数据仪表盘
   - 尺寸：800x600px
   - 要求：体现专业运营管理和数据化
   - 配文："Daily Flight Guarantee"
   - 可选方案：设计运营数据可视化图表

3. 仓库分拣中心
   - 内容：自动化分拣线/包裹处理现场
   - 尺寸：800x600px
   - 要求：展现规模化作业和智能分拣能力
   - 配文："Smart Sorting System"
   - 关键要素：突出邮编分类标识

【末端服务场景 - 3张必备图片】

1. 海关清关文件/流程
   - 内容：CBSA 认证证书 + 清关报关单据
   - 尺寸：800x600px
   - 要求：展现专业清关资质
   - 配文："CBSA Certified | 99%+ Clear Rate"
   - 设计建议：证书 + 流程图组合展示

2. 末端仓库/配送中心
   - 内容：加拿大本地仓库内景/包裹整理场景
   - 尺寸：800x600px
   - 要求：整洁专业的仓储环境
   - 配文："Local Warehouse Network"
   - 关键元素：展现本地化服务能力

3. 派送公司车辆
   - 内容：Canada Post/Purolator/Eagleship 配送车
   - 尺寸：800x600px
   - 要求：品牌化配送车辆，展现多元派送
   - 配文："Multi-carrier Delivery | 2-9 Days"
   - 可选：多家派送公司车辆的组合展示
```

#### 其他运营场景
```
1. 公司设施照片：
   - 中国仓库外观/内景（15+城市网络）
   - 加拿大清关中心外观/内景
   - 办公环境（体现专业性）
   - 尺寸：1200x800px 或更高

2. 团队照片（可选）：
   - 客服团队工作场景
   - 仓库操作团队
   - 尺寸：1200x800px

3. 合作伙伴 Logo：
   - 航司 Logos（如已授权）
   - 末端派送合作方：Purolator、DHL、UPS、FedEx
   - Eagleship 自有品牌 Logo
   - 格式：PNG 透明背景，统一高度 80px
```

#### 图标和装饰元素
```
1. 功能图标：
   - 统一使用 Lucide React 图标库
   - 或设计自定义 SVG 图标（保持风格一致）
   - 图标色：使用 EIE 品牌蓝系

2. 装饰性图形：
   - 地图连线动画元素
   - 流程时间轴图标
   - 数据可视化图表
```

#### 图片获取优先级
```
P0（必须）：
- EIE Logo
- Hero 背景
- 前段物流 3 张（飞机、航班、分拣）
- 末端服务 3 张（清关、仓库、派送车）

P1（重要）：
- Canada Post Logo
- 中国仓库照片
- 加拿大仓库照片
- 合作伙伴 Logos

P2（可选）：
- 团队照片
- 办公环境
- 其他装饰性图片
```

#### 图片处理要求
```
- 格式：WebP（首选）+ JPEG（备用）
- 压缩：使用 Next.js Image 组件自动优化
- 响应式：准备 1x、2x、3x 版本
- 替代文本：所有图片必须有 alt 描述（SEO）
- 懒加载：首屏外图片使用懒加载
```

### 数据可视化需求
```
1. 地图：
   - 中国地图：标注15+城市
   - 加拿大地图：标注服务范围
   - 使用Leaflet + OpenStreetMap

2. 图表：
   - 时效分布柱状图（2-9天）
   - 月度包裹量趋势线（如有数据）
   - 使用Recharts库

3. 数字动画：
   - CountUp动画展示关键数据
   - 使用react-countup库
```

### 第三方服务
```
1. 表单提交：
   - 使用Resend或SendGrid发送邮件
   - 或直接调用API存储到数据库

2. Analytics：
   - Google Analytics 4
   - Vercel Analytics（自带）

3. 地图服务：
   - OpenStreetMap（免费）
   - 或Mapbox（有免费额度）
```

---

## 💰 预算估算

### 免费方案（推荐）
```
✓ Next.js + Vercel托管：     免费
✓ Shadcn UI组件：            免费
✓ OpenStreetMap地图：        免费
✓ Resend邮件服务：          免费（100封/天）
✓ 域名（如需新购）：         约$10-15/年

总计：$10-15/年（仅域名费用）
```

### 可选升级
```
• 专业域名邮箱（Google Workspace）： $6/月
• Mapbox地图服务（更美观）：         免费额度够用
• 付费字体许可（如需特殊字体）：     $99一次性
• 云数据库（如需存储表单）：         免费额度够用
```

---

## 📞 会议演示建议

### 演示流程（5-10分钟）
```
1. 首页 (2min)
   - 展示关键数据
   - 强调Canada Post合作关系
   - 突出四大核心优势

2. Services (2min)
   - 快速浏览服务链路
   - 展示中国网络覆盖
   - 强调清关专业性

3. Network (1min)
   - 交互式地图演示
   - 展示覆盖范围

4. Technology (1min)
   - 展示系统对接能力
   - 演示tracking功能

5. Why EIE (2min)
   - 对比优势说明
   - 总结核心竞争力

6. Contact (1min)
   - 展示联系方式
   - 邀请进一步洽谈
```

### 演示要点
- ✓ 用数据说话（500万、99%、40,000+）
- ✓ 强调Canada Post合作背书
- ✓ 突出差异化优势（无附加费、无排仓）
- ✓ 展示专业性（CBSA认证、系统对接）
- ✓ 保持自信和专业
- ✓ 准备应对可能的问题

---

## 🎯 成功衡量指标

### 会议目标
- [x] 网站成功上线并展示
- [ ] 获得至少3位决策者的名片/联系方式
- [ ] 安排至少1次后续深入洽谈
- [ ] 获得关于低价清关账号的明确回复

### 网站目标（会议后）
- [ ] 月独立访问量 > 500
- [ ] 平均停留时间 > 2分钟
- [ ] 跳出率 < 60%
- [ ] 表单提交 > 5次/月

---

## 📧 后续支持

### 会议后优化（Phase 2）
1. 添加案例详情页（成功案例深度介绍）
2. 添加博客/新闻模块
3. 添加在线报价计算器
4. 添加在线下单系统
5. 添加客户登录系统
6. SEO深度优化
7. 多语言扩展（法语）

### 维护建议
- 定期更新数据（包裹量、城市数等）
- 添加新的案例研究
- 保持内容新鲜度（新闻/公告）
- 监控网站性能
- 收集访客反馈并优化

---

## 📄 文档交付清单

本PRD完成后，您将获得：
- [x] 完整的产品需求文档（本文档）
- [ ] Next.js项目代码（4天后交付）
- [ ] 部署文档和维护指南
- [ ] 图片素材需求清单
- [ ] 会议演示脚本
- [ ] SEO优化建议

---

**项目代号**: EIE-Website-v1  
**创建日期**: 2025-11-01  
**交付日期**: 2025-11-05  
**文档版本**: 1.0

---

## 附录：常见问题解答

**Q: 4天时间够吗？**  
A: 采用Next.js + Shadcn UI的技术栈，组件开发速度极快。内容已经明确，主要是搭建和整合工作，4天完全可行。

**Q: 没有设计师怎么办？**  
A: Shadcn UI提供了开箱即用的美观组件，参考DHL/UPS等物流公司官网的布局结构，可以做出专业水准的网站。

**Q: 如果会议现场网络不好？**  
A: 建议准备：1) 网站本地版本 2) 录屏视频 3) PDF版本的网站截图

**Q: 后续如何更新内容？**  
A: 文案内容都在代码中，简单修改即可。或后期可接入Headless CMS（如Sanity）方便非技术人员更新。

**Q: 网站安全吗？**  
A: Next.js + Vercel部署自动提供HTTPS，表单提交做好验证即可。无敏感数据处理，安全性足够。

---

**祝您会议成功！有任何问题随时沟通！** 🚀
