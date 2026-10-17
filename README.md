# 智能步数管理（HyperOS）

<p align="center">
  <strong>为 Xiaomi HyperOS 打造的步数管理模块</strong><br>
  通过 KernelSU / Magisk 与手机端 WebUI，方便地控制步数任务、调整运行配置并查看更新信息。
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

**智能步数管理**（模块 ID：`S-T-E-P-S`）是面向 Xiaomi HyperOS 环境的 KernelSU / Magisk 模块。模块提供手机端 WebUI 控制面板，用于启动或停止步数管理任务、重启相关进程、刷新运行状态，以及调整页面提供的基础配置。

不同设备、HyperOS 版本及 Root 环境可能影响模块表现。以下说明以当前 WebUI 提供的功能为准；如果后续版本调整了界面或选项，请以实际安装版本为准。

## ✨ 功能详细介绍

### 🎛️ 1. 运行控制

- **开始运行**：启动模块的步数管理任务。
- **停止计步**：停止当前正在运行的计步任务。
- **重启进程**：重新启动模块相关进程，适用于任务状态异常时尝试恢复。
- **刷新状态**：重新读取当前运行状态，查看操作后的状态变化。

> 提示：如果操作后状态没有变化，可以先点击「刷新状态」；仍未恢复时，再尝试「重启进程」，并查看运行日志辅助排查。

### ⚙️ 2. 基础配置

- **24 点后自动重新运行**：控制是否启用午夜后自动重新运行的行为。
- **保留运行日志**：控制是否保留运行日志，方便查看和排查运行问题。
- **运行间隔等参数**：对于 WebUI 中提供的时间或间隔选项，可按自己的使用需求调整；请以当前版本页面显示的参数名称和单位为准。

修改配置后，请留意页面提示，确认操作是否保存成功。不同参数可能影响任务的运行行为，建议先使用默认值，了解效果后再调整。

### 📋 3. 运行日志

- 通过 WebUI 底部的「运行日志」入口查看模块提供的运行记录（如果当前版本启用了该页面）。
- 日志可用于辅助判断任务是否启动、操作是否执行，以及发生异常时的排查方向。
- 如果需要向开发者反馈问题，建议附上相关时间段的错误信息；分享前请检查并遮盖可能涉及个人隐私的内容。

### 🔔 4. 版本更新

- **当前版本**：显示本机安装模块的版本信息。
- **检查更新**：查询 GitHub Release 信息，并提示是否发现新版本。
- **查看发布页**：跳转到 GitHub Releases，查看版本说明和安装包。
- **更新状态提示**：显示检查结果；如果网络或仓库发布信息读取失败，可稍后重试或手动前往发布页。

**重要：检查更新不等于自动安装。** 发现新版本后，需要从 Release 下载可安装的 ZIP，并通过 KernelSU / Magisk 安装，才能更新设备上的模块。

### 💬 5. 交流与链接

- **打开 Telegram 群组**：跳转到项目交流群。
- **复制群组链接**：复制群组地址，方便分享给其他用户。
- **酷安主页**：访问作者的酷安主页，关注项目相关动态。

### 📱 6. 移动端界面

- 卡片式布局，适配手机屏幕。
- 将运行控制、群组入口、版本更新和基础配置分区展示。
- 底部导航用于在 WebUI 页面之间切换（以当前版本实际显示为准）。

## 📦 下载与安装

1. 打开 **[GitHub Releases 下载页](https://github.com/xiaoji0308/Steps/releases)**。
2. 下载对应版本的模块 ZIP 安装包。
3. 打开设备上的 KernelSU 或 Magisk 管理器，选择从本地安装 ZIP。
4. 按安装器提示完成操作；如果安装器要求重启，请重启设备。
5. 安装完成后打开模块 WebUI，确认运行状态正常，再按需调整配置。

**更新前建议：** 保留当前可用的安装包，并阅读对应 Release 的更新说明。请下载 Release 附件中的可安装 ZIP，不要将 GitHub 的源码压缩包误当作模块安装包。

## 🔄 版本发布与更新说明

- **模块下载：** [GitHub Releases](https://github.com/xiaoji0308/Steps/releases)
- **最新 Release 信息：** [GitHub API](https://api.github.com/repos/xiaoji0308/Steps/releases/latest)

维护者发布新版本时，应创建 GitHub Release 并附上可安装的模块 ZIP。Release 标签、模块 `module.prop` 中的版本信息和 WebUI 的版本比较规则应保持一致。

如果 WebUI 提示发现新版本，但版本号看起来相同，请检查 Release 标签及项目使用的版本比较规则是否一致。只修改仓库文件不会自动更新已经安装在设备上的模块。

## ❓ 常见问题

### 更新检查失败

1. 检查设备网络是否能够访问 GitHub。
2. 确认仓库已发布 Release，而不只是提交了代码或上传了普通文件。
3. 确认 Release 附件中包含可安装的模块 ZIP。
4. 如果暂时无法检查更新，可先从 [Releases 页面](https://github.com/xiaoji0308/Steps/releases) 手动下载并安装。

### 安装后页面仍显示旧内容

- 确认安装的是最新下载的 ZIP，而不是之前保存的旧包。
- 在 KernelSU / Magisk 中确认模块已启用。
- 关闭 WebUI 后重新打开；必要时重启设备。
- 如果问题仍然存在，反馈时请附上模块版本、系统版本、Root 方案和错误截图。

### 操作后任务状态不符合预期

- 先点「刷新状态」查看最新状态。
- 必要时尝试「重启进程」。
- 查看运行日志（如果当前版本提供）并记录复现步骤。
- 不确定参数作用时，先恢复默认值，再逐项调整。

## 💬 交流与反馈

欢迎加入交流群、关注酷安主页，或通过 GitHub 提交问题与建议。

- ✈️ **Telegram 交流群：** [https://t.me/Stepsxxx](https://t.me/Stepsxxx)
- 📱 **酷安个人主页：** [https://www.coolapk.com/u/1547334](https://www.coolapk.com/u/1547334)
- 🐛 **GitHub Issues：** [提交问题 / 建议](https://github.com/xiaoji0308/Steps/issues)
- 📥 **GitHub Releases：** [下载模块 / 查看更新](https://github.com/xiaoji0308/Steps/releases)

反馈问题时，建议描述设备型号、HyperOS 版本、KernelSU / Magisk 版本、模块版本、复现步骤和相关截图。请勿公开账号密码或其他敏感信息。

## ⚠️ 免责声明

本项目按现状提供。不同设备、系统版本、Root 方案及第三方应用环境可能影响模块行为。请自行评估使用风险，并在更新前做好必要备份。

---

<p align="center">
  如果这个项目对你有帮助，欢迎点亮 ⭐、提交反馈，或加入 Telegram 交流群。
</p>
