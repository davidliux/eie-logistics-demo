# EIE官网图片素材需求清单

**项目**: EIE Logistics 官网
**创建日期**: 2025-11-04
**图片存放路径**: `/Users/david/ai开发项目/eiedemo官网/page/`
**总计图片数**: 20张 (P0: 9张, P1: 8张, P2: 3张)

---

## 目录结构规划

```
page/
├── logo/              # 品牌Logo
├── hero/              # 首页Hero区域
├── services/          # 业务场景图片
│   ├── china-ops/     # 中国运营场景
│   └── canada-ops/    # 加拿大运营场景
├── partners/          # 合作伙伴Logo
└── network/           # 网络地图可视化
```

---

## P0级别 - 必须图片 (9张)

### 1. 核心品牌资产

| 序号 | 文件名 | 用途 | 尺寸 | 格式 | AI生成提示词 |
|------|--------|------|------|------|--------------|
| P0-01 | `logo/eie-logo.svg` | 网站主Logo,用于导航栏、页脚 | 矢量,导出多尺寸 | SVG + PNG | **不适用AI生成** - 需使用现有品牌Logo `/Users/david/ai开发项目/eiedemo官网/page/logo.png`,转换为SVG格式并优化 |
| P0-02 | `logo/canada-post-logo.png` | Canada Post官方Logo,合作背书 | 400x200px | PNG透明背景 | **不适用AI生成** - 需从Canada Post官网下载官方Logo,或使用已授权素材,确保高清且背景透明 |

### 2. 前段物流核心场景 (3张)

| 序号 | 文件名 | 用途 | 尺寸 | 格式 | AI生成提示词 |
|------|--------|------|------|------|--------------|
| P0-03 | `services/china-ops/air-transport.jpg` | 国际航空运输能力展示 | 1600x900px (16:9) | JPEG/WebP | **提示词**:<br/>A professional photograph of a cargo aircraft being loaded at an international airport, modern logistics operations, workers loading freight containers onto a wide-body cargo plane, airport tarmac setting, blue sky, professional commercial aviation photography style, high detail, sharp focus, bright natural lighting, modern and clean aesthetic, colors: blue tones matching #144272 primary blue, emphasize scale and professional operations, wide angle view, 16:9 aspect ratio<br/><br/>**中文提示词**:<br/>专业的货运飞机装载场景摄影,国际机场货运区,工作人员正在将货物集装箱装载到宽体货机上,机场停机坪环境,蓝天背景,商业航空摄影风格,高细节,清晰对焦,明亮自然光,现代整洁美感,配色以蓝色调为主(#144272),突出规模化和专业运营,广角视角,16:9比例 |
| P0-04 | `services/china-ops/flight-schedule.jpg` | 航班调度管理能力 | 1600x900px (16:9) | JPEG/WebP | **提示词**:<br/>Modern logistics operations center dashboard, large digital display screens showing flight schedules and departure times, professional control room setting, multiple monitors displaying real-time data visualization, airline route maps, departure/arrival information, blue and white color scheme matching #144272, clean and modern interface design, professional lighting, high-tech atmosphere, data-driven logistics management, 16:9 aspect ratio<br/><br/>**中文提示词**:<br/>现代物流运营中心控制台,大型数字显示屏展示航班时刻表和起飞时间,专业控制室环境,多个显示器显示实时数据可视化,航线地图,航班起降信息,蓝白配色方案(#144272),简洁现代的界面设计,专业照明,高科技氛围,数据驱动的物流管理,16:9比例 |
| P0-05 | `services/china-ops/sorting-center.jpg` | 智能分拣系统展示 | 1600x900px (16:9) | JPEG/WebP | **提示词**:<br/>Modern automated parcel sorting facility, conveyor belts with packages, barcode scanning systems, postal code sorting equipment, warehouse interior with organized operations, workers in uniform, bright industrial lighting, clean and efficient workspace, emphasis on automation and scale, blue industrial equipment accents matching #144272, packages with postal labels visible, professional logistics photography, wide angle view, 16:9 aspect ratio<br/><br/>**中文提示词**:<br/>现代化自动包裹分拣设施,传送带上的包裹,条码扫描系统,邮编分拣设备,仓库内部有序运营,穿制服的工作人员,明亮的工业照明,整洁高效的工作空间,强调自动化和规模,蓝色工业设备点缀(#144272),包裹上可见邮政标签,专业物流摄影,广角视角,16:9比例 |

