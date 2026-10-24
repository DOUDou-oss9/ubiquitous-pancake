# 青科大美术馆 · 原生可编辑交互版 v3

[点击下载 Figma 原生可编辑交互安装包（ZIP，约 14.5 MB）](https://github.com/DOUDou-oss9/ubiquitous-pancake/raw/refs/heads/figma-prototype-download/figma-museum-editable-v3.zip)

本版重新创建 Figma Text、矢量、按钮和卡片 Frame，不使用整页图片作为界面。书法与园林等真正的配图仍为可替换图片。

## 安装与使用

1. 解压新版 ZIP，在 Figma 桌面端选择 Plugins → Development → Import plugin from manifest，选择新版 manifest.json。
2. 运行 **青科大美术馆 · 原生可编辑交互版**。不要运行旧的视觉还原修正版。
3. 会新增页面，不改动旧页面。直接编辑文字、图形、按钮和卡片；在右侧 Prototype 面板修改跳转。
4. 点击右上角 **Present** 体验点击跳页。编辑画布中的点击是选中图层。

[完整使用说明](IMPORT-GUIDE.md) · [点击跳转清单](PROTOTYPE-LINKS.csv)

## 检查范围

- 约 2980 个可编辑 Text 和 716 个矢量组。
- 983 个按钮/卡片 Frame 直接绑定交互，无备用透明热区替代主要按钮。
- 20 个页面状态和112个面板状态均可从流程起点到达。
- 修改文字、移动按钮后，模拟结构检查确认链接仍附着在相同按钮上。
- 透明展架、原生滚动及 Smart Animate 组件保留。

检查为官方 SDK 类型和模拟节点验证，尚未连接真实 Figma 编辑器运行。字体可用性可能影响换行，实际导入后需要核对。布局可以编辑，但并非完整 Auto Layout 设计系统。

不执行真实搜索输入、文件上传/导出或后台持久化。书法与园林为生成示意，非真实师生作品；校园实拍待补充。

此前版本的固定下载链接保留；通用安装包文件名同步更新到 v3。本分支仅用于交付，不修改 main。
