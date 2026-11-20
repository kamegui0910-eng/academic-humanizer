# Academic Humanizer

## 中文

**Academic Humanizer** 是一套学术写作自然化技能，用于起草、修改和润色论文、essay、案例研究、报告或正式书面作业，使文本读起来像严谨、自然的人类学术写作，而不是 AI 生成的套话。

它采用强制三遍修订流程：

1. **Pass 1：学术严谨与结构** — 删掉套话开场、堆叠转承和空泛的重要性表述，把引用嵌入具体主张，拆开过长的从句堆叠。
2. **Pass 2：清除常见 AI 写作痕迹** — 去掉 `not X, but Y` 对照、戏剧化收束、空洞深刻句，以及 `delve`、`tapestry`、`pivotal` 等套词。
3. **Pass 3：防区块检测的节奏与结构变化** — 打破连续平行句式、对称反义句、分号对偶，以及多道问答共用同一模板的节奏，降低 Copyleaks、Turnitin 等重叠窗口检测器对结构均匀性的误报。

**核心保证**

- 保留全部引文、统计数字、公式和技术术语，不为文风改动事实。
- 保持正式、克制、有证据依据的学术语气，不故意口语化或加入虚假个性。
- 主张强度与证据匹配，不用夸大动词。

**怎样用**

用 skill-installer 安装：

```text
$skill-installer Install skills/academic-humanizer from https://github.com/kamegui0910-eng/academic-humanizer
```

也可以下载本仓库，把 `skills/academic-humanizer` 整个文件夹放入所用工具的 skills 目录（Cursor / Grok Bot / Claude / ChatGPT 等以各自说明为准），或直接把 [SKILL.md](skills/academic-humanizer/SKILL.md) 作为系统提示 / 自定义指令使用。然后告诉 AI：

```text
使用 Academic Humanizer 修订这篇学术文稿，保留全部引文、数据和术语。
```

[Skill 正文](skills/academic-humanizer/SKILL.md)

## English

**Academic Humanizer** is a reusable academic writing skill for drafting, revising, and polishing papers, essays, case studies, reports, and other formal work so the prose reads like rigorous, natural human scholarship rather than AI-generated text.

It uses a mandatory three-pass editing workflow:

1. **Pass 1: Academic Rigor & Structure** — Cut formulaic openers, stacked transitions, and empty significance claims; integrate citations at the claim they support; break clause-stacked sentences.
2. **Pass 2: Strip General AI Writing Tells** — Remove "not X, but Y" contrasts, dramatic one-line closers, hollow profundities, and stock AI vocabulary such as *delve*, *tapestry*, and *pivotal*.
3. **Pass 3: Anti-Block-Detector Rhythm & Structural Variation** — Break repeated parallel openers, mirrored antithesis, semicolon contrasts, and uniform Q&A templates so overlapping-window detectors (such as Copyleaks and Turnitin) are less likely to flag structural uniformity.

**Core guarantees**

- Preserves every citation, statistic, equation, and technical term.
- Keeps a formal, measured scholarly tone — no forced slang or artificial personality.
- Matches claim strength to evidence.

Install with the command above, copy `skills/academic-humanizer` into your tool's skills directory, or paste [SKILL.md](skills/academic-humanizer/SKILL.md) into custom instructions for Cursor, Grok Bot, Claude, or ChatGPT. Then ask the model to revise the draft with Academic Humanizer while keeping all citations and facts intact.

## Attribution

This skill is inspired by [`AIScientists-Dev/academic-humanizer`](https://github.com/AIScientists-Dev/academic-humanizer) (Pass 1 academic rigor) and [`blader/humanizer`](https://github.com/blader/humanizer) (Pass 2 general AI writing tells), and extends them with Pass 3 structural rules for block-level AI detectors.
