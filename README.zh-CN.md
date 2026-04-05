# Socratic Discovery Skills

[English](./README.md)

Socratic Discovery 是一组用于“苏格拉底式探索”的双语 skill。它的目标不是替用户给答案，而是让助手一次只问一个真正值得思考的问题，陪用户自己把路走出来。

这个仓库目前包含两个版本：

- `socratic-discovery-en`：英文优先版
- `socratic-discovery-zh`：中文优先版

它们都适合帮助用户探索：

- 一时还说不清楚的困惑
- 自己没意识到的盲区和隐藏假设
- “不知道自己不知道”的部分
- 通过自己思考获得的更深理解

## 适用场景

这两个 skill 适合在 Codex、Claude Code 这类支持本地 skill 的助手环境中使用，尤其适合下面这些情况：

- 用户想拆开一个模糊但重要的话题
- 用户更想被引导思考，而不是直接被告知答案
- 用户希望增强独立思考，而不是只拿结论
- 用户正在处理技术、策略、反思或开放性议题

## Skill 会做什么

每个版本都会把助手切换成一个耐心的“赛博苏格拉底”，它会：

- 先收集用户当前的基线理解
- 初始化后一次只问一个真正的问题
- 根据用户回答动态调整难度
- 留意思维模式、盲区和隐藏假设
- 在收束阶段把总结权交还给用户

## 选择哪个版本

如果你希望整段对话默认使用英文，使用 [socratic-discovery-en/SKILL.md](./socratic-discovery-en/SKILL.md)。

如果你希望整段对话默认使用中文，使用 [socratic-discovery-zh/SKILL.md](./socratic-discovery-zh/SKILL.md)。

## 从仓库安装

1. 直接在浏览器打开这个仓库，或者把仓库 clone 到本地。
2. 选择你要使用的 skill 文件夹：
   `socratic-discovery-en` 或 `socratic-discovery-zh`
3. 把这个文件夹放进你当前助手环境所使用的本地 skills 目录。
4. 如果你的环境不会自动刷新本地 skills，就重启或重新加载一次。

你也可以把两个文件夹都放进去，使用时按语言选择。

## 在 Codex 中使用

当 skill 文件夹已经能被你的本地 skills 库读取之后，可以直接这样调用：

- `Use $socratic-discovery-en to help me think through something I do not understand yet by asking one question at a time.`
- `Use $socratic-discovery-zh to guide me in Chinese through a topic I do not fully understand yet, one question at a time.`

## 在 Claude Code 中使用

如果你的 Claude Code 工作流支持本地可复用的 skill 或类似 prompt-pack 的目录结构，把选中的 skill 文件夹加入那套本地库里，然后同样按名字调用：

- `Use $socratic-discovery-en ...`
- `Use $socratic-discovery-zh ...`

关键不在于某个固定路径，而在于这个 skill 文件夹已经被你的助手环境识别为本地可复用 skill。

## 仓库结构

- [socratic-discovery-en/SKILL.md](./socratic-discovery-en/SKILL.md)
- [socratic-discovery-en/agents/openai.yaml](./socratic-discovery-en/agents/openai.yaml)
- [socratic-discovery-zh/SKILL.md](./socratic-discovery-zh/SKILL.md)
- [socratic-discovery-zh/agents/openai.yaml](./socratic-discovery-zh/agents/openai.yaml)
