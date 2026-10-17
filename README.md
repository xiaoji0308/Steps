# 智能步数管理（HyperOS）

<p align="center">
  <strong>为 Xiaomi HyperOS 打造的步数管理模块</strong><br>
  通过 KernelSU / Magisk 与 WebUI，便捷管理模块运行状态和基础配置。
</p>

<p align="center">
  <a href="https://github.com/xiaoji0308/Steps/releases"><img alt="下载 Releases" src="https://img.shields.io/badge/下载-Releases-5865F2?style=for-the-badge&logo=github&logoColor=white"></a>
  <a href="https://t.me/Stepsxxx"><img alt="Telegram 群组" src="https://img.shields.io/badge/Telegram-交流群-26A5E4?style=for-the-badge&logo=telegram&logoColor=white"></a>
  <a href="https://www.coolapk.com/u/1547334"><img alt="酷安主页" src="https://img.shields.io/badge/酷安-个人主页-19B75A?style=for-the-badge"></a>
</p>

<p align="center">
  <a href="https://github.com/xiaoji0308/Steps/issues">反馈问题</a> ·
  <a href="https://github.com/xiaoji0308/Steps/releases">版本下载</a> ·
  <a href="https://t.me/Stepsxxx">加入交流群</a>
</p>

---

## 📖 项目简介

**智能步数管理**（模块 ID：`S-T-E-P-S`）是面向 Xiaomi HyperOS 环境的 KernelSU / Magisk 模块。它提供手机端 WebUI 控制面板，帮助用户管理步数任务的运行状态、重启相关进程，并调整模块提供的基础选项。

项目持续迭代中。不同设备、系统版本和 Root 环境可能存在差异，实际功能以安装包中的 WebUI 和模块行为为准。

## ✨ 功能特色

| 功能 | 说明 |
| --- | --- |
| 🎛️ **运行控制** | 开始运行、停止计步任务、重启相关进程、刷新当前状态 |
| ⚙️ **基础配置** | 管理午夜后自动重新运行、运行日志保留及页面提供的其他选项 |
| 📱 **移动端 WebUI** | 卡片式布局，适合在手机屏幕上查看和操作 |
| 🔔 **版本更新检查** | 检查 GitHub Release 信息，并提供发布页入口 |
| 🧩 **模块化管理** | 通过 KernelSU / Magisk 安装、启用和管理模块 |

> **说明：** 更新检查用于提示版本信息，不等于自动下载或自动安装。发现新版本后，请按发布说明下载 ZIP 并通过 KernelSU / Magisk 安装。

## 📦 下载与安装

1. 打开 **[GitHub Releases 下载页](https://github.com/xiaoji0308/Steps/releases)**。
2. 下载对应版本的模块 ZIP 安装包。
3. 打开设备上的 KernelSU 或 Magisk 管理器，选择从本地安装 ZIP。
4. 按安装器提示完成操作；如果安装器要求重启，请重启设备。
5. 安装完成后打开模块 WebUI，确认运行状态正常，再按需调整配置。

**更新前建议：** 保留当前可用的安装包，并阅读对应 Release 的更新说明。请勿将源码压缩包误当作模块安装包；应下载 Release 附件中的可安装 ZIP。

## 🕹️ WebUI 使用说明

- **开始运行：** 启动模块提供的步数管理任务。
- **停止计步：** 停止当前计步任务。
- **重启进程：** 重启模块相关进程。
- **刷新状态：** 重新读取并显示运行状态。
- **基础配置：** 根据页面提示调整自动重新运行、日志保留等选项。
- **检查更新：** 查询仓库发布信息并显示检查结果。
- **查看发布页：** 打开 GitHub Releases 页面，查看版本说明和安装包。

页面选项可能随版本调整，请以当前安装版本显示的内容为准。

## 🔄 版本更新说明

- **最新版本与安装包：** [Releases](https://github.com/xiaoji0308/Steps/releases)
- **最新 Release 信息：** [GitHub API](https://api.github.com/repos/xiaoji0308/Steps/releases/latest)

如果 WebUI 提示发现新版本，手机上已安装的模块不会因此自动改变；需要下载新 ZIP 并通过 KernelSU / Magisk 安装，才能完成更新。

## ❓ 常见问题

### 更新检查失败

1. 检查设备网络是否能够访问 GitHub。
2. 确认仓库已经发布 Release，而不只是提交了代码或上传了普通文件。
3. 确认 Release 附件中有可安装的模块 ZIP。
4. 如果暂时无法检查更新，可先从 [Releases 页面](https://github.com/xiaoji0308/Steps/releases) 手动下载并安装。

### 安装后页面仍显示旧内容

- 确认安装的是最新下载的 ZIP，而不是之前保存的旧包。
- 在 KernelSU / Magisk 中确认模块已启用。
- 关闭 WebUI 后重新打开；必要时重启设备。
- 如果问题仍然存在，反馈时请附上模块版本、系统版本、Root 方案和错误截图。

## 💬 交流与反馈

欢迎加入交流群、关注酷安主页，或通过 GitHub 提交问题与建议。

- ✈️ **Telegram 交流群：** [https://t.me/Stepsxxx](https://t.me/Stepsxxx)
- 📱 **酷安个人主页：** [https://www.coolapk.com/u/1547334](https://www.coolapk.com/u/1547334)
- 🐛 **GitHub Issues：** [提交问题 / 建议](https://github.com/xiaoji0308/Steps/issues)
- 📥 **GitHub Releases：** [下载模块 / 查看更新](https://github.com/xiaoji0308/Steps/releases)

提交反馈时，建议描述设备型号、HyperOS 版本、KernelSU / Magisk 版本、模块版本和复现步骤。请勿公开账号密码或其他敏感信息。

## ⚠️ 免责声明

本项目按现状提供。不同设备、系统版本、Root 方案及第三方应用环境可能影响模块行为。请自行评估使用风险，并在更新前做好必要备份。

---

<p align="center">
  如果这个项目对你有帮助，欢迎点亮 ⭐、提交反馈，或加入 Telegram 交流群。
</p>
