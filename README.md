# ChatCut Online

ChatCut Online 是一款以真实多轨时间线为核心的 AI 视频编辑客户端。你可以像使用传统剪辑软件一样手动调整素材，也可以直接告诉 Agent 想怎么剪；工程、导入素材、生成结果和导出文件默认保存在本机。

> ChatCut Online 正在持续迭代。功能、模型、套餐和积分消耗以客户端及服务端实时显示为准。

[下载最新版](https://github.com/chaoshidai/ChatCut-Online/releases/latest) · [查看全部文档](docs/README.md) · [提交问题](https://github.com/chaoshidai/ChatCut-Online/issues/new/choose)

## 主要能力

| 能力 | 说明 | 是否需要联网 |
| --- | --- | --- |
| 本地工程 | 创建、复制、导入和继续编辑多个视频工程 | 否 |
| 多轨时间线 | 视频、音频、字幕、图片与图形元素均可继续手动调整 | 否 |
| AI Agent | 用自然语言执行剪辑操作，修改落到真实时间线上 | 是 |
| AI 素材生成 | 生成图片、视频、语音、音乐和音效，并下载到本地工程 | 是 |
| 本地处理 | 场景检测、自动调色、人声分离、素材规范化等 | 视功能而定 |
| 本地导出 | 视频、音频、字幕、FCPXML 和工程数据等 | 否 |

ChatCut Online 的平台模型由服务端统一提供，普通用户不需要配置模型厂商、服务地址或 API Key。使用 Agent 和 AI 生成前需要登录；收费操作会先展示积分报价，只有确认后才会创建云端任务。

## 三分钟开始

1. 从 [Releases](https://github.com/chaoshidai/ChatCut-Online/releases/latest) 下载与你的系统匹配、由本仓库发布的安装包。
2. 安装并启动 ChatCut Online，新建一个工程。
3. 把视频、音频或图片导入素材库，再拖到时间线。
4. 直接手动剪辑，或登录后在 Agent 面板输入：`把开头 3 秒删掉，并让剩余片段首尾衔接。`
5. 预览结果，确认时间线没有空隙、字幕遮挡或音量跳变。
6. 打开导出面板，选择格式、分辨率和保存位置后导出。

完整流程见[安装与首次启动](docs/01-installation.md)和[完成第一个视频工程](docs/02-first-project.md)。

## 当前版本边界

首个 Electron 版本已支持本地剪辑、平台 Agent，以及图片、视频、语音、音乐和音效生成。以下能力暂未开放：

- 云端自动转写和基于文字稿的剪辑；
- 素材站搜索；
- Agent 网页提取和远程代码沙箱；
- 图片、视频、音频生成的参考素材模式。

界面若显示“将在后续版本开放”，不需要配置第三方 Key；请等待正式更新。详情见[已知限制](docs/10-known-limitations.md)。

## 数据与付费原则

- 本地编辑与导出不依赖登录；离线时已有本地工程仍可编辑和导出。
- 工程、导入素材、自动下载的生成结果和导出文件保存在本机。
- Agent 与生成服务需要联网和登录，可能消耗积分。
- 每次生成前会展示模型、参数和积分报价，确认后才提交任务。
- 请求一旦进入生产队列，中途停止等待通常不代表自动退款；最终以服务端账单和正式付费规则为准。
- 购买套餐、退款或退出账号不会主动删除本地工程和已下载文件。

阅读[账号、套餐与积分](docs/07-account-and-points.md)和[本地数据与隐私](docs/08-local-data-and-privacy.md)了解详情。

## 文档目录

- [安装与首次启动](docs/01-installation.md)
- [完成第一个视频工程](docs/02-first-project.md)
- [时间线编辑基础](docs/03-timeline-basics.md)
- [使用 AI Agent 剪辑](docs/04-ai-agent.md)
- [生成图片、视频、语音、音乐和音效](docs/05-ai-generation.md)
- [导出与交付](docs/06-export.md)
- [账号、套餐与积分](docs/07-account-and-points.md)
- [本地数据与隐私](docs/08-local-data-and-privacy.md)
- [故障排查](docs/09-troubleshooting.md)
- [已知限制](docs/10-known-limitations.md)
- [常见问题](docs/11-faq.md)

## 获取帮助

先查看[故障排查](docs/09-troubleshooting.md)。仍无法解决时，请使用对应的 [Issue 模板](https://github.com/chaoshidai/ChatCut-Online/issues/new/choose)提交问题，并附上客户端版本、系统版本、复现步骤和脱敏诊断包。

请勿在公开 Issue 中粘贴手机号、支付凭据、登录二维码、访问令牌、完整本地路径或未打码的个人信息。

## 关于本仓库

本仓库用于发布 ChatCut Online 安装包、使用文档、教程和公开问题跟踪，不代表客户端或服务端源代码已在此开源。文档改进请参阅[贡献指南](CONTRIBUTING.md)。
