# 青科大美术馆｜V9 完整交互体验与可编辑画板

## 希望交互和 V9 HTML 一样

[下载 V9 完整交互体验插件（约 1.7 MB）](https://github.com/DOUDou-oss9/ubiquitous-pancake/raw/refs/heads/figma-prototype-download/figma-museum-v9-full-interaction.zip)

导入包内 manifest.json，运行 **青科大美术馆 · V9完整交互体验**，会直接打开手机应用窗口。**在插件窗口内操作，不是原生 ▶ Present。**

本插件直接使用 V9 的同一份 HTML/JavaScript：导航、筛选、收藏与计数、预约与记录、报名、搜索输入、校园滑动、本地图片导入、HTML 导出等逻辑保留。没有创建或修改任何画板，不触发 Starter 三页限制。

[完整说明](LIVE-DEMO.md) · [独立 HTML 原文件（保存后用浏览器打开）](prototype-v9.html)

画板编辑不会自动同步到 HTML 窗口。原生 Figma Present 不能直接执行网页 JavaScript；若课程要求只用 Present，此插件窗口不替代该要求。

## 编辑 Figma 图层与原型连线

[下载原生可编辑点击版 v3.2](https://github.com/DOUDou-oss9/ubiquitous-pancake/raw/refs/heads/figma-prototype-download/figma-museum-editable-v3.2.zip)

文字、图形、按钮和卡片可修改；原生 Prototype 用于预设页面/状态跳转，不能当作网页运行环境。

[已有文件的导航修复小插件](https://github.com/DOUDou-oss9/ubiquitous-pancake/raw/refs/heads/figma-prototype-download/figma-museum-navigation-fix-v3.2.zip) · [原生版说明](IMPORT-GUIDE.md)

## 回归证据

V9 原脚本逐一保留，在 Chromium 的 sandbox iframe 中完成 70 项检查，含真实输入、文件选择与下载，无 JavaScript 错误。入口通过官方 Plugin SDK 类型检查与窗口宿主模拟检查。没有直接连接真实 Figma 编辑器验收。

[回归结果](LIVE-VALIDATION.json) · [浏览器状态预览 GIF](v9-live-preview.gif)

本地演示不连接馆方真实业务系统；书法/园林为生成示意，真实校园照片待提供。本下载分支保留此前版本，不修改 main。
