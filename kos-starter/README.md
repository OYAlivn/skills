# kos-starter — 个人知识库起步引导 skill

> 配套《个人AI知识库搭建方案》使用。装好之后，对 AI 说一句「搭建知识库」，它会带你 30 分钟搭出一个「让 AI 一开门就认识你」的个人知识库，并在后续使用中帮你记账、提醒升级。

## 先读文档（人看），再装 skill（AI 用）

完整方法论见 [`docs/个人AI知识库搭建方案 - 从零到AI分身.md`](./docs/个人AI知识库搭建方案%20-%20从零到AI分身.md)：原理（输入=命令+上下文）、5 节点搭建流程、日常用法、30 分钟最小可行版、跨工具兼容说明。skill 是它的执行层——文档告诉你为什么，skill 带你做。

## 你需要先有

一台电脑 + 任意一个 AI 编码工具（能对话、能读写本地文件）：

| 工具 | 获取方式 | 特点 |
|---|---|---|
| OpenCode | 开源免费，GitHub 搜 opencode，按说明安装 | 免费全功能 |
| Cursor | 官网下载安装 | 图形界面，最好上手 |
| Claude Code | Anthropic 出品 | 需订阅 |

手机 / 平板暂不支持（skill 依赖读写本地文件的能力，先在电脑上搭）。

## 怎么装（2 分钟）

1. 获取 skill 文件夹（任选其一）：
   - 命令行：`git clone https://github.com/OYAlivn/skills.git`，取其中的 `kos-starter` 文件夹
   - 网页：GitHub 仓库页（OYAlivn/skills）Code → Download ZIP，解压后取 `kos-starter` 文件夹
2. 把整个 `kos-starter` 文件夹复制到你 AI 工具的 skills 目录：
   - Claude Code / OpenCode：`C:\Users\你的用户名\.claude\skills\`（macOS：`~/.claude/skills/`）
   - 其他工具：查其文档中「skills / 技能 / extensions」的安装位置，通常是类似的 skills 目录
3. 重启你的 AI 工具、开一个新会话（skills 在会话启动时加载）
4. 验证：问 AI「你现在有哪些 skill」，列表里出现 kos-starter 即成功

## 装完怎么说

| 你说 | 发生什么 |
|---|---|
| 「搭建知识库」（第一次） | AI 访谈你几个问题，30 分钟搭出最小版知识库 |
| 「记录这个」+ 内容（日常） | AI 先报「四选一」分诊再入库，自动登记索引 |
| 「升级知识库」（库变大后） | AI 按四台阶带你升级：五域结构 → Git 备份 → 对账体检 → AI 分身 |

## 不想装 skill？

把本仓库 `docs/` 里的《个人AI知识库搭建方案》直接发给任意 AI，说「照这个方案带我搭」——方案本身就够用，skill 只是让过程更省心。

## 隐私一句话

库文件只存在你的电脑上；但 AI 读库时，内容会随会话发送给它背后的模型服务商——会话本身不保密，证件、密码类信息不要入库。
