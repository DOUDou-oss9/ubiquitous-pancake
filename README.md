# 青科大美术馆｜原生交互图、可编辑画板与完整演示

## 在 Figma 画布里查看、编辑与播放原型图

[下载原生原型交互图插件（约 207 KB）](https://github.com/DOUDou-oss9/ubiquitous-pancake/raw/refs/heads/figma-prototype-download/figma-museum-native-prototype-map-v4.zip)

在已有手机画板所在的 Page 导入 manifest.json，运行 **青科大美术馆 · 原生原型交互图**。

会在画布右侧生成可编辑的总览、24 个可点击节点和可见流程线。节点连接到已有真实画板或弹层；保留原有手机按钮的 Prototype 动作。点击右上角 Present，选择「原型图 / 总览与路径」或「原生应用 / 首页点击体验」。不打开插件演示窗口，不新建 Page。

[安装及使用说明](PROTOTYPE-MAP.md) · [布局预览](native-prototype-map-preview.png)

尚无手机画板时，先导入 [原生可编辑版 v3.2](https://github.com/DOUDou-oss9/ubiquitous-pancake/raw/refs/heads/figma-prototype-download/figma-museum-editable-v3.2.zip)，再运行原型图插件。

## 体验与 V9 HTML 相同的完整运行逻辑

[下载 V9 完整交互插件](https://github.com/DOUDou-oss9/ubiquitous-pancake/raw/refs/heads/figma-prototype-download/figma-museum-v9-full-interaction.zip) · [说明](LIVE-DEMO.md)

直接运行 V9 原始脚本，交互在插件窗口中；原生 Present 使用预设页面/状态，不运行网页 JavaScript。两种表现层不自动同步，任意搜索输入、完整记录联动与文件处理在 V9 窗口或独立 HTML 中体验。

## 检查

原生图插件通过 API 类型与模拟已有文件检查：24 个节点目标有效、100 个导航入口检查、既有画板位置和流程保留、createPage/showUI 调用均为 0。预览为布局渲染，不是真实 Figma 运行截图；实际导入后仍需核对 Present。[检查结果](MAP-VALIDATION.json)

V9 运行逻辑通过 70 项浏览器沙箱检查。此前版本的下载链接全部保留，本分支不修改 main。
