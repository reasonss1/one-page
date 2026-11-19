# 一页纸 · Agent Skill

**不是让 AI 少说几句，是让人不用读完几段，才知道事情到底怎样了。**

「一页纸」用在 AI 把结果交给人的那一刻。默认就在聊天里用文本或 Markdown 回答：一句能答清就直接答；有几件事要分清，再分行或列表。**给人看才用，Agent 之间仍按原格式交接。**

## 聊天里是什么样？

**你：README 改好了吗？我现在去 GitHub 能看到新版吗？**

绕着答：「我先调整了首页的例子，又检查了文档链接，本地修改已经完成，目前还没有推送到 GitHub。」

直接答：「**现在还看不到新版。** README 在本地改好了，链接也检查过了，但还没推送。」

**你：两张销售表合并了吗？周报能发给运营了吗？**

> 两张表合并了，**周报还不能发**：有两笔退款没对上原订单，净销售额还没核准。
>
> - **已核对：** 两张表里的销售记录都在合并表里。
> - **需要你补：** 把那两笔退款对应的原订单号发我，我才能核准净销售额。

## 一条命令安装到 Codex

电脑上有 Git 即可。在运行 Codex 的系统里打开终端（如果 Codex 跑在 WSL，就在对应的 WSL 里运行）：

```sh
git clone --depth 1 --branch v0.2.0 https://github.com/reasonss1/one-page.git "$HOME/.agents/skills/one-page"
```

这条命令安装固定版本 `v0.2.0`，不会覆盖已有的 `one-page` 目录。没有 Git 或克隆超时时，可以[直接下载 ZIP](https://codeload.github.com/reasonss1/one-page/zip/refs/tags/v0.2.0)，解压后将含 `SKILL.md` 的文件夹命名为 `one-page`，放进 `$HOME/.agents/skills/`。

## 装完试一次

打开新会话，复制下面这条。如果技能不在列表里，重启 Codex 后再试。

```text
用 $one-page 回答我：这份销售周报现在能发给运营吗？
已知：两张销售表已合并，销售记录已核对。还有两笔退款找不到原订单，净销售额未核准；原订单号需要我提供。
```

看答复，不看字数：第一眼能不能知道**还不能发**？能不能分清「表已合并」和「金额已核准」，知道自己该补什么？不必另开附件。

### 让它成为项目的默认汇报方式

想让 AI 在这个项目里优先这样汇报，可把下面这句加入项目的 `AGENTS.md`：

```markdown
AI 最后把结果交给人看时，优先使用 $one-page：先回答读者最关心的问题，把会改变判断的阻塞或未验证项放在结论旁。按场景使用可扫读的 Markdown 样式；简单反馈直接答。Agent 交接、工具调用和机器读取继续使用原有格式。
```

复杂的聊天回复可以从 [Markdown 模板](assets/one-page-template.md) 开始。

## 你可以拿它做什么？

| 如果你想…… | 可以拿到…… |
|---|---|
| 理清一堆想法或待办 | [取舍清单](references/cards/foundations.md)：先列候选，再按目的筛选 |
| 让别人看懂汇报或旧资料 | [一页总览](references/cards/documents.md)：先给结论，再交代依据与待确认项 |
| 开会时不跑题，散会后能接着做 | [会议工作页](references/cards/meetings.md)：候选、已定、未定和下一步 |
| 安排工作、准备协商或反馈 | [计划与沟通页](references/cards/work.md)：标出负荷、固定期限和可商量的事项 |
| 定目标或做复盘 | [目标与复盘页](references/cards/goals.md)：说明取舍，再选一个能试的动作 |
| 把读到的东西用起来 | [学习与记录页](references/cards/learning.md)：区分材料、个人判断和动手试验 |

每张玩法卡都配有一份填好内容的 Markdown 成稿，不用凭字段名猜版式。[查看全部 27 种场景成稿 →](references/playbook.md) · [没有 Markdown 渲染？看纯文本版 →](assets/layouts/plain-text.txt)

## 适用边界

「一页」指读者不用翻找就能判断现状，不要求每次做成一张图。只有明确要单独传阅或打印时，再用[可编辑框图示例](assets/visual-one-page-example.html)和[布局指南](references/visual-layout.md)；要印成 A4 单页，须检查分页。这是独立工具，不代表任何组织的内部标准。

[技能入口](SKILL.md)