### 3. 末端服务核心场景 (3张)

| 序号 | 文件名 | 用途 | 尺寸 | 格式 | AI生成提示词 |
|------|--------|------|------|------|--------------|
| P0-06 | `services/canada-ops/customs-clearance.jpg` | 专业清关资质展示 | 1600x900px (16:9) | JPEG/WebP | **提示词**:<br/>Professional customs brokerage office scene, CBSA certification certificate displayed on wall, customs declaration documents on desk, professional customs broker at work, Canadian flag visible, official government forms and paperwork, professional business setting, natural office lighting, credibility and trust atmosphere, blue and white color scheme matching #144272, official and authoritative feel, 16:9 aspect ratio<br/><br/>**中文提示词**:<br/>专业清关经纪公司办公场景,墙上展示的CBSA认证证书,办公桌上的报关申报文件,专业报关员工作中,可见加拿大国旗,官方政府表格和文书,专业商务环境,自然办公室照明,可信赖的氛围,蓝白配色方案(#144272),官方权威感,16:9比例 |
| P0-07 | `services/canada-ops/canada-warehouse.jpg` | 加拿大本地仓储能力 | 1600x900px (16:9) | JPEG/WebP | **提示词**:<br/>Modern Canadian warehouse interior, organized shelving with packages, clean and well-lit space, workers processing shipments, forklift operations, inventory management system visible, Canadian maple leaf branding elements, professional logistics facility, blue industrial theme matching #144272, efficient operations atmosphere, packages being sorted and prepared for delivery, wide angle warehouse view, 16:9 aspect ratio<br/><br/>**中文提示词**:<br/>现代化加拿大仓库内景,有序的货架和包裹,整洁明亮的空间,工作人员处理货物,叉车作业,可见库存管理系统,加拿大枫叶品牌元素,专业物流设施,蓝色工业主题(#144272),高效运营氛围,包裹分拣和配送准备,仓库广角视角,16:9比例 |
| P0-08 | `services/canada-ops/delivery-vehicles.jpg` | 多元派送网络展示 | 1600x900px (16:9) | JPEG/WebP | **提示词**:<br/>Fleet of delivery vehicles in parking lot, Canada Post branded truck, Purolator van, modern delivery vehicles with company logos, clean and professional appearance, Canadian urban setting, blue sky background, vehicles parked in organized rows, emphasis on multi-carrier delivery network, blue and white color scheme matching #144272, professional commercial photography, wide angle view, 16:9 aspect ratio<br/><br/>**中文提示词**:<br/>停车场的配送车队,Canada Post品牌卡车,Purolator货车,带公司logo的现代配送车辆,整洁专业的外观,加拿大城市环境,蓝天背景,车辆有序停放,强调多承运商配送网络,蓝白配色方案(#144272),专业商业摄影,广角视角,16:9比例 |

### 4. Hero区域背景

| 序号 | 文件名 | 用途 | 尺寸 | 格式 | AI生成提示词 |
|------|--------|------|------|------|--------------|
| P0-09 | `hero/hero-background.jpg` | 首页Hero区域背景图 | 1920x1080px (16:9) | JPEG/WebP | **提示词**:<br/>Professional logistics hero image, container ship or cargo aircraft in motion, modern international shipping, blue gradient sky, sense of global connectivity and movement, aerial or elevated perspective, professional commercial photography style, blue color tones matching #144272 and #2C74B3, emphasis on scale and reliability, cinematic wide angle composition, suitable as website hero background with space for text overlay, 16:9 aspect ratio<br/><br/>**中文提示词**:<br/>专业物流主视觉图,集装箱货轮或货运飞机运动中,现代国际运输,蓝色渐变天空,全球互联互通感,航拍或高视角,专业商业摄影风格,蓝色调(#144272和#2C74B3),强调规模和可靠性,电影级广角构图,适合作为网站主背景并留出文字叠加空间,16:9比例 |

