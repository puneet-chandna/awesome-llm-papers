# Awesome LLM Papers [![Awesome](https://awesome.re/badge.svg)](https://awesome.re)

[![License: CC0-1.0](https://img.shields.io/badge/License-CC0_1.0-lightgrey.svg)](https://creativecommons.org/publicdomain/zero/1.0/)

> A curated list of seminal and breakthrough papers in Large Language Models.

**Read what matters. Skip the noise.** 🎯

Find the idea that changed the field, understand what the evidence supports, and follow it to the next useful paper. Selection favors distinct contributions and lasting reader value, across any lab, category or year.

**Your starting point:** [Understand the foundations](categories/hall-of-fame.md) · [Follow a reading route](#-this-weeks-essential-reads) · [Find a research area](#%EF%B8%8F-browse-by-category)

## Contents

- [🔥 Today's Pick](#-todays-pick)
- [🔥 Trending Topics](#-trending-topics)
- [📆 This Week's Essential Reads](#-this-weeks-essential-reads)
- [📚 Must-Read Papers (Hall of Fame)](#-must-read-papers-hall-of-fame)
- [🗂️ Browse by Category](#%EF%B8%8F-browse-by-category)
- [📈 Research Trends Dashboard](#-research-trends-dashboard)
- [🤝 Contributing](#-contributing)

## 🔥 Today's Pick

### 📍 [Lost in the Middle: How Language Models Use Long Contexts](https://arxiv.org/abs/2307.03172)

*Selected 10 October 2026 · First public paper: July 2023 · TACL 2024*

<table>
<tr>
<td width="70%" valign="top">

**Authors:** Nelson F. Liu et al.

**The idea to take away:** accepting a long input and using it well are different abilities.

The authors move relevant information through long inputs while keeping the task comparable. Many tested models answer better when that information is near the beginning or end, and worse when it sits in the middle.

**Why read it:** this gives you a practical evaluation design for long-context models and retrieval systems—not just a larger context-window number.

</td>
<td width="30%" valign="top">

**Read with these questions:**

- Where is the useful evidence?
- Does moving it change the answer?
- Which model and task were tested?

**Resources:** [Paper](https://arxiv.org/abs/2307.03172) · [TACL version](https://aclanthology.org/2024.tacl-1.9/) · [Related reading](categories/rag.md#-long-context)

</td>
</tr>
</table>

> **Keep the boundary in view:** these are experiments with particular 2023 models, multi-document QA and key-value retrieval. Retest the idea on your own model and task.

---

## 🔥 Trending Topics

*Editorial reading themes selected 10 October 2026. These are suggested directions through the collection, not measured popularity rankings.*

| Research question | Start reading |
| :-- | :-- |
| ✅ **How do we know a solution is right?** | [Verifiers](https://arxiv.org/abs/2110.14168) → [Process supervision](https://arxiv.org/abs/2305.20050) |
| 🌀 **Can a model think without writing every step?** | [Coconut](https://arxiv.org/abs/2412.06769) · [Recurrent depth](https://arxiv.org/abs/2502.05171) |
| 🧠 **What belongs inside the context window?** | [Long context](categories/rag.md#-long-context) · [Memory systems](categories/rag.md#-memory-systems) |
| 🧩 **Where should computation and memory go?** | [MoE](categories/architectures.md#-mixture-of-experts) · [Recent architectures](categories/architectures.md#-recent-breakthroughs) |
| 🛡️ **When does alignment leave a weakness behind?** | [Evaluation](categories/analysis.md#-evaluation) · [Safety](categories/safety.md) |

---

## 📆 This Week's Essential Reads

<details open>
<summary><b>Five readings: from visible reasoning to latent computation</b> · Selected 10 October 2026</summary>

Use the weekday labels as a suggested reading sequence at your own pace.

| Reading | Paper and question |
| :-- | :-- |
| **Monday**<br>Elicit | [Zero-Shot Reasoners](https://arxiv.org/abs/2205.11916)<br>What changes when we request reasoning without demonstrations? |
| **Tuesday**<br>Aggregate | [Self-Consistency](https://arxiv.org/abs/2203.11171)<br>Can several imperfect paths yield a better answer? |
| **Wednesday**<br>Verify | [Training Verifiers](https://arxiv.org/abs/2110.14168)<br>How does selecting differ from generating? |
| **Thursday**<br>Compress | [Coconut](https://arxiv.org/abs/2412.06769)<br>What survives when intermediate states are continuous? |
| **Friday**<br>Iterate | [Recurrent Depth](https://arxiv.org/abs/2502.05171)<br>What does extra hidden computation buy? |

**Before the route:** [Few-shot CoT summary](summaries/Chain-of-Thought%20Prompting.md). **After it:** [Verification and search](categories/reasoning.md#-verification--search) · [Test-time compute](categories/reasoning.md#%EF%B8%8F-test-time-compute).

</details>

*Selections are dated and refreshed when there is something worth recommending; there is no daily or weekly publishing schedule.*

---

## [📚 Must-Read Papers (Hall of Fame)](categories/hall-of-fame.md)

> 🏛️ **Established works with lasting influence.** Promising new breakthroughs belong in the main categories while their influence develops.

| Paper and resources | Why read it |
| :-- | :-- |
| 🏗️ **Attention Is All You Need** · 2017<br>[Paper](https://arxiv.org/abs/1706.03762) · [Summary](summaries/Attention%20Is%20All%20You%20Need%20.md) | Understand self-attention, parallel training and the Transformer’s encoder–decoder design. |
| 🚀 **Language Models are Few-Shot Learners** · 2020<br>[Paper](https://arxiv.org/abs/2005.14165) · [Summary](summaries/GPT-3%20Language%20Models%20are%20Few-Shot%20Learners.md) | Separate pretraining scale from adapting a task through prompt examples. |
| 🧮 **Chain-of-Thought Prompting** · 2022<br>[Paper](https://arxiv.org/abs/2201.11903) · [Summary](summaries/Chain-of-Thought%20Prompting.md) | See what worked demonstrations change—and what explanations cannot certify. |
| 🎯 **InstructGPT** · 2022<br>[Paper](https://arxiv.org/abs/2203.02155) · [Summary](summaries/RLHF%20Training%20with%20Human%20Feedback.md) | Follow demonstrations → reward modeling → policy optimization. |
| 🛡️ **Constitutional AI** · 2022<br>[Paper](https://arxiv.org/abs/2212.08073) · [Summary](summaries/Constitutional%20AI%20Harmlessness%20from%20AI%20Feedback.md) | Understand AI harmlessness feedback alongside human helpfulness labels. |

[**View all 46 Hall of Fame works →**](categories/hall-of-fame.md)

---

## 🗂️ Browse by Category

**Looking for something specific?** Choose the question closest to your work.

**📋 [All Papers (Chronological)](categories/all-papers.md)** · **148 unique works · 2000–2026**

<table>
<tr>
<td width="50%" valign="top">

### [🏗️ Model Architectures](categories/architectures.md)

How should a language model be built?

Transformers · recurrent depth · state spaces · MoE<br>
**36 works**

</td>
<td width="50%" valign="top">

### [🧮 Reasoning & Agents](categories/reasoning.md)

How should it reason, search and act?

Prompting · verification · latent reasoning · tools<br>
**23 works**

</td>
</tr>
<tr>
<td width="50%" valign="top">

### [⚡ Efficiency & Scaling](categories/efficiency.md)

Where can compute and memory be saved?

Quantization · pruning · attention · training systems<br>
**15 works**

</td>
<td width="50%" valign="top">

### [🎯 Training & Alignment](categories/training.md)

What signals should shape its behavior?

Pretraining · preferences · adaptation · self-training<br>
**33 works**

</td>
</tr>
<tr>
<td width="50%" valign="top">

### [🎨 Multimodal Models](categories/multimodal.md)

How do language and visual representations meet?

Vision–language · image generation · video<br>
**18 works**

</td>
<td width="50%" valign="top">

### [📚 RAG & Knowledge](categories/rag.md)

How should it access information beyond its weights?

Retrieval · long context · memory · recursive access<br>
**17 works**

</td>
</tr>
<tr>
<td width="50%" valign="top">

### [🛡️ Safety & Security](categories/safety.md)

Which failure modes survive our defenses?

Attacks · engineered backdoors · safety evaluation<br>
**7 works**

</td>
<td width="50%" valign="top">

### [🔬 Analysis & Theory](categories/analysis.md)

What does the evidence actually tell us?

Circuits · scaling · evaluation · critical analysis<br>
**22 works**

</td>
</tr>
</table>

*A useful cross-list appears in each relevant category but counts once in the complete index. Counts include curated papers, reports and author research resources.*

---

## 📈 Research Trends Dashboard

**A map for your next reading, selected 10 October 2026.** Follow a question across methods, then examine how the result was measured.

```mermaid
flowchart TD
    Q[Choose a question]
    Q --> R[Reasoning]
    Q --> K[Knowledge]
    Q --> C[Resources]
    R --> V["Generate<br/>Aggregate<br/>Verify"]
    K --> M["Retrieve<br/>Retain<br/>Inspect"]
    C --> S["Experts<br/>Memory<br/>Kernels"]
    V --> E[Evaluate assumptions and limits]
    M --> E
    S --> E
    E --> A[Study failure modes]
```

| Route | Compare, then question |
| :-- | :-- |
| **Reasoning** | [Prompting](categories/reasoning.md#-chain-of-thought-reasoning) → [verification](categories/reasoning.md#-verification--search) → [latent states](categories/reasoning.md#-latent-reasoning)<br>Was the gain from training, sampling, selection or extra compute? |
| **Knowledge** | [Retrieval](categories/rag.md#-rag-foundations) → [context](categories/rag.md#-long-context) → [memory](categories/rag.md#-memory-systems)<br>Was the evidence available, retrieved and used? |
| **Resources** | [MoE](categories/architectures.md#-mixture-of-experts) → [efficiency](categories/efficiency.md)<br>Were data, active parameters, hardware and budgets comparable? |

The map expresses reading relationships, not measured field growth or a forecast. For failure analysis, continue with [evaluation](categories/analysis.md#-evaluation) and [safety](categories/safety.md).

---

## 🤝 Contributing

<div align="center">

### [Suggest the next paper worth reading](CONTRIBUTING.md)

[![Submit Paper](https://img.shields.io/badge/Submit_Paper-Open_the_form-blue?style=for-the-badge&logo=github)](https://github.com/puneet-chandna/awesome-LLM-papers/issues/new?template=new-paper.yml)

Bring a primary source, the distinct contribution, why a reader benefits, and an important limitation.

**Older papers welcome. Corrections welcome. Quality over quantity.**

</div>

---

<div align="center">

[⬆ Back to Top](#awesome-llm-papers-)

Made with ❤️ for the AI Research Community

Last updated: **10 October 2026** · Research cutoff: **10 October 2026**

[![Follow on Twitter](https://img.shields.io/twitter/follow/puneet_chandna_?style=social)](https://x.com/puneet_chandna_)
[![GitHub followers](https://img.shields.io/github/followers/puneet-chandna?style=social)](https://github.com/puneet-chandna)

</div>
