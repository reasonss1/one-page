# 一页纸 · Agent Skill

**给 AI 的汇报 Skill：先说结果，别让人从一大段过程里找答案。**

AI 可以写很多，但人的注意力有限。一次交付、一次进度更新，甚至一句日常反馈，都应该先说清：**做成了什么，验证到哪一步，有没有需要我处理的事。** 与判断无关的过程留在后面，没验证的别写成已完成。

**一句能说清，就不要写一页。** 需要整理复杂材料时，再按场景选用 27 张玩法卡。

## 一条命令安装到 Codex

电脑上有 Git 即可。在运行 Codex 的系统里打开终端（如果 Codex 跑在 WSL，就在对应的 WSL 里运行）：

```sh
git clone --depth 1 --branch v0.1.1 https://github.com/reasonss1/one-page.git "$HOME/.agents/skills/one-page"
```

这条命令安装固定版本 `v0.1.1`，不会覆盖已有的 `one-page` 目录。没有 Git 或克隆超时时，可以[直接下载 ZIP](https://codeload.github.com/reasonss1/one-page/zip/refs/tags/v0.1.1)，解压后将含 `SKILL.md` 的文件夹命名为 `one-page`，放进 `$HOME/.agents/skills/`。

## 第一次怎么用？

开一个新会话，输入 `$one-page`，贴上材料，说明**写给谁、看完要做什么**。如果技能不在列表里，重启 Codex 后再试。

> 用 `$one-page` 汇报刚才做的事：先说结果，再说验证到哪、还有什么未确认。只有需要我行动或决定时，才写下一步。

一条日常反馈就可以是这样：「已整理会议纪要，三项决定已和参会人核对。场地还没确认，通知先不发。」

### 让它成为项目的默认汇报方式

想让 AI 在这个项目里优先这样汇报，可把下面这句加入项目的 `AGENTS.md`：

```markdown
AI 向人汇报进度、交付或日常结果时，优先使用 $one-page：第一句说结果，只保留影响判断的证据和未验证项；需要行动或拍板时才列下一步。一句够用就不写一页。
```

更复杂的汇报可从 [通用模板](assets/one-page-template.md) 开始。

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
