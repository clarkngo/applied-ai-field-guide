---
title: Glossary
layout: default
parent: Start Here
nav_order: 7
---

# Glossary
{: .no_toc }

Plain-language definitions of the AI terms used in this guide.
{: .fs-6 .fw-300 }

<details markdown="block">
  <summary>Jump to a letter</summary>
  {: .text-delta }
1. TOC
{:toc}
</details>

## How the main terms fit together

```mermaid
flowchart TB
  AI["Artificial intelligence"] --> GEN["Generative AI"]
  GEN --> LLM["Large language model (LLM)"]
  LLM --> CHAT["Chat assistant"]
  CHAT --> PROJ["Projects and<br/>custom instructions"]
  CHAT --> DR["Deep research"]
  CHAT --> GR["Grounded synthesis"]
  CHAT --> AG["Agent"]
  AG --> CON["Connectors<br/>and scheduling"]
  P["Prompt + context"] --> LLM
  LLM --> OUT["Output"]
  OUT --> RISK["Risks: hallucination,<br/>bias, stale data"]
  RISK --> HITL["Human in the loop"]
```

## A–C

**Agent**
: An AI setup that takes several steps toward a goal, such as searching, reading, writing, or using tools, without being prompted at each step. See [Workflows & Agents]({% link docs/workflows/index.md %}).

**Agreeableness (sycophancy)**
: A model's tendency to agree with the user, accept false premises, or change a correct answer when pushed. See [How LLMs fail]({% link docs/foundations/how-llms-fail.md %}).

**Automation bias**
: Over-trusting automated output, so that reviewers approve it without really checking. See [Human-in-the-loop design]({% link docs/foundations/human-in-the-loop.md %}).

**Autonomy level**
: How much an AI step does without human approval, from 0 (a human does it) to 4 (AI acts, monitored by metrics). See [Automate or judge?]({% link docs/workflows/automate-vs-judge.md %}).

**Chat assistant**
: An application that lets you talk to a language model in conversation, often with extras like file upload, web search, or code execution.

**Connector**
: A feature that gives an AI tool access to another system, such as your email, calendar, or file storage.

**Context**
: Everything the model can consider when responding: your prompt, files, instructions, and the conversation so far. See [Context engineering]({% link docs/foundations/context-engineering.md %}).

**Context window**
: The maximum amount of text a model can consider at once.

**Custom instructions**
: Standing instructions that apply to every conversation or project, such as your role, house style, or recurring rules.

## D–H

**Data classification**
: Sorting data into levels (Public, Internal, Confidential, Restricted) to decide which tools it may go into. See [Data classification]({% link docs/foundations/data-classification.md %}).

**Deep research**
: A tool mode that searches many sources, reads them, and writes a cited report. Every citation still needs checking.

**De-identification**
: Removing or generalizing details that identify people, such as names, emails, and account numbers, before using data.

**Disclosure**
: A clear statement of AI's role in a piece of work: what it did, what you checked, and what you changed. See [the rubric]({% link docs/start-here/rubric.md %}).

**GPU**
: Graphics processing unit, a chip built for massively parallel arithmetic, which is what running AI models mostly is. See [Hardware requirements]({% link docs/running-ai/hardware.md %}).

**Generative AI**
: AI that produces new content, such as text, images, audio, or code, rather than only classifying or predicting from data.

**Grounding**
: Limiting a model's answers to specific sources you provide, usually with citations to passages. It reduces hallucination but doesn't eliminate it.

**Hallucination**
: A confident, plausible, false output, such as an invented statistic, citation, or quote.

**Human in the loop**
: A process design where people review, approve, or decide at defined points. See [Human-in-the-loop design]({% link docs/foundations/human-in-the-loop.md %}).

**First principles**
: Ten basic truths about how AI tools behave, such as "it predicts, it doesn't know." See [First principles of AI]({% link docs/start-here/first-principles.md %}).

## I–P

**Inference**
: Running a trained model to produce an output, as opposed to training it.

**Knowledge cutoff**
: The date after which a model has no training data. Unless the tool searches the web, the model doesn't know about later events.

**Large language model (LLM)**
: A model trained on large amounts of text to predict likely next words. It powers chat assistants.

**Model**
: The trained AI system itself, as distinct from the app or tool you use to access it.

**Open-weight model**
: A model whose weights are published so you can run it yourself, under its license terms.

**Project**
: A workspace in some AI tools where instructions and files persist across conversations.

**Prompt**
: The instructions and input you give a model.

**Proxy (in bias)**
: A detail, such as a zip code or school, that indirectly stands in for a protected characteristic. See [Bias, fairness, and ethics]({% link docs/foundations/bias-and-ethics.md %}).

## R–Z

**Quantization**
: Storing a model's weights at lower precision (such as 4-bit) to cut memory needs, usually with some loss of quality.

**RAG (retrieval-augmented generation)**
: Finding relevant passages in your documents first, then having the model answer from them. See [Software and infrastructure]({% link docs/running-ai/software-infrastructure.md %}).

**Retention**
: How long a tool's provider keeps your inputs and outputs.

**Second principles**
: Ten working rules derived from the first principles, such as "provide, don't describe." See [Second principles of AI]({% link docs/start-here/second-principles.md %}).

**Scheduling**
: Running an AI task automatically at set times, such as a weekly digest.

**Skill (or template)**
: A saved, reusable set of instructions for a recurring task.

**Socratic tutor**
: An AI set up to ask guiding questions instead of giving answers. See [Socratic tutor prompt]({% link docs/educators/socratic-tutor-prompt.md %}).

**Swap test**
: A bias check: change one detail about a person (name, pronouns) and compare the outputs. See [Bias, fairness, and ethics]({% link docs/foundations/bias-and-ethics.md %}).

**Third principles**
: Ten principles for teams and organizations that make good AI habits the default, such as "make the safe path the easy path." See [Third principles of AI]({% link docs/start-here/third-principles.md %}).

**Token**
: A small chunk of text, often part of a word, that a model reads and generates. Context windows and pricing are usually measured in tokens.

**Training (on inputs)**
: When a provider uses your inputs to improve future models. Whether this happens depends on the tool, plan, and settings.

**VRAM**
: Memory on a GPU. A model's weights usually need to fit in it to run quickly.

**Use · Verify · Disclose · Decide**
: The four habits this guide is built on. See [the rubric]({% link docs/start-here/rubric.md %}).
