---
title: Research-to-brief pipeline
layout: default
parent: Workflows & Agents
nav_order: 1
---

# Research-to-brief pipeline
{: .no_toc }

A simple multi-step agent pattern that gathers sources, extracts claims, and drafts a cited brief, with human checkpoints.
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

## AI-assisted approach

```mermaid
flowchart LR
  Q["You: question<br/>+ scope"] --> S["Agent: search<br/>and collect"] --> C1{"You: approve<br/>source list"}
  C1 --> E["Agent: extract<br/>claims + quotes"] --> D["Agent: draft<br/>brief"] --> C2{"You: check<br/>citations, decide"}
```

<!-- TODO -->

## Prompt template

<!-- TODO -->

## Verify checklist

<!-- TODO -->

## Common failure modes

<!-- TODO -->

## Disclose and decide notes

<!-- TODO -->

## For educators: turn this into a challenge

<!-- TODO -->
