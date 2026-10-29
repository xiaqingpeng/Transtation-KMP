下面是在保留原有项目信息和技术特点的基础上，对 Transtation 项目介绍进行整理优化后的版本。主要优化了标题层级、功能分类、技术栈描述和 Markdown 格式，适合放在 GitHub README 中。

# Transtation

Transtation 是一款面向中文用户的跨平台翻译工具，名称由 **Translate（翻译）** 和 **Station（站点/平台）** 组合而成。项目采用 **Kotlin Multiplatform（KMP）** 和 **Compose Multiplatform** 构建，支持 Android 和基于 JVM 的桌面平台，致力于提供高效、灵活且可扩展的翻译体验。

## ✨ 核心功能

- **多引擎翻译**：支持同时调用多个翻译引擎进行翻译，包括必应、谷歌、百度、腾讯等。
- **大语言模型翻译**：支持接入 ChatGPT、GPT-4、ChatGLM、通义千问等多种大语言模型（LLM）。
- **对话式翻译**：支持通过与大语言模型进行多轮对话完成翻译。
- **长文本翻译**：利用大语言模型处理超长文本，满足复杂文本翻译需求。
- **插件系统**：支持插件开发、下载、更新、导入和导出，具备良好的可扩展性。
- **图片翻译**：支持识别并翻译图片中的文本，并提供多种翻译引擎选择。
- **屏幕翻译**：支持悬浮窗翻译、区域截图翻译和全屏截图翻译等模式。
- **个性化配置**：支持自定义主题、应用语言、翻译引擎等设置。

> 受开发时间限制，部分功能尚未在桌面端实现，后续将逐步完善。

## 📖 项目简介

Transtation 不仅是一款实用的翻译工具，也是一个面向 Android、Kotlin Multiplatform 和 Compose Multiplatform 开发者的开源学习项目。

本项目是 [FunnySaltyFish/Transtation](https://github.com/FunnySaltyFish/FunnyTranslation) 的 Kotlin Multiplatform 版本。原版 Android 应用已持续维护四年，为本项目提供了成熟的功能基础。

### 技术特点

- **跨平台开发**：采用 Kotlin Multiplatform + Compose Multiplatform，实现 Android 与 JVM 桌面端的跨平台开发。
- **现代化技术栈**：使用 MVVM 架构、Kotlin Coroutines、Flow 和 SQLDelight，构建清晰、可维护的应用结构。
- **多模块架构**：将通用模块（Common Module）与业务模块分离，提高代码复用率和模块独立性。
- **多引擎扩展机制**：支持多种翻译引擎并行工作，并提供插件开发、下载、更新、导入和导出能力。
- **丰富的 Kotlin 语言特性**：充分运用 Lazy Loading、类委托、协程、Flow、密封类（Sealed Classes）、扩展函数、扩展属性及反射等特性。
- **JavaScript 插件运行环境**：基于 Rhino JavaScript 引擎，设计并实现完整的 JavaScript 插件加载、运行与调试环境，为插件开发提供一站式支持。
- **Android 系统适配**：适配 Android 11 文件访问权限要求，并逐步支持 Android 13 的相关特性。
- **多语言与多形态 UI**：支持双语界面、深色模式，以及横屏和平板布局。
- **动态主题图标**：支持 Monet 动态图标等 Android 个性化特性。

此外，项目还开发并开源了四个相关库，进一步完善了项目的技术生态。

## 📥 下载与使用

项目支持 Android 和 Windows 平台，可通过以下渠道获取最新版本：

- **官方网站（中文）**：[Transtation 官方网站](https://www.funnysaltyfish.fun/trans)
- **GitHub Releases**：[下载最新版本](https://github.com/FunnySaltyFish/Transtation-KMP/releases)


## 🛠️ 源码阅读指南

如果你希望通过源码学习 Kotlin Multiplatform、Compose Multiplatform 或现代 Android 应用架构，建议从以下入口开始：

1. **主 Activity**：[`TransActivity.android.kt`](https://github.com/FunnySaltyFish/Transtation-KMP/blob/main/composeApp/src/androidMain/kotlin/com/funny/translation/translate/TransActivity.android.kt)，了解 Android 平台入口及初始化流程。
2. **应用导航**：[`AppNavigation.kt`](https://github.com/FunnySaltyFish/Transtation-KMP/blob/main/composeApp/src/commonMain/kotlin/com/funny/translation/translate/AppNavigation.kt)，了解跨平台 UI 组织与页面导航结构。

建议结合 `commonMain`、`androidMain` 等源码目录，进一步理解 KMP 的共享代码组织方式，以及公共业务逻辑与平台相关实现之间的协作机制。

## 📸 项目截图

### 屏幕录制

**v2.8.0 · 2024-01-15**

[查看项目演示视频](https://github.com/FunnySaltyFish/Transtation-KMP/assets/46063434/ded5d1c6-553c-4f45-96a4-74d870fcbcb8)

### Android 版本

**UI v4**

| 截图 1 | 截图 2 | 截图 3 |
| ---- | ---- | ---- |
| <br> | <br> | <br> |
| <br> | <br> | <br> |
| <br> | <br> | <br> |

\<details>\
\<summary>旧版界面（UI v3）\</summary>

| 截图 1                                                          | 截图 2                                                          |
| ------------------------------------------------------------- | ------------------------------------------------------------- |
| \<img src="./screenshots/1.png" alt="旧版界面截图 1" width="320" /> | \<img src="./screenshots/2.png" alt="旧版界面截图 2" width="320" /> |
| \<img src="./screenshots/3.png" alt="旧版界面截图 3" width="320" /> | \<img src="./screenshots/4.png" alt="旧版界面截图 4" width="320" /> |

\</details>

### 桌面版本

桌面版仍在持续开发中，界面与交互设计后续可能会有较大调整。

| 桌面版截图 1                                                              | 桌面版截图 2                                                              |
| -------------------------------------------------------------------- | -------------------------------------------------------------------- |
| \<img src="./screenshots/desktop_1.png" alt="桌面版截图 1" width="400" /> | \<img src="./screenshots/desktop_2.png" alt="桌面版截图 2" width="400" /> |

## ⭐ 支持项目

如果 Transtation 对你有所帮助，欢迎前往 GitHub 为项目点亮一颗 **Star**，支持开源项目持续发展！



### 优化说明

- 保留原有内容：没有主动删除原有功能、技术栈、下载渠道和截图信息。
- 优化阅读体验：按功能介绍、技术特点、下载方式、源码入口和截图重新组织内容。
- 突出 KMP 技术价值：重点呈现跨平台架构、多模块设计、JavaScript 插件系统及公共代码复用思路。
- 规范 Markdown：修复原文中重复加粗、转义符和链接格式问题，便于直接用于 GitHub README。

注意： 原文中的 GPT-4、Android 13 适配情况、桌面端功能完整度及版本信息属于原始介绍内容，并不代表已经核实的当前状态。若用于项目主页，建议后续结合仓库实际代码与最新 Release 再确认一次。