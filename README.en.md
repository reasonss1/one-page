# One Page · Agent Skill

[简体中文](README.md)

**The point isn’t to make AI say less. It’s to know where things stand without reading three paragraphs first.**

For updates to people, answer the question first, in plain text or Markdown. Put any caveat that changes the answer right next to it. Agent-to-agent handoffs keep their existing format.

> **You:** `$one-page` I merged both sales sheets, but two refunds still don’t match an order. Can I send the weekly report?
>
> **AI:** **Not yet.** Those refunds affect net sales. Send me the two original order IDs so I can check the total.

## Install in Codex

Run this in the terminal where you use Codex. If you use WSL, run it inside that distribution.

```sh
git clone --depth 1 --branch v0.2.0 https://github.com/reasonss1/one-page.git "$HOME/.agents/skills/one-page"
```

Open a new session, type `$one-page`, and add your task or notes. No Git? [Download the ZIP](https://codeload.github.com/reasonss1/one-page/zip/refs/tags/v0.2.0) and move the extracted folder containing `SKILL.md` to `~/.agents/skills/one-page/`.

To make this the default for your project, add this line to `AGENTS.md`:

```markdown
Use $one-page for progress updates and results meant for people. Lead with the answer, then give the evidence, blockers, or unverified details that affect it.
```

## From a real chat: a device test plan

![A test plan in a Chinese-language chat. Its columns show the step, how to run it, and what counts as a pass. Its rows cover setup, sequential tests, and exception handling.](assets/chat-test-plan.png)

Each step sits next to its pass criteria. The screenshot shows what to check, not which tests passed.

[27 scenario layouts](references/playbook.md) · [Plain-text examples](assets/layouts/plain-text.txt) · [Markdown template](assets/one-page-template.md) (all in Chinese)