---

## P1级别 - 重要图片 (8张)

### 5. 合作伙伴Logo

| 序号 | 文件名 | 用途 | 尺寸 | 格式 | AI生成提示词 |
|------|--------|------|------|------|--------------|
| P1-01 | `partners/purolator-logo.png` | 末端派送合作方Logo | 统一高度80px | PNG透明背景 | **不适用AI生成** - 从Purolator官网下载官方Logo,处理为透明背景PNG,统一高度80px |
| P1-02 | `partners/dhl-logo.png` | 末端派送合作方Logo | 统一高度80px | PNG透明背景 | **不适用AI生成** - 从DHL官网下载官方Logo,处理为透明背景PNG,统一高度80px |
| P1-03 | `partners/ups-logo.png` | 末端派送合作方Logo | 统一高度80px | PNG透明背景 | **不适用AI生成** - 从UPS官网下载官方Logo,处理为透明背景PNG,统一高度80px |
| P1-04 | `partners/fedex-logo.png` | 末端派送合作方Logo | 统一高度80px | PNG透明背景 | **不适用AI生成** - 从FedEx官网下载官方Logo,处理为透明背景PNG,统一高度80px |
| P1-05 | `partners/eagleship-logo.png` | 自营品牌Logo | 统一高度80px | PNG透明背景 | **根据品牌设计** - 如已有Eagleship Logo使用现有素材,如需设计可用AI:<br/>Modern logistics company logo for "Eagleship", minimalist eagle wing symbol, blue color scheme matching #144272, professional and trustworthy design, simple and clean, suitable for delivery company branding, vector style illustration |

### 6. 网络地图可视化

