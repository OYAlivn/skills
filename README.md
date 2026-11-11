# skills — Agent Skill 集合

个人构建的 AI Agent Skills。每个子目录是一个独立 skill，可直接装进支持 skills 的 AI 工具（Claude Code / OpenCode / Cursor 等）。

## Skill 清单

| Skill | 干什么 | 详情 |
|---|---|---|
| [kos-starter](./kos-starter/) | 产品经理 AI 工作流 skill（公司场景版）：30 分钟搭出「让 AI 一开门就认识你和你的工作」的个人工作知识库，日常入库记账，四台阶升级到 AI 分身 | [说明文档](./kos-starter/README.md) · [配套方法论](./kos-starter/docs/) |

> 后续新 skill 将持续加入本仓库。

## 通用安装（任意 skill 通用）

1. `git clone https://github.com/OYAlivn/skills.git`（或网页 Code → Download ZIP 解压）
2. 把你想要的 skill 文件夹（如 `kos-starter/`）复制到你的 AI 工具 skills 目录：
   - Claude Code / OpenCode：`C:\Users\你的用户名\.claude\skills\`（macOS：`~/.claude/skills/`）
   - 其他工具：查其文档中「skills / 技能 / extensions」的安装位置
3. 重启工具、开新会话，问 AI「你现在有哪些 skill」验证

各 skill 的详细说明与场景用法见其目录内的 README（如 [kos-starter/README.md](./kos-starter/README.md)）。

## 安全一句话

库文件只存在你的电脑上；但 AI 读库时，内容会随会话发送给它背后的模型服务商——会话本身不保密。公司红线内容不入库、不进会话。

## License

MIT（见根 [LICENSE](./LICENSE)），各 skill 可自由使用与修改。
