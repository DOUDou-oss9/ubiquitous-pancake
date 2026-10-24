# 青科大美术馆 · 免费版兼容可编辑交互 v3.1

[点击下载 Starter 兼容安装包（ZIP，约 14.5 MB）](https://github.com/DOUDou-oss9/ubiquitous-pancake/raw/refs/heads/figma-prototype-download/figma-museum-editable-v3.1.zip)

## 修复 Starter 三页上限报错

旧插件新建 Page 会触发 Starter 的每文件 3 页限制。本版不调用 createPage，直接在当前 Page 右侧放置画板，因此无需升级套餐。

保留当前页面名称、已有图层的位置与原型流程起点。会在已有内容之外留出间距，完成后自动定位。App 界面使用 Frame 承载，不需要多个 Page。

## 使用

1. 解压新版 ZIP，用 Figma 桌面端导入新版 manifest.json。
2. 运行 **青科大美术馆 · 免费版兼容可编辑交互**。
3. 使用右上角 Present，选择带「可编辑版 v3.1」的流程；编辑模式可以修改原生文字、图形、按钮和卡片。

[完整使用说明](IMPORT-GUIDE.md) · [跳转清单](PROTOTYPE-LINKS.csv)

可编辑图层与交互能力延续 v3。已按官方 SDK 做类型检查，并在模拟“三页已满且 createPage 禁止”的环境通过结构检查，创建 Page 调用次数为 0；原有图层与流程保留。真实编辑器中的字体和排版仍需导入后核对。

版本历史下载链接保留，通用安装包同步为当前兼容版。本分支仅用于交付，不修改 main。
