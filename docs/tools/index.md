---
title: Tools
layout: default
nav_order: 8
has_children: true
---

# Tools

A vendor-neutral way to grow your AI toolkit one rung at a time. Features change monthly. The kinds of tools change much more slowly.
{: .fs-6 .fw-300 }

This guide describes **kinds of tools** rather than products, and it prefers approaches that work on free tiers. Climb the ladder only as far as your work needs. Each rung adds capability, and each adds something new to verify.

```mermaid
flowchart BT
  R0["0 · Basic chat"] --> R1["1 · Projects with<br/>custom instructions"]
  R1 --> R2["2 · Deep research modes"]
  R2 --> R3["3 · Source-grounded<br/>synthesis"]
  R3 --> R4["4 · Reusable templates<br/>and skills"]
  R4 --> R5["5 · Connectors<br/>and scheduling"]
  R5 --> R6["6 · Desktop agents"]
  classDef low fill:#e6f4ea,stroke:#3c8c5a;
  classDef mid fill:#e8f0fe,stroke:#4a6fa5;
  classDef high fill:#fde2e1,stroke:#b3261e;
  class R0,R1,R2 low;
  class R3,R4 mid;
  class R5,R6 high;
```

| Rung | What it adds | New thing to verify |
|:--|:--|:--|
| 1 · Projects with custom instructions | Standing context, so you stop repeating yourself | Are the instructions still current? |
| 2 · Deep research modes | Multi-source web research with citations | Does every citation exist and say what's claimed? |
| 3 · Source-grounded synthesis | Answers limited to documents you upload | Did it stay inside the sources? |
| 4 · Reusable templates and skills | Repeatable quality across tasks and people | Does the template still fit this case? |
| 5 · Connectors and scheduling | Access to your files, email, and calendar; runs on a timer | What data can it reach? Who reviews scheduled output? |
| 6 · Desktop agents | Acts on your computer: clicks, types, files | What can it change, and can you undo it? |

Colors show rising risk: green rungs mostly produce text for you to read, while red rungs can reach your data or take actions. Check [Data classification]({% link docs/foundations/data-classification.md %}) before connecting anything. To understand what runs *behind* these tools, and what it takes to build or host your own, see [Running AI]({% link docs/running-ai/index.md %}).
