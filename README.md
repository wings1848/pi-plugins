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

合集包内所有插件依赖声明为 `*`（永远拉最新版），
`pi update --all` 或重装合集包都会自动跟随各插件最新版本。

## 说明

- **版本策略**：全部依赖声明为 `*`（跟随最新）。插件发新版后无需等合集包发版，安装/更新即自动拉取
- ⚠️ **风险提示**：`*` 会直接跟随最新版，若上游插件出现破坏性变更可能导致不兼容。遇到问题可临时改回精确版本：`git clone` 后编辑 `package.json` 中的版本号再安装
- 模型凭证（API key 等）请在各设备自行配置，插件不涉及
- computer-use-linux 首次使用时自动下载二进制（约 7.5MB）

## License

MIT
