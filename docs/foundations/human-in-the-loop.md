---
title: Human-in-the-loop design
layout: default
parent: Foundations
nav_order: 4
---

# Human-in-the-loop design
{: .no_toc }

Where to put human checkpoints in an AI-assisted process so that errors get caught before they cost anything.
{: .fs-6 .fw-300 }

{: .stub }
This page is a stub. It follows the [page template](https://github.com/clarkngo/applied-ai-field-guide/tree/main/docs/_templates) and will be filled in soon.

<details open markdown="block">
  <summary>On this page</summary>
  {: .text-delta }
1. TOC
{:toc}
</details>

## Scenario

<!-- TODO -->

## Why it matters

<!-- TODO -->

## Key ideas

```mermaid
flowchart LR
  A[Input] --> B[AI step] --> C{"Human<br/>checkpoint"}
  C -->|Approve| D[Next step or output]
  C -->|Fix| B
  C -->|Reject| E[Human does it]
```

<!-- TODO -->

## Worked example

<!-- TODO -->

## Verify checklist

<!-- TODO -->

## Common failure modes

<!-- TODO -->

## Disclose and decide notes

<!-- TODO -->

## For educators: turn this into a challenge

<!-- TODO -->
