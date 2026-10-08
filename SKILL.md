---
name: global-preferences
description: Maintain concise global personal preferences in ~/.config/opencode/AGENTS.md. Use when the user asks to remember a durable preference across projects, update global AGENTS.md, add a cross-project habit, or review personal agent instructions.
---

## 目标

只把**跨项目、长期、稳定**的个人偏好写入全局 `~/.config/opencode/AGENTS.md`。

不要写入：
- 某个项目专属的架构、命令、路径（放项目的 `AGENTS.md`）
- 一次性任务、临时决定、调试上下文
- 密钥、凭据、个人隐私
- 短时间会过期的模型/工具状态

## 工作流

1. 读当前全局 `AGENTS.md`，判断是否已存在同类规则。
2. 判断用户说的是否属于全局偏好；不确定时先问一句澄清。
3. 只提出最小修改：能追加就不重写；能合并就删除重复项。
4. 修改前说明要写在哪一行附近、为什么这是全局偏好。
5. 写入后简短告知改了什么。

## 写作标准

- 中文，先结论后理由。
- 具体可执行，例如“改完必须运行测试”，而不是“注意质量”。
- 保持短，每条尽量一句话。
- 同类内容合并到同一小节。
- 项目里已经说明的内容，不复制到全局。

## 示例

可以写：

> 改完代码必须实际运行测试；只讲思路不给结论时不算完成。

不要写：

> 项目 A 的 `pnpm dev` 命令见 `/path/to/project/AGENTS.md`。
