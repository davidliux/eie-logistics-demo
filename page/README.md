# EIE官网图片资源目录

本目录用于存放EIE官网的所有图片和Logo素材。

## 目录结构

```
page/
├── logo/              # 品牌Logo
│   ├── eie-logo.svg          # EIE主Logo (SVG矢量格式)
│   ├── eie-logo.png          # EIE主Logo (PNG备用格式)
│   └── canada-post-logo.png  # Canada Post官方Logo
├── hero/              # 首页Hero区域
│   └── hero-background.jpg   # Hero背景图 (1920x1080px)
├── services/          # 业务场景图片
│   ├── china-ops/     # 中国运营场景
│   │   ├── air-transport.jpg      # 航空运输场景 (1600x900px)
│   │   ├── flight-schedule.jpg    # 航班调度界面 (1600x900px)
│   │   ├── sorting-center.jpg     # 智能分拣中心 (1600x900px)
│   │   └── china-warehouse.jpg    # 中国仓库外观 (1600x900px, P1)
│   └── canada-ops/    # 加拿大运营场景
│       ├── customs-clearance.jpg  # 清关资质展示 (1600x900px)
│       ├── canada-warehouse.jpg   # 加拿大仓库内景 (1600x900px)
│       ├── delivery-vehicles.jpg  # 派送车队 (1600x900px)
│       ├── customer-service.jpg   # 客服团队 (1600x900px, P2)
│       ├── package-inspection.jpg # 质量检验 (1600x900px, P2)
│       └── team-photo.jpg         # 团队合影 (1600x900px, P2)
├── partners/          # 合作伙伴Logo
│   ├── purolator-logo.png    # Purolator Logo (高度80px)
│   ├── dhl-logo.png          # DHL Logo (高度80px)
│   ├── ups-logo.png          # UPS Logo (高度80px)
│   ├── fedex-logo.png        # FedEx Logo (高度80px)
│   └── eagleship-logo.png    # Eagleship自有品牌 (高度80px)
└── network/           # 网络地图可视化
    ├── china-map.png         # 中国网络覆盖地图 (1200x900px)
    └── canada-map.png        # 加拿大网络覆盖地图 (1200x900px)
```

## 图片命名规范

- 使用小写字母和连字符: `air-transport.jpg`
- 避免空格和特殊字符
- 文件名要有语义性,便于识别

## 文件格式要求

- **Logo**: SVG矢量格式优先, PNG透明背景备用
- **场景图片**: WebP格式优先(体积小), JPEG备用(兼容性好)
- **地图**: PNG格式(保证细节清晰)

## 质量标准

- **分辨率**: Web用72dpi, 印刷用300dpi
- **压缩**: WebP品质80-90%, JPEG品质85-95%
- **文件大小**: 单张不超过500KB (Hero背景可1MB)
- **颜色空间**: sRGB

## 当前状态

目前已有文件:
- ✅ logo.png (EIE Logo, 需转换为SVG)
- ✅ 首页图片.png (可能用于Hero背景, 需重命名)

待补充的P0级别图片: 7张
待补充的P1级别图片: 8张  
待补充的P2级别图片: 3张

详细清单请参考: `/Users/david/specs/001-prd-eie/IMAGE_REQUIREMENTS.md`

## 使用说明

在HTML中引用图片:

```html
<!-- Logo -->
<img src="page/logo/eie-logo.svg" alt="EIE Logistics">

<!-- Hero背景 -->
<div style="background-image: url('page/hero/hero-background.jpg')"></div>

<!-- 业务场景 -->
<img src="page/services/china-ops/air-transport.jpg" alt="Air Transport">

<!-- 合作伙伴Logo -->
<img src="page/partners/purolator-logo.png" alt="Purolator">
```

## 备注

所有图片路径均相对于项目根目录,在HTML中使用相对路径即可正确加载。
