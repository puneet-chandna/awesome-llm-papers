# 🧠 Reasoning & Agents: From Chain-of-Thought to Autonomous Systems

<div align="center">

[![Awesome](https://awesome.re/badge-flat2.svg)](https://awesome.re)
[![Works](https://img.shields.io/badge/Works-23-blue.svg)](all-papers.md)
[![Years](https://img.shields.io/badge/Years-2021--2026-green.svg)](all-papers.md)
[![License: CC0](https://img.shields.io/badge/License-CC0-yellow.svg)](../LICENSE)
[![PRs Welcome](https://img.shields.io/badge/PRs-welcome-brightgreen.svg?style=flat-square)](../CONTRIBUTING.md)

### A curated collection of papers on reasoning techniques and autonomous AI agents

_From prompting strategies that unlock step-by-step thinking to systems that can plan, use tools, and act autonomously._

</div>

---

## 📑 Table of Contents

- [💭 Chain-of-Thought Reasoning](#-chain-of-thought-reasoning)
- [🤖 Agent Systems](#-agent-systems)
- [🆕 Recent Breakthroughs](#-recent-breakthroughs)
- [✅ Verification & Search](#-verification--search)
- [⏱️ Test-Time Compute](#%EF%B8%8F-test-time-compute)
- [🌀 Latent Reasoning](#-latent-reasoning)
- [💻 Code Models](#-code-models)

---

## 💭 Chain-of-Thought Reasoning

### 📄 [Chain-of-Thought Prompting Elicits Reasoning in Large Language Models](https://arxiv.org/abs/2201.11903) ![Hall of Fame](https://img.shields.io/badge/⭐-Hall%20of%20Fame-ff1493?style=flat&labelColor=000000)

**Authors:** Jason Wei et al. (Google)<br>
**Contribution:** `🧮 Reasoning`

> Shows that **worked reasoning demonstrations** can improve arithmetic, commonsense and symbolic tasks without weight updates. Distinguish this few-shot method from Kojima et al.’s zero-shot reasoning instruction; extra tokens cost inference compute and explanations need not be faithful. [Detailed summary](../summaries/Chain-of-Thought%20Prompting.md).

---

### 📄 [Tree of Thoughts: Deliberate Problem Solving with Large Language Models](https://arxiv.org/abs/2305.10601)

**Authors:** Shunyu Yao et al.<br>
**Contribution:** `🌳 Structured Reasoning`

> Searches a **tree of candidate thoughts**, using evaluation and backtracking in tasks such as Game24 and mini crosswords. Tree of Thoughts makes search policy explicit; additional model calls increase compute and neither search nor self-evaluation certifies correctness.

---

### 📄 [Graph of Thoughts: Solving Elaborate Problems with Large Language Models](https://arxiv.org/abs/2308.09687)

**Authors:** Maciej Besta et al.<br>
**Contribution:** `🕸️ Graph Reasoning`

> Organizes generated thoughts as a **graph**, supporting aggregation, refinement and reuse of intermediate solutions. Graph of Thoughts studies tasks including sorting and set operations; gains depend on graph design and additional calls to generation/evaluation models.

---

### 📄 [Self-Consistency Improves Chain of Thought Reasoning in Language Models](https://arxiv.org/abs/2203.11171) ![Hall of Fame](https://img.shields.io/badge/⭐-Hall%20of%20Fame-ff1493?style=flat&labelColor=000000)

**Authors:** Wang et al.<br>
**Contribution:** `🗳️ Answer Aggregation`

> Samples **diverse reasoning paths and aggregates final answers** rather than using a single greedy chain. A foundational test-time-compute baseline; voting adds generation cost and is not a correctness certificate.

---

### 📄 [Large Language Models are Zero-Shot Reasoners](https://arxiv.org/abs/2205.11916) ![Hall of Fame](https://img.shields.io/badge/⭐-Hall%20of%20Fame-ff1493?style=flat&labelColor=000000)

**Authors:** Kojima et al.<br>
**Contribution:** `💭 Zero-Shot CoT`

> Uses a **reasoning instruction followed by answer extraction** without worked demonstrations. This separates zero-shot CoT from Wei et al.’s few-shot method; gains vary with model and task, and generated explanations may be wrong.

---

## 🤖 Agent Systems

### 📄 [ReAct: Synergizing Reasoning and Acting in Language Models](https://arxiv.org/abs/2210.03629)

**Authors:** Shunyu Yao et al.<br>
**Contribution:** `🔄 Reasoning + Action`

> Interleaves **reasoning traces, actions and observations** in knowledge and decision tasks. ReAct shows how tool/environment feedback can guide subsequent steps; performance depends on tools, demonstrations and task, with additional interaction costs.

---

### 📄 [Reflexion: Language Agents with Verbal Reinforcement Learning](https://arxiv.org/abs/2303.11366)

**Authors:** Noah Shinn et al.<br>
**Contribution:** `🪞 Self-Reflection`

> Enabled agents to **learn from their mistakes through verbal self-reflection**. After failing a task, Reflexion agents generate natural language feedback about what went wrong and store these reflections in memory. On subsequent attempts, they use this accumulated experience to avoid past errors, achieving significant improvements without any weight updates—a form of in-context reinforcement learning.

---

### 📄 [Toolformer: Language Models Can Teach Themselves to Use Tools](https://arxiv.org/abs/2302.04761)

**Authors:** Timo Schick et al.<br>
**Contribution:** `🔧 Tool Use`

> Uses a few API demonstrations to seed **self-supervised tool-call generation and filtering**, then trains a model to use the retained calls. Toolformer explains when external tools help prediction; its constrained API suite differs from arbitrary autonomous tool use.

---

### 📄 [Recursive Language Models](https://arxiv.org/abs/2512.24601)

**Authors:** Zhang, Kraska & Khattab<br>
**Contribution:** `🔁 Context as Environment`

> See the main entry in [Rag](rag.md) for the method, evidence and limitations.

---

## 🆕 Recent Breakthroughs

### 📄 [DeepSeek-R1: Incentivizing Reasoning Capability in LLMs via Reinforcement Learning](https://arxiv.org/abs/2501.12948) ![Hall of Fame](https://img.shields.io/badge/⭐-Hall%20of%20Fame-ff1493?style=flat&labelColor=000000)

**Authors:** DeepSeek-AI et al.<br>
**Contribution:** `🧠 Advanced Reasoning`

> Studies reasoning-oriented reinforcement learning: **R1-Zero uses rule-based final-answer accuracy and format rewards**, rather than labels on each intermediate step. R1 adds cold-start and further training stages; verification, readability and reward design remain important limitations.

---

### 📄 [DeepSeekMath: Pushing the Limits of Mathematical Reasoning in Open Language Models](https://arxiv.org/abs/2402.03300) ![Hall of Fame](https://img.shields.io/badge/⭐-Hall%20of%20Fame-ff1493?style=flat&labelColor=000000)

**Authors:** Zhihong Shao et al.<br>
**Contribution:** `🧮 Mathematical Reasoning`

> Presents DeepSeekMath and **Group Relative Policy Optimization (GRPO)**, which estimates relative advantages from groups of sampled solutions without a separate critic. Its math results depend on training and inference setup; avoid treating the model as the first open system near GPT-4 on every math benchmark.

---

### 📄 [OpenAI o1 System Card](https://arxiv.org/abs/2412.16720)

**Authors:** OpenAI (Aaron Jaech et al.)<br>
**Contribution:** `🎯 Reasoning at Scale`

> An **official system card** documenting o1’s capabilities, safety evaluations and mitigations. It is useful for examining safety evidence around reasoning models; the card does not disclose a reproducible training recipe or establish a general test-time scaling law.

---

### 📄 [IQuest-Coder-V1 Technical Report](https://github.com/IQuestLab/IQuest-Coder-V1/blob/main/papers/IQuest_Coder_Technical_Report.pdf)

**Authors:** IQuest Coder Team / Yang et al.<br>
**Contribution:** `🔄 Code-Flow Training` `🎯 Bifurcated Post-Training`

> An **official technical report** on repository-evolution Code-Flow training and separate Instruct/Thinking post-training. The later paper reports 76.2% SWE-bench Verified for the 40B-Loop variants and 71.2% for plain 40B-Thinking; these are model-plus-agent evaluations, not an isolated causal effect of Code-Flow.

---

### 📄 [Context as a Tool: Context Management for Long-Horizon SWE-Agents](https://arxiv.org/abs/2512.22087)

**Authors:** Shukai Liu et al.<br>
**Contribution:** `🧠 Context Management` `🤖 SWE Agents`

> Makes **context management a callable action** for long-horizon software agents. Qwen2.5-Coder-32B/SWE-Compressor reaches 57.6% Pass@1 on SWE-bench Verified in OpenHands, versus 49.8% ReAct and 53.8% threshold compression in that setup; results concern the combined agent, model and context budget.

---

### 📄 [STaR: Bootstrapping Reasoning With Reasoning](https://arxiv.org/abs/2203.14465)

**Authors:** Zelikman et al.<br>
**Contribution:** `🔄 Rationale Bootstrapping`

> See the main entry in [Training](training.md) for the method, evidence and limitations.

---

### 📄 [Absolute Zero: Reinforced Self-play Reasoning with Zero Data](https://arxiv.org/abs/2505.03335)

**Authors:** Andrew Zhao et al.<br>
**Contribution:** `🔄 Executor-Guided Self-Play`

> See the main entry in [Training](training.md) for the method, evidence and limitations.

---

## ✅ Verification & Search

### 📄 [Training Verifiers to Solve Math Word Problems](https://arxiv.org/abs/2110.14168) ![Hall of Fame](https://img.shields.io/badge/⭐-Hall%20of%20Fame-ff1493?style=flat&labelColor=000000)

**Authors:** Cobbe et al.<br>
**Contribution:** `✅ GSM8K & Verifiers`

> Introduces **GSM8K and learned verification** to select among sampled math solutions. It separates proposing an answer from ranking candidates; gains require sampling compute, and larger search can exploit verifier errors.

---

### 📄 [Let's Verify Step by Step](https://arxiv.org/abs/2305.20050)

**Authors:** Lightman et al.<br>
**Contribution:** `✅ Process Supervision`

> Compares **process and outcome supervision** for ranking math solutions and releases PRM800K step labels. The headline MATH result uses best-of-many selection with a fixed generator, not one-sample accuracy or generator RL; annotation and search budgets matter.

---

## ⏱️ Test-Time Compute

### 📄 [s1: Simple Test-Time Scaling](https://arxiv.org/abs/2501.19393)

**Authors:** Muennighoff et al.<br>
**Contribution:** `⏱️ Budget Forcing`

> Distills a small curated reasoning set into a pretrained model and uses **budget forcing**, including “Wait” continuations, to control test-time reasoning length. A clean study of inference budget; the short fine-tuning run excludes base-model and teacher compute.

---

### 📄 [Scaling LLM Test-Time Compute Optimally can be More Effective than Scaling Model Parameters](https://arxiv.org/abs/2408.03314)

**Authors:** Snell et al.<br>
**Contribution:** `⚖️ Compute Allocation`

> Studies **difficulty-dependent allocation** between answer revision and verifier-guided search. It makes test-time scaling an allocation problem rather than “think longer”; comparisons depend on tasks and budgets, and exclude difficulty-estimation cost.

---

## 🌀 Latent Reasoning

### 📄 [Training Large Language Models to Reason in a Continuous Latent Space](https://arxiv.org/abs/2412.06769)

**Authors:** Hao et al.<br>
**Contribution:** `🌀 Continuous Reasoning`

> **Coconut** feeds continuous hidden states back as input embeddings and trains through a curriculum replacing verbal reasoning steps. Its structured-search gains coexist with weaker GSM8K performance than CoT; latent reasoning is not a universal replacement for language traces.

---

### 📄 [Scaling up Test-Time Compute with Latent Reasoning: A Recurrent Depth Approach](https://arxiv.org/abs/2502.05171)

**Authors:** Geiping et al.<br>
**Contribution:** `🌀 Recurrent Depth`

> See the main entry in [Architectures](architectures.md) for the method, evidence and limitations.

---

## 💻 Code Models

### 📄 [Evaluating Large Language Models Trained on Code](https://arxiv.org/abs/2107.03374) ![Hall of Fame](https://img.shields.io/badge/⭐-Hall%20of%20Fame-ff1493?style=flat&labelColor=000000)

**Authors:** Mark Chen et al. (OpenAI)<br>
**Contribution:** `💻 Functional Code Evaluation`

> Studies **Codex code generation** and introduces HumanEval with execution-based functional correctness and sampling metrics. It makes candidate sampling and test-based evaluation central; passing limited tests differs from proving program correctness or broad reasoning ability.

---

<div align="center">

### 🌟 Contributing

Feel free to submit PRs to add more reasoning and agent papers or improve existing entries!

### 📜 License

This repository is licensed under CC0 License.

### 🙏 Acknowledgments

Thanks to all the researchers pushing the boundaries of AI reasoning and autonomous systems.

---

⭐ If you find this repository helpful, please consider giving it a star!

</div>
