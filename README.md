<!--
 * @Author: huanggk
 * @Date: 2025-07-07 18:35:48
 * @LastEditTime: 2025-07-07 18:40:35
 * @LastEditors: huanggk
 * @Description: 
 * @FilePath: \gas-pipeline-edit-dev\README.md
-->
# 🔥 燃气管网矢量数据编辑Demo

[![预览地址](https://img.shields.io/badge/预览-Demo-brightgreen)](https://huanggk7.github.io/gas-pipeline-edit-dev/)

## 📝 项目简介

这是一个基于Web的燃气管网矢量数据编辑演示系统，旨在提供直观、高效的燃气管网地理信息可视化和编辑功能。系统支持多种地图底图和矢量瓦片数据的加载，以及丰富的几何图形绘制和编辑功能，为燃气管网规划、管理和维护提供便捷的工具支持。

## ✨ 功能特性

- **多源地图展示**：支持加载多种地图底图和矢量瓦片数据，提供清晰的燃气管网地理信息展示
- **矢量数据编辑**：允许用户在地图上绘制点、线、面等几何图形，模拟燃气管网的不同元素（如阀门、管道、区域等）
- **符号化配置**：针对不同类型的几何图形（点、线、面），可自定义符号样式，包括颜色、大小、图标等
- **精准捕捉功能**：在绘制和编辑过程中，提供捕捉功能，帮助用户更精准地定位和连接几何图形
- **丰富工具栏操作**：提供多种工具栏操作按钮，如切换绘制模式、禁用编辑、清除地图数据等
- **属性信息查看**：支持点击查看管线的详细属性信息，包括ID、名称、类型等

## 🛠️ 技术栈

- **前端框架**：[Vue 3](https://vuejs.org/) - 用于构建用户界面和管理应用状态
- **地图库**：
  - [Maptalks](https://maptalks.org/) - 用于地图的渲染和交互操作，支持矢量数据的编辑和可视化
- **构建工具**：[RsBuild](https://rsbuild.dev/) - 用于项目的构建、打包和开发服务器的启动
- **类型检查**：[TypeScript](https://www.typescriptlang.org/) - 为代码提供类型检查，提高代码的可维护性和健壮性
- **包管理器**：[pnpm](https://pnpm.io/) - 高效的Node.js包管理器

## 🌟 项目特点

- **高性能矢量瓦片**：使用`19091`条街道数据模拟燃气管网，将GeoJSON数据转换为矢量瓦片数据，显著提高地图渲染性能和数据加载效率
- **全面的几何图形支持**：支持点、线、面等多种几何图形的绘制和编辑，满足不同燃气管网元素的表达需求
- **实时属性信息展示**：点击管线时，即时显示管线的详细属性信息，便于用户了解和分析管网数据
- **友好的用户交互**：精心设计的用户界面和交互方式，使操作更加直观和高效

## 📦 安装与运行

### 环境要求

- Node.js（版本 >= 22）
- pnpm（推荐使用最新版本）

### 安装依赖

```bash
# 克隆项目
git clone https://github.com/huanggk7/gas-pipeline-edit-dev.git

# 进入项目目录
cd gas-pipeline-edit-dev

# 安装依赖
pnpm install
```

### 启动开发服务器

```bash
# 启动开发服务器
pnpm dev
```

### 构建生产版本

```bash
# 构建生产版本
pnpm build
```

## 🚀 未来计划

1. 使用[WFS](https://www.ogc.org/standards/wfs/)或[OGC API - Features](https://ogcapi.ogc.org/features/)标准实现数据编辑结果保存到数据库
2. 在数据库或后端实现矢量瓦片diff更新功能
3. 修改maptalks底层矢量瓦片更新逻辑
4. 添加更多高级编辑功能，如拓扑编辑、批量属性编辑等

## 📄 许可证

[MIT](LICENSE)