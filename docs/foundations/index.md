---
title: Foundations
layout: default
nav_order: 3
has_children: true
---

# Foundations

The concepts underneath every task in this guide. Read these when a task page sends you here, or all at once if you want the full picture.
{: .fs-6 .fw-300 }

Each foundation supports one or more habits in the rubric:

```mermaid
flowchart LR
  CE["Context engineering"] --> U["USE"]
  DC["Data classification"] --> U
  LF["How LLMs fail"] --> V["VERIFY"]
  HL["Human-in-the-loop design"] --> V
  HL --> D["DECIDE"]
  classDef use fill:#e8f0fe,stroke:#4a6fa5;
  classDef verify fill:#e6f4ea,stroke:#3c8c5a;
  classDef dd fill:#fef7e0,stroke:#b08900;
  class U use;
  class V verify;
  class D dd;
```

- **Context engineering:** what to give the tool so it can do the job well.
- **How LLMs fail:** hallucination, bad math, stale data, and how to catch each.
- **Data classification:** what may go into which tool.
- **Human-in-the-loop design:** where people must check, approve, or decide.
