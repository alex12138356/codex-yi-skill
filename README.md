# Codex 壹 · 多线记忆系统（Codex Skill）

给 Codex 装上"外挂记忆"：7 个文件组成的多线协作系统，填一次背景，所有新对话自动知道你是谁。

Give your Codex persistent memory: a 7-file multi-thread collaboration system. Fill in your background once, and every new conversation automatically knows who you are.

## 解决什么 / What it solves

- 对话到 400 截断，上下文全丢 → SESSION_LOG 续传，新对话直接接上
- 每个新对话重新教一遍 → 共享知识库 + 启动指令，自动读取
- 多项目互相干扰 → 中枢调度 + 执行线隔离 + 回传日志

## 安装 / Install

\`\`\`bash
cp -r codex-yi-skill ~/.codex/skills/
\`\`\`

然后对 Codex 说："帮我搭多线协作系统，解决 400 截断丢上下文。"

## 文件结构 / Structure

- SKILL.md —— 触发条件与执行流程
- templates/ —— 7 个模板文件（含【占位符】，Skill 运行时按你的答案替换）
  - 共享知识库.md（桌面，所有对话共用）
  - 启动指令.txt（每个新对话粘贴一次）
  - 任务指南.md（给中枢调度对话）
  - SESSION_LOG.md（对话快满时续传状态）
  - 回传日志.md（各线完成后回传）
  - 项目管理模板.md（中枢维护进度）
  - 协作协议.md（各线协作规范）

## 免费与付费 / Free & Paid

- 在线生成器（免费，无需安装 Skill）：https://codex-yi.com
- ¥39.9 付费代搭：填背景 → 帮你生成+部署整套系统+使用指导（站内扫码加微信）
- 企业/团队定制：站内联系

## 作者 / Author

深圳佳景程科技 · https://jiajingcheng.com
GitHub: https://github.com/alex12138356/codex-yi

