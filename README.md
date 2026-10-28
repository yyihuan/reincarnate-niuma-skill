# reincarnate-niuma

[中文](#中文) · [English](#english)

## 中文

一个为**具体雇主或岗位**准备求职简历和申请材料的 Agent Skill。

也就是：**求投胎成牛马。**

它适合认真研究一个想去的地方，梳理自己的经历，再把双方的匹配讲清楚。**不适合海投。**

### 怎么用

把岗位说明、已有简历和相关经历交给 Agent，使用 `$reincarnate-niuma` 开始。已有底稿时可以直接续接当前阶段。

```text
使用 $reincarnate-niuma。我想申请这个岗位，请先查看我的已有材料，
通过多轮提问整理职业底稿和侧写，再分析岗位匹配与申请材料的写作策略。
```

流程从多轮访谈开始，保留原始叙述，整理成可检索的事实和不依附岗位的职业侧写。随后分析雇主与岗位，先写 CV，再准备 Cover Letter 或招聘方要求的其他材料。

招聘视角评审使用独立上下文，只看岗位和实际提交材料。每轮反馈回来，先判断写作策略是否需要调整，再由用户决定修改哪些内容、是否继续，以及何时定稿。有接口时可自动委派，也支持同模型新会话或手动转交。

### 安装

在 Codex 的默认个人 Skill 目录安装：

```bash
git clone https://github.com/yyihuan/reincarnate-niuma-skill.git ~/.codex/skills/reincarnate-niuma
```

如果设置了 `CODEX_HOME`，将目录放入其 `skills/reincarnate-niuma` 下。其他兼容 Agent 按各自的 Skill 加载方式使用，保留目录结构即可。

### 材料经验与贡献

通用流程和地区／材料经验分开维护。目前附有英国 CV 与 Cover Letter 模块；其他材料由 Agent 按实际要求检索。欢迎通过 PR 补充其他地区或材料的经验，请附可靠来源、适用范围及核查日期。

- [Skill 执行入口](SKILL.md)
- [材料模块与贡献规则](references/material-modules.md)
- [独立招聘评审与可转交提示词](references/independent-screening.md)

个人履历保存在使用者自己的工作区。共享规则和示例中请勿加入真实履历、私人评语或账号配置。

## English

An Agent Skill for writing a CV and application materials **tailored to a specific employer or role**.

In other words: **trying to reincarnate as a corporate workhorse.** “Niuma” literally means “cattle and horses,” Chinese slang for people doing the daily grind.

Use it when you have a particular opportunity in mind and want to explain how your actual experience fits. **It is not designed for mass applications.**

### How it works

Start with the job description, your existing CV, and whatever experience you can recall. Invoke `$reincarnate-niuma`; if you already have a career record, resume from the relevant stage.

```text
Use $reincarnate-niuma to help me apply for this role. Read my existing materials,
interview me over several rounds to build a career record and profile,
then analyze the role fit and plan the application materials.
```

The workflow preserves your original account, organizes searchable facts, and builds a career profile independent of the target role. It then analyzes the employer and role, drafts the CV first, and develops a writing strategy for the cover letter or other requested documents.

Recruiter-style reviewers work in fresh contexts and see only the job information and application materials. After each review, the drafting agent checks whether the strategy needs to change. You decide which suggestions to adopt, whether to continue, and when the draft is ready. Reviews can use connected agents, a fresh session with the same model, or a prompt you transfer manually.

### Installation

For Codex with its default personal Skill directory:

```bash
git clone https://github.com/yyihuan/reincarnate-niuma-skill.git ~/.codex/skills/reincarnate-niuma
```

If you set `CODEX_HOME`, use its `skills/reincarnate-niuma` directory. For other compatible agents, follow their Skill-loading mechanism and preserve the folder structure. The Skill instructions are written in Chinese; this README provides an English introduction.

### Material guides and contributions

The general workflow is separate from regional and document-specific guidance. A UK CV and cover-letter module is included. For other documents, the agent researches the relevant requirements. Contributions via PR are welcome: include reliable sources, scope, and the date you checked them.

- [Skill entry point](SKILL.md)
- [Material modules and contribution rules](references/material-modules.md)
- [Independent recruiter review and transferable prompts](references/independent-screening.md)

Keep personal career records in your own workspace. Shared guidance and examples should not contain real candidate histories, private feedback, or account configuration.
