# AI Visualization Toolkit

一套交互式的AI/CNN原理可视化工具集，帮助直观理解深度学习的核心概念。

## 项目特点

- **交互式学习** - 通过动画和交互操作理解AI原理
- **可视化丰富** - 结合GSAP、Three.js、ECharts等现代前端技术
- **中文友好** - 界面和注释均为中文，便于理解

## 功能模块

### 1. CNN训练可视化 (CNN0304.html)

展示卷积神经网络的训练过程：
- 卷积核滑动动画
- 正向传播计算过程
- 反向传播梯度更新
- 多种推理模式（正方形、小三角形）

### 2. AI核心原理演示 (modeltrain.html)

直观展示AI基础概念：
- **梯度下降** - 小球沿抛物线滚动的动画，理解学习率的作用
- **卷积计算** - 卷积核扫描图像的动态过程

### 3. 模型推理可视化

- `inference_square.html` - 正方形图案推理
- `inference_small_triangle.html` - 小三角形图案推理

### 4. 性能分析仪表板 (profiling.html)

大模型训练任务的性能扫描结果展示：
- 动态性能球评分
- 桑基图数据流分析
- 训练瓶颈识别

### 5. 动画效果演示

- `liquid-animation.html` - SVG液态变形动画
- `morph-example.html` - GSAP MorphSVG形状变换
- `host-device-visualization.html` - Three.js 3D数据流可视化

## 技术栈

| 技术 | 用途 |
|------|------|
| [GSAP](https://greensock.com/gsap/) | 高性能动画引擎 |
| [MorphSVGPlugin](https://greensock.com/morphsvg/) | SVG形状变换 |
| [Three.js](https://threejs.org/) | 3D可视化 |
| [ECharts](https://echarts.apache.org/) | 数据图表 |
| [Tailwind CSS](https://tailwindcss.com/) | UI样式框架 |

## 快速开始

### 方式一：直接打开

双击任意 `.html` 文件即可在浏览器中查看。

### 方式二：本地服务器

```bash
# 使用 Node.js
node server.js

# 或使用 Python
python -m http.server 8080
```

然后访问 `http://localhost:8080`

## 目录结构

```
wzh/
├── CNN0304.html              # CNN训练可视化（主入口）
├── modeltrain.html           # AI核心原理演示
├── inference_square.html     # 正方形推理
├── inference_small_triangle.html  # 小三角形推理
├── profiling.html            # 性能分析仪表板
├── liquid-animation.html     # 液态动画
├── morph-example.html        # SVG变形演示
├── host-device-visualization.html  # 3D数据流
├── server.js                 # 本地服务器
├── js/                       # JavaScript库
│   ├── gsap.min.js
│   ├── MorphSVGPlugin.min.js
│   └── ...
├── svg/                      # SVG资源
└── images/                   # 图片资源
```

## 学习路径建议

1. **入门** - 从 `modeltrain.html` 开始，理解梯度下降和卷积基础
2. **进阶** - 查看 `CNN0304.html`，深入了解CNN训练过程
3. **应用** - 体验推理页面，观察模型如何识别不同图案
4. **扩展** - 探索动画和3D可视化效果

## 适用人群

- AI/深度学习初学者
- 需要直观理解CNN原理的开发者
- 前端动画技术爱好者
- 教育培训场景

## License

MIT License
