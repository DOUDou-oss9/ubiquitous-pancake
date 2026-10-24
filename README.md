# 青科大美术馆 · Figma 可交互原型安装包

[点击下载 Figma 交互安装包（ZIP，约 8.4 MB）](https://github.com/DOUDou-oss9/ubiquitous-pancake/raw/refs/heads/figma-prototype-download/figma-museum-interactive.zip)

## 安装

1. 下载并解压整个 ZIP。
2. 使用 Figma 桌面端打开一个 Design 文件。
3. Plugins → Development → Import plugin from manifest，选择解压后的 manifest.json。
4. 从 Development 菜单运行「青科大美术馆 · 可交互原型导入」。
5. 点击右上角 Present，选择完整浏览、校园服务或校园滑动流程。

插件会新增独立页面，不修改原有页面。无需服务器、npm 或网络权限。

[完整安装与交互范围说明](IMPORT-GUIDE.md)

包含原生校园卡片横向滚动、Smart Animate 组件、主页面导航与演示弹层。Figma 中搜索、上传、真实数据提交等浏览器功能不执行。书法、园林为生成示意，不是青科大真实师生作品；校园实景仍待补充。

已完成 API 类型与模拟结构检查，尚未在真实 Figma 编辑器中运行验证。运行后请先用 Present 检查滑动和导航。

此分支仅用于存放安装包，不改动 main 分支。SHA-256 校验值见 SHA256SUMS。
