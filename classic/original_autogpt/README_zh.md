# AutoGPT：一个自主的GPT-4实验项目

[📖 **文档**][docs]
&ensp;|&ensp;
[🚀 **贡献指南**](../../CONTRIBUTING.md)

AutoGPT是一个展示现代大型语言模型能力的实验性开源应用。这个由GPT-4驱动的程序能够将LLM的"思考"串联起来，自主实现你设定的任何目标。作为首批完全自主运行的GPT-4示例之一，AutoGPT正在突破AI可能性的边界。

<h2 align="center"> 2023年4月16日演示 </h2>

https://user-images.githubusercontent.com/70048414/232352935-55c6bf7c-3958-406e-8610-0913475a0b05.mp4

演示由<a href=https://twitter.com/BlakeWerlinger>Blake Werlinger</a>制作

## 🚀 功能特性

- 🔌 代理协议([文档](https://agentprotocol.ai))
- 💻 易用的用户界面
- 🌐 支持互联网搜索和信息收集
- 🧠 由GPT-4和GPT-3.5 Turbo混合驱动
- 🔗 可访问热门网站和平台
- 🗃️ 文件生成和编辑能力
- 🔌 支持插件扩展
<!-- - 💾 长期和短期记忆管理 -->

## 设置AutoGPT
1. 获取OpenAI [API密钥](https://platform.openai.com/account/api-keys)
2. 复制`.env.template`为`.env`并设置`OPENAI_API_KEY`
3. 确保已安装Poetry[安装指南](https://python-poetry.org/docs/#installation)

更多运行AutoGPT的方式、详细说明和配置选项，请参阅[安装指南][docs/setup]。

## 运行AutoGPT
CLI应该是自解释的：
```shell
$ ./autogpt.sh --help
用法: python -m autogpt [选项] 命令 [参数]...
选项:
  --help  显示此帮助信息并退出。
命令:
  run    根据用户指定的任务设置并运行代理，或恢复现有代理...
  serve  启动符合Agent协议的AutoGPT服务器，该服务器为每个任务...
```
当不带子命令运行时，出于兼容性考虑会默认使用`run`命令。

<details>
<summary>
<code>$ ./autogpt.sh run --help</code>
</summary>

`run`子命令以传统CLI界面启动AutoGPT：

```shell
$ ./autogpt.sh run --help
用法: python -m autogpt run [选项]
  根据用户指定的任务设置并运行代理，或恢复现有代理。
选项:
  -c, --continuous                启用连续模式
  -y, --skip-reprompt             跳过脚本开始时的重新提示消息
  -l, --continuous-limit INTEGER  定义连续模式下的运行次数
  --speak                         启用语音模式
  --debug                         启用调试模式
  --skip-news                     指定是否在启动时禁止显示最新新闻
  --install-plugin-deps           安装第三方插件的外部依赖
  --ai-name TEXT                  覆盖AI名称
  --ai-role TEXT                  覆盖AI角色
  --constraint TEXT               添加或覆盖AI约束条件到提示中；可多次使用以传递多个约束
  --resource TEXT                 添加或覆盖AI资源到提示中；可多次使用以传递多个资源
  --best-practice TEXT            添加或覆盖AI最佳实践到提示中；可多次使用以传递多个最佳实践
  --override-directives           如果指定，--constraint、--resource和--best-practice将覆盖AI的指令而不是追加 
  --component-config-file TEXT    组件配置文件的json路径  
  --help                          显示此帮助信息并退出</details>
```
<details>
<summary>
<code>$ ./autogpt.sh serve --help</code>
</summary>

`serve`子命令以Agent协议服务器形式启动AutoGPT：

```shell
$ ./autogpt.sh serve --help用法: python -m autogpt serve [选项]  启动符合Agent协议的AutoGPT服务器，该服务器为每个任务创建自定义代理。选项:  --debug                     启用调试模式  --install-plugin-deps       安装第三方插件的外部依赖  --help                      显示此帮助信息并退出</details>
```
使用`serve`时，应用程序会暴露一个符合Agent协议的API并提供前端界面，默认在`http://localhost:8000`。

更全面的使用说明，请参阅[用户指南][docs/usage]。

[docs]: https://docs.agpt.co/autogpt
[docs/setup]: https://docs.agpt.co/classic/original_autogpt/setup
[docs/usage]: https://docs.agpt.co/classic/original_autogpt/usage
[docs/plugins]: https://docs.agpt.co/classic/original_autogpt/plugins

## 📚 资源
* 📔 AutoGPT [项目Wiki](https://github.com/Significant-Gravitas/AutoGPT/wiki)
* 🧮 AutoGPT [项目看板](https://github.com/orgs/Significant-Gravitas/projects/1)
* 🌃 AutoGPT [路线图](https://github.com/orgs/Significant-Gravitas/projects/2)

## ⚠️ 局限性

本实验旨在展示GPT-4的潜力，但存在一些限制：

1. 不是一个成熟的应用或产品，只是一个实验
2. 在复杂的现实商业场景中可能表现不佳。事实上，如果确实表现良好，请分享您的结果！
3. 运行成本相当高，请设置并监控您在OpenAI的API密钥限额！

## 🛡 免责声明

AutoGPT是一个实验性应用，按"原样"提供，不作任何明示或暗示的保证。使用本软件即表示您同意承担使用该软件的所有风险，包括但不限于数据丢失、系统故障或可能出现的任何其他问题。

本项目的开发者和贡献者不对因使用本软件而导致的任何损失、损害或其他后果承担任何责任或义务。您全权负责基于AutoGPT提供的信息做出的任何决定和采取的行动。

**请注意，使用GPT-4语言模型可能会因其token使用而产生高昂费用。** 使用本项目即表示您承认您有责任监控和管理自己的token使用及相关费用。强烈建议定期检查您的OpenAI API使用情况，并设置必要的限额或提醒以防止意外收费。

作为一个自主实验，AutoGPT可能会生成不符合现实商业实践或法律要求的内容或采取相应行动。您有责任确保基于本软件输出做出的任何行动或决定符合所有适用的法律、法规和道德标准。本项目的开发者和贡献者不对因使用本软件而产生的任何后果负责。

使用AutoGPT即表示您同意赔偿、辩护并使开发者、贡献者和任何关联方免受因您使用本软件或违反这些条款而产生的任何和所有索赔、损害、损失、责任、成本和费用(包括合理的律师费)的影响。

---

在2023年第二季度，AutoGPT成为历史上增长最快的开源项目。现在尘埃落定，我们致力于项目的可持续发展和持续增长。

<p align="center">
  <a href="https://star-history.com/#Significant-Gravitas/AutoGPT&Date">
    <img src="https://api.star-history.com/svg?repos=Significant-Gravitas/AutoGPT&type=Date" alt="Star History Chart">
  </a>
</p>

