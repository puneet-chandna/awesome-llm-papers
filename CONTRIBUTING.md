# 🤝 Contributing to Awesome LLM Papers

Help readers find work that changes how they understand language models. **Quality over quantity**, across any lab, category or year.

## 🚀 Quick Start

[**Suggest a paper through the form →**](https://github.com/puneet-chandna/awesome-LLM-papers/issues/new?template=new-paper.yml)

Bring the primary source, its distinct contribution, why a reader benefits, and an important limitation. Older omissions and factual corrections are welcome.

---

## 📄 Paper Submission Guidelines

We look for one or more of these qualities:

- **A distinct idea:** a method, architecture or result that changes how a problem can be approached.
- **Strong evidence:** clear tasks, baselines, assumptions and limitations supporting the claimed contribution.
- **Lasting reader value:** a reusable mental model, evaluation design, research resource or essential historical link.

Explain the closest related work and what the paper adds. Popularity, institution, recency, citation counts and a leaderboard gain alone do not establish that case. We have no category quotas or numerical improvement cutoff.

Preprints, technical reports and author research resources can qualify when their contribution and evidence merit inclusion. Label the document type. Code and data are useful when available; they are optional. Released weights alone do not establish full reproducibility.

**Hall of Fame has a higher bar:** established lasting influence. Promising new breakthroughs can belong in the main categories without a Hall badge.

## 📊 What Makes a Good Submission?

```text
Paper: Lost in the Middle: How Language Models Use Long Contexts
Primary source: https://arxiv.org/abs/2307.03172
Contribution: Varies the position of relevant information in comparable long inputs.
Reader value: Separates context capacity from effective information use.
Limit: Tested 2023 models and selected QA/retrieval tasks; newer models need retesting.
Related work: Context extensions and RAG comparisons answer different questions.
```

A small, controlled result can be worth reading. A large score increase needs its model, task, data and budget before readers can assess it.

---

## 🎯 Submission Process

### Option 1: GitHub Issue

Use the [paper form](https://github.com/puneet-chandna/awesome-LLM-papers/issues/new?template=new-paper.yml), or identify a correction and its primary-source evidence in an issue. Reviews happen as maintainer time permits.

### Option 2: Pull Request

1. Search the complete index and topic pages for the title and identifier, including alternate URLs or titles.
2. Add one record to [the chronological index](categories/all-papers.md), using the earliest public paper/resource date you can verify. Note a different venue/revision year where useful.
3. Add the primary topic entry. Use a secondary category when it helps navigation; a short cross-link can avoid repeating prose.
4. Check titles, authors, local paths, anchors and affected counts. A cross-list changes category counts but adds no new unique work.
5. Explain the evidence in your PR. Hall membership and README features are separate editorial choices; routine additions need neither.

The eight categories are [Architectures](categories/architectures.md), [Reasoning & Agents](categories/reasoning.md), [Efficiency & Scaling](categories/efficiency.md), [Training & Alignment](categories/training.md), [Multimodal](categories/multimodal.md), [RAG & Knowledge](categories/rag.md), [Safety & Security](categories/safety.md), and [Analysis & Theory](categories/analysis.md).

## 📝 Paper Format Template

```markdown
### 📄 [Paper Title](primary-source-link)

**Authors:** First author et al.<br>
**Contribution:** `Short method or research theme`

> Two to four sentences: distinct contribution, why it is useful to read,
> and a meaningful limitation. Scope metrics to the evaluated setup.
```

Follow nearby entries. Link code/data or an existing summary when helpful. Hall badges require the corresponding editorial decision; invented impact scores and universal priority claims are unhelpful.

For a correction, update every affected occurrence: index, topic pages, Hall, README and existing summary. Explain what the source supports; an inaccurate description is separate from the paper's merits.

## 🏆 Recognition

Contributions and discussions remain visible in GitHub's history. Acceptance does not imply a promised README feature or update schedule.

## 💬 Questions?

- **Email:** puneetchandna7@gmail.com
- **Twitter:** [@puneet_chandna_](https://x.com/puneet_chandna_)

## 📜 Code of Conduct

Follow our [Code of Conduct](CODE_OF_CONDUCT.md). Keep feedback respectful, constructive and focused on evidence.
