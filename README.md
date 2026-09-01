# pi-plugins

wings1848 的 pi coding agent 插件合集包。

一条命令安装 **14 个精选插件**（扩展、技能、提示词模板一次全齐）。

## 安装

```bash
pi install git:https://github.com/wings1848/pi-plugins.git
```

安装后运行 `/reload` 或重启 pi 即可生效。

## 包含的插件

| 插件 | 用途 |
| --- | --- |
| pi-subagents | 子代理工作流（council-mode 等） |
| pi-mcp-adapter | MCP 服务器适配（可接入任意 MCP 工具） |
| pi-tool-display | 工具展示优化 |
| pi-rtk-optimizer | RTK 上下文优化 |
| pi-image-tools | 图片处理工具 |
| pi-cache-optimizer | 缓存优化 |
| @vndv/pi-codegraph | CodeGraph 代码索引 |
| @juicesharp/rpiv-todo | 任务清单 |
| @juicesharp/rpiv-ask-user-question | 结构化提问 |
| @juicesharp/rpiv-web-tools | 网页搜索/抓取 |
| @llblab/pi-telegram | Telegram 桥接 |
| @wingsbutterfly/pi-zh | 中文回复风格 |
| @agent-sh/computer-use-linux | Linux 桌面自动化（隐藏工作区） |
| pi-config-sync | 多设备配置同步（可选，按需初始化） |

## 更新

```bash
pi update --all
```

合集包更新后会拉取各插件最新版本。

## 说明

- 版本以合集包声明为准（精确锁定），更新依赖合集包发布新版本
- 模型凭证（API key 等）请在各设备自行配置，插件不涉及
- computer-use-linux 首次使用时自动下载二进制（约 7.5MB）

## License

MIT
