---
name: 家纺画稿提示词生成器
description: 自动生成专业的家纺产品设计画稿 AI 提示词，支持床品、窗帘、毛巾、地毯等多种家纺品类
---

# 🎨 家纺画稿提示词生成器

## 概述

这是一个专门用于生成家纺产品设计画稿 AI 提示词的技能。它可以帮助设计师快速生成高质量的 Midjourney、Stable Diffusion 或其他 AI 绘图工具的提示词。

---

## 支持的产品品类

| 品类 | 英文 | 常见类型 |
|------|------|----------|
| 床品 | Bedding | 四件套、被罩、床单、枕套 |
| 窗帘 | Curtains | 遮光帘、纱帘、罗马帘 |
| 毛巾 | Towels | 浴巾、面巾、方巾 |
| 地毯 | Rugs/Carpets | 地垫、区域地毯、床边毯 |
| 桌布 | Tablecloths | 餐桌布、茶几布 |
| 抱枕 | Throw Pillows | 沙发靠垫、抱枕套 |
| 毯子 | Blankets | 法兰绒毯、针织毯、夏凉被 |

---

## 设计风格库

### 现代风格 (Modern Styles)
- **极简主义** (Minimalist): 简洁线条、单色或双色、几何图形
- **北欧风** (Scandinavian): 自然色调、简约图案、温暖质感
- **现代奢华** (Modern Luxury): 金属元素、大理石纹理、深色调

### 传统风格 (Traditional Styles)
- **中式传统** (Chinese Traditional): 云纹、龙凤、牡丹、青花瓷
- **欧式古典** (European Classical): 大马士革、巴洛克、洛可可
- **波西米亚** (Bohemian): 民族图腾、流苏、混搭色彩

### 自然风格 (Natural Styles)
- **花卉图案** (Floral): 玫瑰、牡丹、小碎花、热带植物
- **动物图案** (Animal): 豹纹、蛇纹、鸟类、蝴蝶
- **自然元素** (Nature Elements): 树叶、海浪、山脉、星空

### 几何风格 (Geometric Styles)
- **抽象几何** (Abstract Geometric): 不规则形状、艺术拼贴
- **规则几何** (Regular Geometric): 条纹、格子、圆点、菱形
- **3D立体** (3D Effect): 立体视觉、光影效果

### 儿童风格 (Kids Styles)
- **卡通动漫** (Cartoon): 可爱动物、卡通人物
- **童话梦幻** (Fairy Tale): 城堡、公主、独角兽
- **教育主题** (Educational): 数字、字母、地图

---

## 色彩方案

### 经典配色
- **莫兰迪色系**: 灰粉、灰蓝、灰绿、低饱和度
- **大地色系**: 米色、棕色、驼色、卡其色
- **海洋色系**: 深蓝、宝蓝、青绿、白色
- **森林色系**: 墨绿、橄榄绿、苔绿、棕色

### 季节配色
- **春季**: 粉色、嫩绿、天蓝、鹅黄
- **夏季**: 白色、薄荷绿、柠檬黄、珊瑚橙
- **秋季**: 枫叶红、南瓜橙、金黄、深棕
- **冬季**: 酒红、墨绿、金色、银白

### 流行配色
- **马卡龙色**: 浅粉、浅蓝、浅紫、浅绿
- **高级灰**: 灰白、浅灰、中灰、深灰
- **撞色组合**: 蓝+橙、紫+黄、绿+粉

---

## 提示词生成模板

### 基础模板结构

```
[产品类型] + [图案风格] + [色彩方案] + [设计元素] + [材质效果] + [用途场景] + [技术参数]
```

### Midjourney 模板

```
[Product Type] textile pattern design, [Style] style, [Color Scheme] color palette, 
[Pattern Description], seamless pattern, flat lay, high quality fabric texture, 
professional textile design, 4K resolution --ar 1:1 --tile --stylize 500
```

### Stable Diffusion 模板

```
(masterpiece, best quality), textile pattern, [Product Type], [Style] design,
[Color Description], [Pattern Elements], seamless repeat pattern, fabric texture,
professional product design, high resolution, detailed
Negative: blurry, low quality, distorted, watermark
```

---

## 提示词生成流程

### 步骤 1: 确定产品信息
询问用户以下信息：
1. **产品类型**: 床品/窗帘/毛巾/地毯/其他
2. **目标市场**: 国内/出口/电商
3. **目标客群**: 年轻人/家庭/儿童/高端

