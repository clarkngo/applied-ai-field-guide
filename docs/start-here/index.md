---
title: Start Here
layout: default
nav_order: 2
has_children: true
---

# Start Here
{: .no_toc }

What this guide is, who it's for, and how to get value from it in your first hour.
{: .fs-6 .fw-300 }

<details open markdown="block">
  <summary>On this page</summary>
  {: .text-delta }
1. TOC
{:toc}
</details>

## What this guide is

The Applied AI Field Guide is a practical reference for using AI in real business and teaching work. It is not a list of prompt tricks. Prompts change every few months as tools change. The judgment behind a good prompt does not: knowing what to ask, what to check, what to disclose, and what to decide yourself.

Each page is built around a task you might actually do on a Tuesday afternoon, such as a break-even analysis for a pricing decision, a market scan before a strategy meeting, or a knowledge check for next week's class. Every task page follows the same pattern, so once you've read one you know where to find things in the rest.

The guide is vendor-neutral. It describes kinds of tools ("a chat assistant with file upload", "a source-grounded notebook") rather than specific products, and it prefers approaches that work on free tiers.

## Who it's for

| If you are... | You want to... | Start with |
|:--|:--|:--|
| A business student (undergraduate, MBA, EMBA) | Use AI on coursework and job tasks without outsourcing your thinking | [Break-even analysis]({% link docs/students/break-even-analysis.md %}) |
| A faculty member or instructional designer | Design activities that build AI fluency, not AI dependence | [Designing an AI-fluency challenge]({% link docs/educators/ai-fluency-challenge.md %}) |
| A corporate trainer | Run hands-on AI practice with realistic business scenarios | [Socratic tutor prompt]({% link docs/educators/socratic-tutor-prompt.md %}) |
| Anyone new to AI | Understand what it is and try it safely in 15 minutes | [What is AI? A quick start]({% link docs/start-here/what-is-ai.md %}) |

## How to use it

```mermaid
flowchart LR
  A["New to AI?<br/>Read the quick start"] --> FP["First, second, and<br/>third principles"]
  FP --> B["Should AI touch<br/>this task at all?"]
  B --> C["Learn the rubric:<br/>Use · Verify · Disclose · Decide"]
  C --> D{"Who are you?"}
  D -->|Student| E["Work one task page<br/>end to end"]
  D -->|Educator| F["Run one challenge<br/>with your learners"]
  E --> G["Go deeper:<br/>Foundations, Workflows, Tools"]
  F --> G
```

1. **If AI is new to you**, read [What is AI? A quick start]({% link docs/start-here/what-is-ai.md %}). It takes about 10 minutes and ends with a safe first exercise. If you want a structured plan, follow [Your first 30 days]({% link docs/start-here/learning-path.md %}), and skim [AI myths and realities]({% link docs/start-here/ai-myths.md %}) to clear up common misconceptions.
2. **Learn the principles.** [First principles]({% link docs/start-here/first-principles.md %}) explain how AI tools behave, and [second principles]({% link docs/start-here/second-principles.md %}) turn that into ten working rules. If you lead a team or a course, [third principles]({% link docs/start-here/third-principles.md %}) show how to make those rules hold for everyone. They last longer than any tool tip.
3. **Before reaching for AI on any task**, run through [Should you use AI here?]({% link docs/start-here/should-you-use-ai.md %}). Sometimes the right answer is a spreadsheet formula, and sometimes it's you.
4. **Learn the four habits** in [the rubric]({% link docs/start-here/rubric.md %}). Everything else in the guide hangs on them.
5. **Work one task page end to end**, with a real tool open. Reading about verification is not the same as catching your first hallucination.
6. **Use [Templates]({% link docs/templates/index.md %})** when you just need the copy-paste version, and the [Glossary]({% link docs/start-here/glossary.md %}) when a term is unfamiliar.

## How every task page is laid out

Every task page uses the same eight sections, in the same order:

```mermaid
flowchart TB
  S[Scenario] --> W[Why it matters] --> A[AI-assisted approach] --> P[Prompt template]
  P --> V[Verify checklist] --> F[Common failure modes] --> D[Disclose and decide notes] --> E[For educators: turn this into a challenge]
  classDef use fill:#e8f0fe,stroke:#4a6fa5;
  classDef verify fill:#e6f4ea,stroke:#3c8c5a;
  classDef decide fill:#fef7e0,stroke:#b08900;
  class A,P use;
  class V,F verify;
  class D decide;
```

The colors line up with the rubric: blue sections are about **Use**, green about **Verify**, and yellow about **Disclose** and **Decide**. The last section is for educators, but students can read it too. It shows how the same task becomes a practice challenge.

## What this guide is not

- **Not a policy.** Your course, school, or employer sets the rules on AI use. This guide helps you work well inside them. When in doubt, ask.
- **Not tool documentation.** Features change monthly. Check the current documentation for whatever tool you use.
- **Not an endorsement.** This is an independent professional reference by [Clark Ngo](https://clarkngo.github.io/). It is not affiliated with or endorsed by any university or employer. All companies in the examples are fictional.
