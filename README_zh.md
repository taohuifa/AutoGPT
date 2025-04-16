# AutoGPT：构建、部署和运行AI智能体

[![Discord 关注](https://dcbadge.vercel.app/api/server/autogpt?style=flat)](https://discord.gg/autogpt) &ensp;
[![Twitter 关注](https://img.shields.io/twitter/follow/Auto_GPT?style=social)](https://twitter.com/Auto_GPT) &ensp;
[![许可证: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)

**AutoGPT** 是一个强大的平台，允许您创建、部署和管理自动化复杂工作流程的持续AI智能体。

## 托管选项
   - 下载自托管
   - [加入等待列表](https://bit.ly/3ZDijAI) 体验云端托管测试版

## 自托管设置指南
> [!注意]
> 设置和托管AutoGPT平台是一个技术性过程。
> 如果您想要开箱即用的解决方案，我们建议[加入等待列表](https://bit.ly/3ZDijAI)体验云端托管测试版。

### 最新设置说明：
我们已迁移至一个完全维护并定期更新的文档站点。

👉 [点击此处查看官方自托管指南](https://docs.agpt.co/platform/getting-started/)

本教程假设您已安装Docker、VSCode、git和npm。

### 🧱 AutoGPT前端

AutoGPT前端是用户与我们强大的AI自动化平台交互的地方。它提供了多种方式来利用我们的AI智能体。这是您将AI自动化想法变为现实的界面：

   **智能体构建器：** 通过直观的低代码界面设计和配置您自己的AI智能体。
   
   **工作流管理：** 轻松构建、修改和优化您的自动化工作流。通过连接模块来构建智能体，每个模块执行单一操作。
   
   **部署控制：** 管理智能体的生命周期，从测试到生产。
   
   **即用型智能体：** 不想自己构建？只需从我们的预配置智能体库中选择并立即投入使用。
   
   **智能体交互：** 无论是自建还是使用预配置智能体，都能通过用户友好界面轻松运行和交互。
   
   **监控与分析：** 跟踪智能体性能并获得洞察，持续改进自动化流程。

[阅读本指南](https://docs.agpt.co/platform/new_blocks/)了解如何构建自定义模块。

### 💽 AutoGPT服务器

AutoGPT服务器是我们平台的核心动力。这是您的智能体运行的地方。一旦部署，智能体可以被外部源触发并持续运行。它包含使AutoGPT平稳运行的所有基本组件。

   **源代码：** 驱动我们智能体和自动化流程的核心逻辑。
   
   **基础设施：** 确保可靠和可扩展性能的健壮系统。
   
   **市场：** 一个全面的市场，您可以找到并部署各种预构建智能体。

### 🐙 示例智能体

以下是您可以用AutoGPT实现的两个示例：

1. **根据热门话题生成病毒式视频**
   - 该智能体读取Reddit上的话题
   - 识别热门话题
   - 然后自动根据内容创建短视频

2. **从视频中识别社交媒体最佳引用**
   - 该智能体订阅您的YouTube频道
   - 当您发布新视频时，它会转录视频
   - 使用AI识别最具影响力的引用并生成摘要
   - 然后自动撰写帖子发布到您的社交媒体

这些示例只是AutoGPT功能的冰山一角！您可以创建定制工作流来构建适用于任何用例的智能体。

---
### 使命与许可
我们的使命是提供工具，让您专注于重要的事情：

- 🏗️ **构建** - 为伟大事物奠定基础
- 🧪 **测试** - 将智能体调整至完美
- 🤝 **委托** - 让AI为您工作，让想法变为现实

成为革命的一部分！**AutoGPT**将始终站在AI创新的前沿。

**📖 [文档](https://docs.agpt.co)**
&ensp;|&ensp;
**🚀 [贡献指南](CONTRIBUTING.md)**

**许可信息：**

MIT许可证：AutoGPT仓库的大部分内容使用MIT许可证。

Polyform Shield许可证：此许可证适用于autogpt_platform文件夹。

更多信息请见 https://agpt.co/blog/introducing-the-autogpt-platform

---
## 🤖 AutoGPT经典版
> 以下是关于AutoGPT经典版的信息。

**🛠️ [构建自己的智能体 - 快速入门](classic/FORGE-QUICKSTART.md)**

### 🏗️ Forge

**打造您自己的智能体！** &ndash; Forge是一个即用型工具包，用于构建自己的智能体应用程序。它处理大部分样板代码，让您将所有创造力集中在使您的智能体与众不同的地方。所有教程位于[此处](https://medium.com/@aiedge/autogpt-forge-e3de53cc58ec)。[`forge`](/classic/forge/)中的组件也可以单独使用，以加速开发并减少智能体项目中的样板代码。

🚀 [**Forge入门指南**](https://github.com/Significant-Gravitas/AutoGPT/blob/master/classic/forge/tutorials/001_getting_started.md) &ndash;
本指南将带您完成创建自己的智能体并使用基准测试和用户界面的过程。

📘 [了解更多](https://github.com/Significant-Gravitas/AutoGPT/tree/master/classic/forge)关于Forge的信息

### 🎯 基准测试

**测量智能体性能！** `agbenchmark`可用于任何支持智能体协议的智能体，与项目[CLI]的集成使其更易于与AutoGPT和基于forge的智能体一起使用。基准测试提供了一个严格的测试环境。我们的框架允许进行自主、客观的性能评估，确保您的智能体为现实行动做好准备。

📦 [Pypi上的`agbenchmark`](https://pypi.org/project/agbenchmark/)
&ensp;|&ensp;
📘 [了解更多](https://github.com/Significant-Gravitas/AutoGPT/tree/master/classic/benchmark)关于基准测试的信息

### 💻 用户界面

**使智能体易于使用！** `frontend`为您提供了一个用户友好的界面来控制和监控智能体。它通过[智能体协议](#-智能体协议)连接到智能体，确保与我们生态系统内外许多智能体的兼容性。

前端与仓库中的所有智能体开箱即用。只需使用[CLI]运行您选择的智能体！

📘 [了解更多](https://github.com/Significant-Gravitas/AutoGPT/tree/master/classic/frontend)关于前端的信息

### ⌨️ 命令行界面

[CLI]: #-命令行界面

为了使仓库提供的所有工具尽可能易于使用，仓库根目录包含一个CLI：

```shell
$ ./run
用法: cli.py [选项] 命令 [参数]...
选项:
  --help  显示此帮助信息并退出
命令:
  agent      创建、启动和停止智能体的命令
  benchmark  启动基准测试和列出测试及类别的命令
  setup      为您的系统安装所需依赖
```
只需克隆仓库，使用`./run setup`安装依赖项，您就可以开始了！

## 🤔 有问题？遇到问题？有建议？

### 获取帮助 - [Discord 💬](https://discord.gg/autogpt)

[![加入我们的Discord](https://invidget.switchblade.xyz/autogpt)](https://discord.gg/autogpt)

要报告错误或请求功能，请创建[GitHub Issue](https://github.com/Significant-Gravitas/AutoGPT/issues/new/choose)。请确保其他人没有为同一主题创建问题。

## 🤝 姊妹项目

### 🔄 智能体协议

为了保持统一标准并确保与许多当前和未来应用程序的无缝兼容性，AutoGPT采用AI工程师基金会的[智能体协议](https://agentprotocol.ai/)标准。这标准化了从您的智能体到前端和基准测试的通信路径。

---

## 星标统计

<p align="center">
<a href="https://star-history.com/#Significant-Gravitas/AutoGPT">
  <picture>
    <source media="(prefers-color-scheme: dark)" srcset="https://api.star-history.com/svg?repos=Significant-Gravitas/AutoGPT&type=Date&theme=dark" />
    <source media="(prefers-color-scheme: light)" srcset="https://api.star-history.com/svg?repos=Significant-Gravitas/AutoGPT&type=Date" />
    <img alt="星标历史图表" src="https://api.star-history.com/svg?repos=Significant-Gravitas/AutoGPT&type=Date" />
  </picture>
</a>
</p>

## ⚡ 贡献者

<a href="https://github.com/Significant-Gravitas/AutoGPT/graphs/contributors" alt="查看贡献者">
  <img src="https://contrib.rocks/image?repo=Significant-Gravitas/AutoGPT&max=1000&columns=10" alt="贡献者" />
</a>
