# Applied AI Field Guide

A practical field guide to using AI with good judgment in real business and teaching work.

**Live site:** https://clarkngo.github.io/applied-ai-field-guide/

## What this is

The guide teaches **judgment inside real business tasks**, not generic prompt tips. Every task page is built around a four-part AI-fluency rubric:

| Habit | Meaning |
|:--|:--|
| **Use** | Pick the right tool and give it the right context. |
| **Verify** | Check the math, the sources, the assumptions, and look for hallucinations. |
| **Disclose** | Be transparent about AI's role, following course or company policy. |
| **Decide** | The human owns the conclusion and is accountable for it. |

It's written for two audiences:

- **Business students** (undergraduate, MBA, EMBA) learning to use AI with good judgment in business tasks.
- **Business educators** (faculty, instructional designers, corporate trainers) designing AI-fluency activities and using AI in course operations.

This is an independent professional reference by [Clark Ngo](https://clarkngo.github.io/). It is not affiliated with or endorsed by any institution. All companies and scenarios in the examples are fictional.

## Site structure

```
index.md                 Home page
docs/
  start-here/            What is AI, first/second/third principles, should you use AI, the rubric, glossary
  foundations/           Context engineering, how LLMs fail, data classification, human-in-the-loop, bias and ethics
  students/              Worked business tasks (break-even, cash flow, market analysis, research-to-brief,
                         business writing, spreadsheet analysis, customer feedback)
  educators/             Challenge design, Socratic tutor, knowledge checks, course operations,
                         course AI policy, AI-resilient assessment
  workflows/             Agent patterns and when to automate
  running-ai/            Hardware, software and infrastructure, skills and roles, operating AI
  tools/                 Vendor-neutral learning ladder, evaluating a tool
    products/            Product landscape: named, dated examples (see rules below)
  templates/             Index of every copy-paste template and rubric, plus the AI-use log
  _templates/            Page templates for contributors (not published)
```

Built with [Jekyll](https://jekyllrb.com/) and the [Just the Docs](https://just-the-docs.com/) theme, and deployed to GitHub Pages by GitHub Actions (`.github/workflows/jekyll.yml`) on every push to `main`.

## Run it locally

Prerequisites: Ruby 3.2 (see `.ruby-version`) and Bundler.

```bash
bundle install
bundle exec jekyll serve --livereload
```

Open http://localhost:4000/applied-ai-field-guide/.

To build without serving:

```bash
bundle exec jekyll build
```

The build prints Sass deprecation warnings that come from inside the theme. Those are expected. Any other warnings or errors are real.

## Add a new page

1. **Copy a template** from `docs/_templates/`:
   - `task-page.md` for a worked task (students, educators, workflows).
   - `concept-page.md` for an idea or tool category (foundations, tools).
2. **Put it in the right section folder** with a short, hyphenated filename, e.g. `docs/students/pricing-analysis.md`.
3. **Set the front matter.** `parent` must exactly match the section's `title`:

   ```yaml
   ---
   title: Pricing analysis
   layout: default
   parent: For Students      # Start Here | Foundations | For Students | For Educators | Workflows & Agents | Tools
   nav_order: 5              # position within the section
   ---
   ```

4. **Fill in every template section, in order:** Scenario → Why it matters → AI-assisted approach → Prompt template → Verify checklist → Common failure modes → Disclose and decide notes → For educators: turn this into a challenge.
5. **Add at least one diagram.** Use a fenced `mermaid` block (flowchart, `xychart-beta`, `quadrantChart`, `timeline`, `pie`, and so on). Diagrams render in the browser, so check the page locally.
6. **Link internally with `{% link %}`**, e.g. `[rubric]({% link docs/start-here/rubric.md %})`. The build fails if the target doesn't exist, which catches broken links.
7. **If the page adds a template,** list it in `docs/templates/index.md`.
8. **Run `bundle exec jekyll build`** and open the page locally before opening a PR.

A new top-level section needs an `index.md` with `has_children: true` and a `nav_order`.

## Content rules

This is a public repository, so:

- **No confidential or institution-specific content.** Don't name private individuals, partner organizations, internal projects, or unreleased courses. Use fictional companies and generic scenarios.
- **Don't claim endorsement** by any school or employer.
- **Write plainly** for busy professionals: short paragraphs, concrete examples, no hype.
- **Check every number.** Worked examples must be correct. Recompute them before committing.
- **Never invent citations.** Cite a real, verifiable source, or leave `<!-- TODO: source -->`.
- **Stay vendor-neutral in the core pages.** Describe kinds of tools rather than products, and prefer free tiers. Named products follow the rules below.

## Naming products and technologies

The guide's principles and task pages describe *kinds* of tools, because products change monthly and the judgment doesn't. Readers still need concrete names, so products appear in one place, under rules that keep them accurate and neutral.

1. **Two layers.** Core pages (Start Here, Foundations, For Students, For Educators, Workflows & Agents, Running AI, and the Tools overview and ladder) stay product-free. Named AI products appear only in the **Product landscape** pages under Tools. A core page may link there, for example "see the product landscape for current examples."
2. **Technologies and standards can be named anywhere.** Stable concepts, techniques, and open standards (RAG, quantization, open-weight models, prompt injection, WCAG) are fine on any page. Specific products and projects, commercial or open-source, go in the landscape. Everyday non-AI software (for example, a spreadsheet program) may be named where the instruction depends on how it behaves.
3. **Category first, several options.** Each landscape page covers one category of tool, explains how to judge it, and lists at least two options. Include a free or open-source option where one exists. Don't rank, score, or call anything "best."
4. **Every claim is sourced and dated.** Each product entry links to the vendor's official documentation (or the project's official repository) and records the date it was checked. Only state what that source says. If the docs don't confirm something, write "Not confirmed in official docs." Never rely on third-party reviews or memory.
5. **No prices or plan limits.** They change too often. Say whether a free option exists, if the official source confirms it, and link to the vendor's plans page for the rest.
6. **Neutral and transparent.** No affiliate links or sponsored placement. Each landscape page states the author's relationship with listed vendors, and discloses if it was drafted with an AI assistant made by a listed vendor.
7. **Nothing institution-specific.** Don't say which tools any particular school, employer, or organization licenses, approves, or uses.
8. **Review on a schedule.** Each landscape page shows a "Last reviewed" date and is re-checked at least every quarter. Record renames and removals in the page's change log, keeping the former name so readers can find it. If a page goes more than six months without review, add a warning at the top or remove the entries.

To add a landscape page, copy `docs/_templates/landscape-page.md`.
