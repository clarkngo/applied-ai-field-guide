---
title: Workflows & Agents
layout: default
nav_order: 6
has_children: true
---

# Workflows & Agents

Simple patterns for chaining AI steps together, and for deciding where a human has to stay in the loop.
{: .fs-6 .fw-300 }

An **agent** is an AI setup that takes several steps toward a goal, such as searching, reading, drafting, and calling tools, without you prompting each step. Agents can save real time on multi-step work. They also compound errors: a mistake in step 1 carries through every step after it. The patterns here keep them simple and put human checkpoints where they count.

```mermaid
flowchart LR
  subgraph Chat["Single prompt"]
    A1[Prompt] --> A2[Answer]
  end
  subgraph WF["Workflow"]
    B1[Step 1] --> B2[Step 2] --> B3[Step 3]
  end
  subgraph AG["Agent"]
    C1[Goal] --> C2{"Plan"} --> C3[Act] --> C4[Observe] --> C2
  end
  Chat --> WF --> AG
```

Before you build any workflow, read [Should you use AI here?]({% link docs/start-here/should-you-use-ai.md %}). Many "agent" ideas turn out to be plain automation, and a few turn out to be jobs that should stay with a person.
