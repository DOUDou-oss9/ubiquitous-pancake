# 青科大美术馆｜原生交互图整合修正版 v4.1

[下载一次生成可编辑画板、原生交互与总览的整合修正版（约 14.5 MB）](https://github.com/DOUDou-oss9/ubiquitous-pancake/raw/refs/heads/figma-prototype-download/figma-museum-native-integrated-v4.1.zip)

## 本次解决 Reaction destination rejected

旧版把当前导航、分类或已选状态连回自身；Figma 不允许 NAVIGATE 指向来源所属的同一最外层画板。旧版只检查目标 ID，漏掉了这个规则，错误导致后续连线没能生成。

本版按动作区分校验同页最外层目标、滚动目标和组件变体。当前选中项保持原位，不再写自跳转；单个目标异常会记录并跳过，不中断整个导入。

## 使用

1. 解压新版 ZIP，在 Figma 桌面端导入 manifest.json。
2. 运行 **青科大美术馆 · 原生交互图整合修正版 v4.1**。
3. 在当前 Page 的新区域一次生成全部画板、连线和总览；原有画板保留，不新建 Page。
4. 点击 Present，选择 **v4.1 手机应用 / 首页** 或 **v4.1 总览 / 原型交互图**，避免进入旧的 Flow 1。

[完整修复说明](NATIVE-INTEGRATED-FIX.md)

## 验证

更严格的模拟检查先复现旧版同类错误，再验证新版本：20 个主状态、112 个面板状态、24 个总览节点均可到达；安全忽略 152 个重复/自指动作；无无效目标、无 API 拒绝；保留已有设计与流程，createPage 调用为 0。[检查结果](STRICT-REACTION-VALIDATION.json)

当前没有真实 Figma 编辑器连接，导入后仍需实际核对。原生原型使用预设交互，不执行网页 JavaScript。

## 已有完整画板，只修复总览

[原型图安全修复小包 v4.1](https://github.com/DOUDou-oss9/ubiquitous-pancake/raw/refs/heads/figma-prototype-download/figma-museum-prototype-map-safe-v4.1.zip)

如果旧版导入中途报错，建议使用上面的完整整合包，以恢复旧导入从未完成的连接。此前 v4 原型图下载地址也已同步为安全修复版本。

## 完整 V9 运行体验

[完整 V9 演示插件窗口](https://github.com/DOUDou-oss9/ubiquitous-pancake/raw/refs/heads/figma-prototype-download/figma-museum-v9-full-interaction.zip) · [说明](LIVE-DEMO.md)

它运行网页原脚本；原生画板可以编辑且有 Prototype 连线，但不承载任意搜索输入、文件操作和后台状态逻辑。两者不自动同步。本分支不修改 main。
