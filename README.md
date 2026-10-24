# 青科大美术馆 · Figma 视觉还原修正版 v2

[点击下载修正版安装包（ZIP，约 19 MB）](https://github.com/DOUDou-oss9/ubiquitous-pancake/raw/refs/heads/figma-prototype-download/figma-museum-interactive-v2.zip)

修复旧 SVG 导入造成的校门变黑、图标填实、比例失真、透明材质丢失和开屏内容错误。采用 2× 高清原稿视觉底层与 Figma 原生交互层；展架与底栏单独使用原生半透明填充和 Background Blur。

## 安装

1. 解压新版 ZIP。
2. 使用 Figma 桌面端，Plugins → Development → Import plugin from manifest，选择新版 manifest.json。
3. 运行 **青科大美术馆 · 视觉还原修正版**，不要运行旧插件。
4. 会新增一个独立页面；点击右上角 **Present** 操作。编辑画布中的点击只会选中图层，不会跳页。

[完整安装说明与能力范围](IMPORT-GUIDE.md)

## 核对画面

- [浏览器原稿：首页](reference-home.png)
- [浏览器原稿：正确启动页](reference-startup.png)

这些是原稿核对图，不是 Figma 编辑器截图。

## 内容

覆盖 20 个主要页面状态和 112 个面板状态，包括主页面导航、分类、服务身份、四个展览的预约身份/日期/勾选、作品和活动详情、校园横滑与独立 Smart Animate。

视觉层为高清图片，整页文字不可逐字编辑；原生滚动、玻璃材质、交互热区及组件可以编辑。不执行真实搜索输入、文件上传/导出或后台持久化。书法和园林为生成示意，校园实拍仍待补。

已完成官方 API 类型检查、资源比例核对和模拟 Figma 结构检查，结果见 VALIDATION.json。没有实际连接用户的 Figma 编辑器，仍需导入后用 Present 核对效果。

仅更新独立下载分支，不修改 main。原有安装包文件名也同步指向本次修正版，以减少继续下载旧包的问题。
