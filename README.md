⚠️ Disclaimer: This repository contains very old code from my early Unity learning days.
It is messy, experimental, and absolutely not suitable for any real project.

This project — MyFramework (Digital Twin / Dispose) — was one of my personal playgrounds when I first started learning Unity and programming. The code style reflects a true beginner: inconsistent structure, unclear architecture, duplicated logic, and many "please don't ask why" moments.

I uploaded it from an old USB drive about two years ago just to keep a record of my learning journey.

Please do NOT use this code in production (or anywhere else, really).

It exists purely as a nostalgic snapshot of how I used to write code — nothing more.

If you browse this repository, enjoy the chaos… but you’ve been warned. 😄



⚠️ 声明：这个仓库里的代码非常古老，是我刚接触 Unity 时写的练手作品。
代码结构混乱、风格稚嫩，仅作为学习记录保存，不适合任何实际项目使用。

这个项目 —— MyFramework（数字孪生 / dispose） —— 是我当初学习 Unity 时的个人玩具。
代码中充满了新手时期的写法：架构不清晰、逻辑重复、命名随意，还有许多“不要问我当时为什么这么写”的片段。

大约两年前，我从一个老 U 盘里把它整理上传，只是为了留个纪念。

请不要在任何正式项目中使用本代码（甚至最好别参考）。

它纯粹是我学习历程中的一个快照，仅作回顾与存档用途。

如果你坚持浏览它，请享受这份混乱，但——提前提醒你了。😄


# MyFramework

MyFramework 是一个为 Unity 开发的数字孪生工具框架，旨在简化和加速数字孪生应用的开发。该框架提供了一系列模块化的工具和管理器，帮助开发者更高效地构建复杂的应用程序。

## 📦 模块概览

- **EventCenter**: 事件中心，用于事件的注册和分发，简化事件驱动的开发。
- **Extension**: 扩展方法集合，提供了对 Unity 常用功能的扩展。
- **SoundManager**: 音频管理器，负责音效和背景音乐的播放与管理。
- **UIFrame**: UI 框架，提供了 UI 组件的管理和切换功能。
- **Utilities**: 实用工具集合，包含常用的辅助功能和工具类。
- **AnimatorManager**: 动画管理器，简化动画的控制和状态管理。
- **APIRequest**: API 请求模块，处理网络请求和数据解析。
- **CameraFrame**: 相机框架，提供相机的控制和管理功能。
- **Configuration**: 配置管理模块，处理应用程序的配置项。

## 🚀 快速开始

### 安装

1. 克隆或下载此仓库到你的 Unity 项目中。
2. 将 `MyFramework` 文件夹放置在你的 Unity 项目的 `Assets` 目录下。

### 使用

1. **事件中心**

   ```csharp
   EventCenter.Instance.RegisterEvent("OnPlayerDeath", OnPlayerDeathHandler);
   EventCenter.Instance.TriggerEvent("OnPlayerDeath", playerId);
   ```

2. **音频管理**

   ```csharp
   SoundManager.Instance.PlaySound("Explosion");
   SoundManager.Instance.PlayBackgroundMusic("MainTheme");
   ```

3. **UI 管理**

   ```csharp
   UIFrame.Instance.ShowPanel("MainMenu");
   UIFrame.Instance.HidePanel("Settings");
   ```

4. **API 请求**

   ```csharp
   APIRequest.Instance.Get("https://api.example.com/data", OnDataReceived);
   ```

## 📄 许可证

此项目基于 MIT 许可证开源。详情请参阅 [LICENSE](https://github.com/AkaJameson/MyFramework/blob/main/LICENSE)。
