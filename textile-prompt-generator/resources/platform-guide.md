# AI 绘图平台使用指南

## Midjourney 专用参数

### 常用参数
| 参数 | 说明 | 家纺推荐值 |
|------|------|-----------|
| `--ar` | 宽高比 | 1:1 (图案), 2:3 (窗帘), 4:3 (地毯) |
| `--tile` | 无缝平铺 | **必用** 用于生成可重复图案 |
| `--stylize` / `--s` | 艺术化程度 | 400-600 (平衡效果) |
| `--chaos` | 变化程度 | 10-30 (可控变化) |
| `--quality` / `--q` | 质量 | 1 (标准), 2 (高质量) |
| `--no` | 排除元素 | --no text, watermark |

### 版本选择
```
--v 6.1    # 最新版本，细节更好
--niji 6   # 动漫风格，适合儿童系列
```

### 家纺专用模板
```
[图案描述], textile pattern design, seamless pattern,
fabric texture, professional quality, 4K
--ar 1:1 --tile --s 500 --no text watermark
```

---

## Stable Diffusion 设置

### 推荐模型
| 模型 | 适用场景 |
|------|---------|
| SDXL | 高质量通用图案 |
| Realistic Vision | 真实面料质感 |
| DreamShaper | 艺术化设计 |

### 采样器推荐
| 采样器 | 说明 |
|--------|------|
| DPM++ 2M Karras | 平衡质量和速度 |
| Euler a | 快速，适合测试 |
| DPM++ SDE Karras | 高细节 |

### 推荐参数
```
Steps: 30-50
CFG Scale: 7-9
Size: 1024x1024 (后期可放大)
```

### 正向提示词模板
```
(masterpiece, best quality, high resolution),
textile pattern, [产品类型], [风格] design,
[颜色描述], [图案元素],
seamless repeat pattern, fabric texture,
professional textile design, detailed
```

### 负向提示词模板
```
(worst quality, low quality:1.4), blurry,
distorted, watermark, text, logo, signature,
jpeg artifacts, cropped, out of frame,
ugly, deformed, disfigured
```

### ControlNet 应用
```
Tile 模式: 确保图案无缝重复
Canny: 保持图案边缘清晰
```

---

## DALL-E 3 设置

### 提示词技巧
```
1. 使用自然语言描述
2. 明确指出"seamless textile pattern"
3. 描述具体的颜色和风格
4. 避免复杂的技术参数
```

### 模板
```
Create a seamless textile pattern for [产品类型] featuring [图案描述].
Use [颜色方案] colors with a [风格] aesthetic.
The pattern should be suitable for fabric printing with a [材质] texture appearance.
Professional quality, high resolution, tileable design.
```

---

## Leonardo.AI 设置

### 推荐模型
| 模型 | 适用场景 |
|------|---------|
| Leonardo Diffusion XL | 高质量通用 |
| DreamShaper v7 | 艺术化设计 |
| Absolute Reality | 真实质感 |

### 家纺图案设置
```
Tiling: ON (重要!)
Image Dimensions: 1024x1024
Guidance Scale: 7
```

---

## 通用最佳实践

### 1. 确保可平铺
```
关键词: seamless pattern, tileable design, repeat pattern
Midjourney: 必须使用 --tile 参数
SD: 使用 Tile ControlNet 或专用模型
```

### 2. 指定面料质感
```
cotton texture - 棉质
linen texture - 亚麻质感
silk sheen - 丝绸光泽
velvet texture - 天鹅绒
terry cloth - 毛巾质感
jacquard woven - 提花织物
```

### 3. 避免的元素
```
--no: text, watermark, logo, frame, border, 3d render, photograph
负向提示词: 避免生成水印、文字、边框
```

### 4. 颜色准确性
```
使用具体颜色名称: dusty pink, sage green, navy blue
避免模糊描述: pretty color, nice shade
可指定色调: warm tones, cool tones, muted colors
```

### 5. 分辨率建议
```
测试阶段: 512x512 或 768x768
最终输出: 1024x1024 或更高
印刷用途: 需后期使用放大工具 (如 Topaz Gigapixel)
```

---

## 后期处理建议

### 1. 无缝检测
```
使用 Photoshop 偏移滤镜检测接缝
或使用在线工具: seamlesstexture.io
```

### 2. 图案放大
```
工具推荐:
- Topaz Gigapixel AI
- Real-ESRGAN
- Magnific AI
```

### 3. 颜色调整
```
调整到符合 Pantone 色卡
考虑印刷色差 (CMYK 转换)
准备多个配色方案
```

### 4. 重复尺寸调整
```
根据产品调整图案大小:
床品: 通常 60-90cm 一个循环
窗帘: 30-60cm 一个循环
毛巾: 15-30cm 一个循环
```
