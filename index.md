---
title: Home
layout: default
nav_order: 1
description: "A practical field guide to using AI with good judgment in real business and teaching work."
permalink: /
---

# Applied AI Field Guide
{: .fs-9 }

Judgment over prompts: using AI in real business and teaching work.
{: .fs-6 .fw-300 }

[New to AI? Start with the quick start]({% link docs/start-here/what-is-ai.md %}){: .btn .btn-primary .mr-2 }
[Read the rubric]({% link docs/start-here/rubric.md %}){: .btn }

---

Most AI advice is about prompts. This guide is about **judgment**: knowing which tool to use, what context to give it, how to check what comes back, how to be open about AI's role, and when the decision has to stay with you. Every page is built around a real task, such as a break-even analysis, a market scan, or a course announcement. Each one walks through an AI-assisted approach, a verification checklist, and the ways things commonly go wrong. The examples use fictional companies and worked numbers you can check yourself.

## Who this is for

**Business students** (undergraduate, MBA, EMBA) who want to use AI in business tasks without handing over their thinking. Start with [For Students]({% link docs/students/index.md %}).

**Business educators** (faculty, instructional designers, corporate trainers) who design AI-fluency activities or use AI in course operations. Start with [For Educators]({% link docs/educators/index.md %}).

## The rubric: Use · Verify · Disclose · Decide

Every task page in this guide is organized around four habits.

```mermaid
flowchart LR
  U["<b>USE</b><br/>Right tool,<br/>right context"] --> V["<b>VERIFY</b><br/>Math, sources,<br/>assumptions"]
  V --> D1["<b>DISCLOSE</b><br/>Be open about<br/>AI's role"]
  D1 --> D2["<b>DECIDE</b><br/>A human owns<br/>the conclusion"]
  V -.->|"Found a problem"| U
  classDef use fill:#e8f0fe,stroke:#4a6fa5;
  classDef verify fill:#e6f4ea,stroke:#3c8c5a;
  classDef dd fill:#fef7e0,stroke:#b08900;
  class U use;
  class V verify;
  class D1,D2 dd;
```

| | Habit | What it means |
|:--|:--|:--|
| 1 | **Use** | Pick the right tool and give it the right context. |
| 2 | **Verify** | Check the math, the sources, and the assumptions. Look for hallucinations. |
| 3 | **Disclose** | Be transparent about AI's role, following your course or company policy. |
| 4 | **Decide** | A human owns the conclusion and is accountable for it. |

The [full rubric]({% link docs/start-here/rubric.md %}) describes what beginning, developing, and proficient work looks like for each habit. The habits come from ten [first principles]({% link docs/start-here/first-principles.md %}) about how AI works.

## How the guide is organized

- **[Start Here]({% link docs/start-here/index.md %})**: what AI is, first, second, and third principles, whether to use it, the rubric, and a glossary.
- **[Foundations]({% link docs/foundations/index.md %})**: context engineering, how LLMs fail, data classification, human-in-the-loop design, bias and ethics.
- **[For Students]({% link docs/students/index.md %})**: worked business tasks.
- **[For Educators]({% link docs/educators/index.md %})**: challenge design, a Socratic tutor prompt, knowledge checks, course operations, course AI policies, AI-resilient assessment.
- **[Workflows & Agents]({% link docs/workflows/index.md %})**: simple multi-step patterns, and when to automate.
- **[Tools]({% link docs/tools/index.md %})**: a vendor-neutral learning ladder, and how to evaluate a tool.
- **[Templates]({% link docs/templates/index.md %})**: every copy-paste template and rubric in one place.

---

This guide is an independent professional reference by [Clark Ngo](https://clarkngo.github.io/). It is not affiliated with or endorsed by any university or employer.
