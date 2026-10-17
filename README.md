# 智能步数管理（HyperOS）

<p align="center">
  <strong>面向 Xiaomi HyperOS 的步数管理 KernelSU / Magisk 模块</strong><br>
  提供 WebUI 操作面板、运行控制、基础配置与版本更新检查。
</p>

<p align="center">
  <a href="https://github.com/xiaoji0308/Steps/releases">下载模块</a> ·
  <a href="https://t.me/Stepsxxx">Telegram 交流群</a> ·
  <a href="https://www.coolapk.com/u/1547334">酷安主页</a>
</p>

---

## 项目简介

**智能步数管理**（模块 ID：`S-T-E-P-S`）是一个用于 Xiaomi HyperOS 环境的 KernelSU / Magisk 模块。模块通过 WebUI 提供可视化控制入口，方便用户启动或停止步数管理任务、刷新运行状态并调整基础运行配置。

> 本项目面向有模块安装和管理经验的用户。不同系统版本、Root 方案和应用环境可能影响实际表现，请以自己设备上的测试结果为准。

## 功能特性

- **WebUI 可视化面板**：通过网页面板管理模块，不必每次都手动执行命令。
- **运行控制**：支持开始运行、停止计步任务、重启相关进程和刷新状态。
- **基础配置**：可在面板中调整支持的运行选项，例如午夜自动重新运行、是否保留运行日志及相关时间间隔设置。
- **版本更新提示**：WebUI 提供更新检查入口与 Release 页面入口；是否能检查成功取决于设备网络及 GitHub 发布信息。
- **适配移动端**：面板采用卡片式布局，便于在手机屏幕上操作。
- **独立运行**：更新检查失败时，不应影响模块原有的运行控制功能。

## 安装方式

1. 在本仓库的 [Releases 页面](https://github.com/xiaoji0308/Steps/releases) 下载模块 ZIP。
2. 打开设备上已安装的 KernelSU 或 Magisk 管理器。
3. 从本地选择下载的 ZIP 并安装。
4. 按安装器提示完成重启（如果需要）。
5. 在模块详情中打开 WebUI，检查运行状态并按需调整配置。

**建议：** 安装或更新前保留当前可用安装包；首次使用时先确认模块状态正常，再启用自动运行等选项。

## 使用说明

在 WebUI 中可以根据页面提供的按钮和选项操作：

| 页面功能 | 说明 |
| --- | --- |
| 开始运行 | 启动步数管理任务 |
| 停止计步 | 停止当前计步任务 |
| 重启进程 | 重启模块相关进程 |
| 刷新状态 | 重新读取并显示当前运行状态 |
| 24 点后自动重新运行 | 控制是否在午夜后自动重新运行 |
| 保留运行日志 | 控制是否保留模块运行日志 |
| 检查更新 | 查询仓库发布信息并提示可能的新版本 |
| 查看发布页 | 打开 GitHub Releases 页面 |

不同版本的 WebUI 选项可能有所调整，请以实际安装版本显示为准。

## 下载与版本更新

- **最新正式安装包：** [GitHub Releases](https://github.com/xiaoji0308/Steps/releases)
- **更新信息接口：** [GitHub Latest Release API](https://api.github.com/repos/xiaoji0308/Steps/releases/latest)

发布新版本时，维护者应创建 GitHub Release，并附上可直接安装的模块 ZIP。版本号、标签和更新检查逻辑应保持一致；仅修改仓库中的文件，不会自动更新已经安装在设备上的模块。

如果 WebUI 显示发现新版本，通常还需要下载新 ZIP 并通过 KernelSU / Magisk 安装，才会真正更新本地模块。更新检查不等于自动安装。

## 常见问题

### 更新检查失败怎么办？

1. 确认设备网络能够访问 GitHub。
2. 打开 [Releases 页面](https://github.com/xiaoji0308/Steps/releases)，确认已发布正式 Release，并且 Release 附有 ZIP 安装包。
3. 确认本地版本与 Release 使用的版本标识遵循项目当前的版本规则。
4. 如果仍然失败，可以先从 Releases 手动下载并安装模块；检查失败不应影响原有运行功能。

### 安装后 WebUI 没有变化？

- 确认安装的是刚下载的 ZIP，而不是旧版本安装包。
- 在 KernelSU / Magisk 中确认模块已启用。
- 重新打开 WebUI；如果仍显示旧内容，请尝试关闭页面后重新进入，必要时重启设备。
- 提交问题时，请附上模块版本、系统版本、Root 方案和相关截图，避免分享设备敏感信息。

## 交流与反馈

- **Telegram 交流群：** [https://t.me/Stepsxxx](https://t.me/Stepsxxx)
- **酷安主页：** [https://www.coolapk.com/u/1547334](https://www.coolapk.com/u/1547334)
- **GitHub Issues：** [提交问题或建议](https://github.com/xiaoji0308/Steps/issues)

反馈问题时，建议说明设备型号、HyperOS 版本、KernelSU / Magisk 版本、模块版本、复现步骤和错误截图。请勿公开发布账号密码、设备标识等敏感信息。

## 免责声明

本项目按现状提供。请自行评估在设备上安装和使用模块的风险，并在更新前做好备份。因设备环境差异、第三方应用或系统更新造成的问题，请结合实际情况排查。

---

<p align="center">
  如果这个项目对你有帮助，欢迎关注仓库、提交反馈或加入交流群。
</p>