| 序号 | 文件名 | 用途 | 尺寸 | 格式 | AI生成提示词 |
|------|--------|------|------|------|--------------|
| P1-06 | `network/china-map.png` | 中国网络覆盖地图 | 1200x900px (4:3) | PNG | **提示词**:<br/>Simplified map of China with major cities marked, 15+ city location pins highlighted in blue (#144272), modern minimal map design, white background, blue accent colors, clean lines, professional business style, cities include Beijing Shanghai Guangzhou Shenzhen Hangzhou marked with dots and labels, transportation network lines connecting cities, suitable for business presentation<br/><br/>**中文提示词**:<br/>简化的中国地图标注主要城市,15+城市位置用蓝色(#144272)标记,现代简约地图设计,白色背景,蓝色强调色,简洁线条,专业商务风格,标注北京上海广州深圳杭州等城市点和标签,连接城市的运输网络线,适合商务展示 |
| P1-07 | `network/canada-map.png` | 加拿大网络覆盖地图 | 1200x900px (4:3) | PNG | **提示词**:<br/>Simplified map of Canada with key cities marked, Vancouver Toronto Montreal highlighted with blue pins (#144272), modern minimal map design, white background, blue accent colors, clean lines, professional business style, delivery coverage zones indicated with subtle shading, transportation routes shown, suitable for business presentation<br/><br/>**中文提示词**:<br/>简化的加拿大地图标注关键城市,温哥华多伦多蒙特利尔用蓝色大头针(#144272)突出显示,现代简约地图设计,白色背景,蓝色强调色,简洁线条,专业商务风格,配送覆盖区域用浅色阴影表示,显示运输路线,适合商务展示 |

### 7. 设施展示 (可选实景或示意图)

| 序号 | 文件名 | 用途 | 尺寸 | 格式 | AI生成提示词 |
|------|--------|------|------|------|--------------|
| P1-08 | `services/china-warehouse.jpg` | 中国仓库设施展示 | 1600x900px (16:9) | JPEG/WebP | **提示词**:<br/>Modern logistics warehouse in China, exterior view of large industrial building, loading docks visible, trucks being loaded/unloaded, professional facility photography, blue sky, clean and organized appearance, Chinese urban/industrial setting, modern architecture, blue corporate branding elements matching #144272, professional commercial photography, wide angle view, 16:9 aspect ratio<br/><br/>**中文提示词**:<br/>中国现代物流仓库,大型工业建筑外观,可见装卸码头,卡车装卸货,专业设施摄影,蓝天,整洁有序的外观,中国城市/工业环境,现代建筑,蓝色企业品牌元素(#144272),专业商业摄影,广角视角,16:9比例 |

---

## P2级别 - 可选图片 (3张)

### 8. 补充场景素材

| 序号 | 文件名 | 用途 | 尺寸 | 格式 | AI生成提示词 |
|------|--------|------|------|------|--------------|
| P2-01 | `services/customer-service.jpg` | 24/7客服团队展示 | 1600x900px (16:9) | JPEG/WebP | **提示词**:<br/>Professional customer service center, multi-ethnic team wearing headsets, modern office environment, computer monitors displaying customer support systems, friendly and professional atmosphere, blue corporate theme matching #144272, natural office lighting, team collaboration, international business setting, 16:9 aspect ratio<br/><br/>**中文提示词**:<br/>专业客服中心,多元化团队佩戴耳机,现代办公环境,电脑显示器显示客户支持系统,友好专业的氛围,蓝色企业主题(#144272),自然办公照明,团队协作,国际商务环境,16:9比例 |
| P2-02 | `services/package-inspection.jpg` | 质量检验流程 | 1600x900px (16:9) | JPEG/WebP | **提示词**:<br/>Warehouse quality control inspection, worker examining packages on inspection table, barcode scanners and measuring equipment, organized inspection station, professional warehouse setting, bright industrial lighting, attention to detail and quality, blue work uniforms or equipment matching #144272, professional logistics photography, 16:9 aspect ratio<br/><br/>**中文提示词**:<br/>仓库质量控制检验,工作人员在检验台检查包裹,条码扫描仪和测量设备,有序的检验站,专业仓库环境,明亮的工业照明,注重细节和质量,蓝色工作服或设备(#144272),专业物流摄影,16:9比例 |
| P2-03 | `services/team-photo.jpg` | 团队合影 (可选) | 1600x900px (16:9) | JPEG/WebP | **提示词**:<br/>Professional corporate team photo, diverse group of logistics professionals, business casual attire, modern office or warehouse background, confident and friendly expressions, international team representing China-Canada business, blue corporate branding elements, professional business photography, natural lighting, group composition, 16:9 aspect ratio<br/><br/>**中文提示词**:<br/>专业企业团队合影,多元化物流专业团队,商务休闲着装,现代办公室或仓库背景,自信友好的表情,代表中加业务的国际团队,蓝色企业品牌元素,专业商务摄影,自然光,团队构图,16:9比例 |

---

## 图片制作优先级建议

### 第一批 (会议前必须完成 - P0核心9张)

1. **品牌资产** (2张): EIE Logo + Canada Post Logo
2. **Hero背景** (1张): hero-background.jpg
3. **前段物流** (3张): 飞机装载 + 航班调度 + 分拣中心
4. **末端服务** (3张): 清关文件 + 仓库 + 派送车辆

### 第二批 (会议后补充 - P1重要8张)

5. **合作伙伴Logo** (5张): Purolator, DHL, UPS, FedEx, Eagleship
6. **网络地图** (2张): 中国地图 + 加拿大地图  
7. **设施展示** (1张): 中国仓库外观

### 第三批 (长期优化 - P2可选3张)

8. **补充场景** (3张): 客服团队 + 质检流程 + 团队合影

---

## 图片制作技术要求

### 格式规范

- **Logo类**: SVG矢量格式优先,PNG透明背景备用
- **场景类**: WebP格式优先(体积小),JPEG备用(兼容性好)
- **地图类**: PNG格式(保证细节清晰)

### 尺寸规范

- **Hero背景**: 1920x1080px (Full HD)
- **业务场景**: 1600x900px (标准16:9)
- **地图可视化**: 1200x900px (4:3适合展示)
- **Logo**: 原始矢量 + 统一高度80px导出版本

### 质量要求

- **分辨率**: 至少72dpi web用,300dpi用于可能的印刷物料
- **压缩**: WebP品质80-90%,JPEG品质85-95%
- **文件大小**: 单张不超过500KB(Hero背景可放宽到1MB)
- **颜色空间**: sRGB色彩空间

### 命名规范

- 使用小写字母和连字符: `air-transport.jpg`
- 避免空格和特殊字符
- 文件名要有语义: `canada-warehouse.jpg` 优于 `img001.jpg`

---

## AI图片生成工具推荐

### 推荐工具

1. **Midjourney** - 最佳质量,适合所有场景类图片
2. **DALL-E 3** - 文字理解强,适合复杂场景描述
3. **Stable Diffusion** - 开源免费,本地运行可控性强
4. **Leonardo.ai** - 商业用途友好,批量生成效率高

### 生成参数建议

- **Aspect Ratio**: 使用 `--ar 16:9` (Midjourney) 或在提示词末尾注明
- **Style**: 添加 `professional photography` `commercial style` 等关键词
- **Quality**: 使用高质量模式,Midjourney使用 `--q 2`  
- **细节**: 在提示词中明确 `high detail` `sharp focus` `4K quality`

---

## 注意事项

1. **版权问题**: 
   - Canada Post Logo必须使用官方授权素材
   - 合作伙伴Logo仅用于展示合作关系,需确保符合使用规范
   - AI生成的场景图片用于商业用途需检查工具的版权条款

2. **品牌一致性**:
   - 所有图片色调尽量统一,与品牌蓝色系(#144272)协调
   - 避免过于花哨的效果,保持专业商务风格
   - 人物着装、环境整洁度保持一致标准

3. **文化适配**:
   - 中国场景图片体现中国城市/工业环境特征
   - 加拿大场景图片可适当加入枫叶、加拿大国旗等元素
   - 人物多元化,体现国际团队特色

4. **实景vs AI生成**:
   - 如有真实设施照片,优先使用实景(更可信)
   - 无法拍摄的场景(如航空运输)使用AI生成
   - 可将AI生成图作为参考,指导实景拍摄方向

---

## 图片清单核对表

### P0 - 必须 (9/9)

- [ ] P0-01: EIE Logo (SVG+PNG)
- [ ] P0-02: Canada Post Logo (PNG)
- [ ] P0-03: 飞机航空运输场景
- [ ] P0-04: 航班调度管理界面
- [ ] P0-05: 智能分拣中心
- [ ] P0-06: 清关资质展示
- [ ] P0-07: 加拿大仓库内景
- [ ] P0-08: 派送车队
- [ ] P0-09: Hero背景图

### P1 - 重要 (8/8)

- [ ] P1-01: Purolator Logo
- [ ] P1-02: DHL Logo
- [ ] P1-03: UPS Logo
- [ ] P1-04: FedEx Logo
- [ ] P1-05: Eagleship Logo
- [ ] P1-06: 中国网络地图
- [ ] P1-07: 加拿大网络地图
- [ ] P1-08: 中国仓库外观

### P2 - 可选 (3/3)

- [ ] P2-01: 客服团队
- [ ] P2-02: 质量检验
- [ ] P2-03: 团队合影

**完成进度**: __ / 20 张

---

## 联系与反馈

如图片生成遇到问题或需要调整,请及时沟通:

- 图片不符合预期: 提供具体反馈,调整AI提示词重新生成
- 技术问题: 检查文件格式、尺寸是否符合规范
- 版权疑问: 确认使用的素材来源和授权情况

**预祝图片制作顺利!** 🎨✨