### 步骤 2: 确定设计风格
1. **主风格**: 现代/传统/自然/几何/儿童
2. **子风格**: 具体的风格细分
3. **参考图片**: 如有参考图请提供

### 步骤 3: 确定色彩方案
1. **主色调**: 1-2个主要颜色
2. **辅助色**: 1-3个辅助颜色
3. **色彩情绪**: 温暖/清爽/优雅/活力

### 步骤 4: 生成提示词
根据以上信息，生成多个版本的提示词：
- **Midjourney 版本**
- **Stable Diffusion 版本**
- **DALL-E 版本**
- **通用描述版本**

---

## 示例提示词

### 示例 1: 北欧风格床品四件套

**Midjourney:**
```
Scandinavian bedding textile pattern, minimalist geometric design, 
soft grey and white color palette with subtle dusty pink accents, 
abstract line art and organic shapes, seamless pattern, 
cotton fabric texture, cozy bedroom aesthetic, 
professional textile design, 4K --ar 1:1 --tile --stylize 450
```

**中文描述:**
```
北欧风格床品布料图案，极简几何设计，柔和的灰白配色搭配淡粉点缀，
抽象线条艺术与有机形状，无缝重复图案，棉质面料质感，
温馨卧室美学，专业纺织品设计
```

### 示例 2: 中式传统窗帘

**Midjourney:**
```
Chinese traditional curtain fabric pattern, elegant oriental design,
deep navy blue and gold color scheme, auspicious cloud motifs,
subtle bamboo and plum blossom elements, luxurious silk texture,
seamless pattern, classical Chinese aesthetic,
high-end home decor, 4K --ar 2:3 --tile --stylize 600
```

**中文描述:**
```
中式传统窗帘面料图案，典雅东方设计，深藏蓝与金色配色方案，
祥云纹样，竹子与梅花元素点缀，奢华丝绸质感，
无缝图案，古典中式美学，高端家居装饰
```

### 示例 3: 儿童卡通毛巾

**Midjourney:**
```
Kids towel textile pattern, cute cartoon animal design,
playful pastel rainbow colors, adorable bunny and bear characters,
cheerful polka dots and stars background, soft terry cloth texture,
fun and kawaii style, seamless pattern, children's bathroom decor,
4K --ar 1:1 --tile --stylize 400
```

**中文描述:**
```
儿童毛巾布料图案，可爱卡通动物设计，活泼的马卡龙彩虹配色，
萌趣小兔子和小熊角色，欢快的波点和星星背景，
柔软毛圈质感，趣味可爱风格，无缝图案，儿童浴室装饰
```

### 示例 4: 波西米亚风地毯

**Midjourney:**
```
Bohemian area rug pattern design, ethnic tribal motifs,
warm terracotta rust and cream color palette with teal accents,
geometric aztec patterns mixed with floral medallions,
vintage worn texture, handwoven wool appearance,
boho chic home decor, seamless pattern, 4K --ar 4:3 --tile --stylize 550
```

---

## 高级技巧

### 1. 增加细节层次
```
添加: intricate details, layered patterns, subtle texture overlay
```

### 2. 指定印刷工艺
```
添加: digital print effect / screen print style / jacquard woven texture
```

### 3. 季节限定
```
添加: spring collection / summer vibes / autumn harvest / winter holiday
```

### 4. 市场定位
```
高端: luxury, premium, elegant, sophisticated
大众: affordable, trendy, practical, versatile
```

### 5. 可平铺设计
```
必加: seamless pattern, tileable design, --tile (Midjourney专用)
```

---

## 输出格式

当用户请求生成提示词时，按以下格式输出：

```markdown
## 🎨 家纺画稿提示词

### 📋 设计概要
- **产品类型**: [产品]
- **设计风格**: [风格]
- **配色方案**: [颜色]
- **目标客群**: [客群]

---

### 🖼️ Midjourney 提示词
\`\`\`
[提示词内容]
\`\`\`

### 🎯 Stable Diffusion 提示词
\`\`\`
正向提示词:
[正向提示词]

负向提示词:
[负向提示词]
\`\`\`

### 📝 中文设计描述
[中文描述，可用于设计文档或与供应商沟通]

---

### 💡 设计建议
[针对该设计的专业建议]
```

---

## 使用方式

直接告诉我你想要的家纺设计，例如：
- "帮我生成一个北欧风格床品四件套的画稿提示词"
- "我需要一款适合夏季的清新窗帘设计"
- "生成儿童房抱枕的可爱图案提示词"
- "设计一款高端中式风格的地毯图案"

我会根据你的需求，自动生成专业的 AI 绘图提示词！
