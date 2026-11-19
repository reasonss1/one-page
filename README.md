# 一页纸 · Agent Skill

**把零散材料整理成一页：结论是什么，依据是什么，下一步做什么。**

有 **27 张玩法卡**，按手头的任务选一张就能用。每张卡都有步骤、可复制的模板和原创示例，适用于工作、学习和日常生活。

## 一条命令安装到 Codex

电脑上有 Git 即可。在运行 Codex 的系统里打开终端（如果 Codex 跑在 WSL，就在对应的 WSL 里运行）：

```sh
git clone --depth 1 --branch v0.1.0 https://github.com/reasonss1/one-page.git "$HOME/.agents/skills/one-page"
```

这条命令安装固定版本 `v0.1.0`，不会覆盖已有的 `one-page` 目录。没有 Git 时，可以[下载 ZIP](https://github.com/reasonss1/one-page/archive/refs/tags/v0.1.0.zip)，解压后将含 `SKILL.md` 的文件夹命名为 `one-page`，放进 `$HOME/.agents/skills/`。

## 第一次怎么用？

开一个新会话，输入 `$one-page`，贴上材料，说明**写给谁、看完要做什么**。如果技能不在列表里，重启 Codex 后再试。

> 用 `$one-page` 把下面的讨论整理成一页纪要，给没参会的同事看。先写结论，再分开已定、未定和下一步。没人确认的负责人和日期就标待确认。

也可以直接复制 [通用模板](assets/one-page-template.md) 自己填写。

## 你可以拿它做什么？

| 如果你想…… | 可以拿到…… |
|---|---|
| 理清一堆想法或待办 | [取舍清单](references/cards/foundations.md)：先列候选，再按目的筛选 |
| 让别人看懂汇报或旧资料 | [一页总览](references/cards/documents.md)：先给结论，再交代依据与待确认项 |
| 开会时不跑题，散会后能接着做 | [会议工作页](references/cards/meetings.md)：候选、已定、未定和下一步 |
| 安排工作、准备协商或反馈 | [计划与沟通页](references/cards/work.md)：标出负荷、固定期限和可商量的事项 |
| 定目标或做复盘 | [目标与复盘页](references/cards/goals.md)：说明取舍，再选一个能试的动作 |
| 把读到的东西用起来 | [学习与记录页](references/cards/learning.md)：区分材料、个人判断和动手试验 |

[查看全部 27 张玩法卡 →](references/playbook.md)

## 适用边界

「一页」是先做取舍，不是删掉影响判断的事实；确需打印成一张 A4 时，应以分页预览为准。这是独立工具，不代表任何组织的内部标准。

[技能入口](SKILL.md)
