# 🎯 Training & Alignment: Methods for Building Better LLMs

<div align="center">

[![Awesome](https://awesome.re/badge-flat2.svg)](https://awesome.re)
[![Works](https://img.shields.io/badge/Works-33-blue.svg)](all-papers.md)
[![Years](https://img.shields.io/badge/Years-2000--2026-green.svg)](all-papers.md)
[![License: CC0](https://img.shields.io/badge/License-CC0-yellow.svg)](../LICENSE)
[![PRs Welcome](https://img.shields.io/badge/PRs-welcome-brightgreen.svg?style=flat-square)](../CONTRIBUTING.md)

### A curated collection of papers on training methodologies, alignment techniques, and fine-tuning strategies

_From RLHF to parameter-efficient methods, these papers define how we train and align modern language models._

</div>

---

## 📑 Table of Contents

- [🎯 RLHF & Alignment](#-rlhf--alignment)
- [🔧 Parameter-Efficient Fine-Tuning (PEFT)](#-parameter-efficient-fine-tuning-peft)
- [📚 Instruction Tuning](#-instruction-tuning)
- [🔄 Self-Improvement](#-self-improvement)
- [🆕 Recent Breakthroughs](#-recent-breakthroughs)
- [🏗️ Pretraining & Training Systems](#%EF%B8%8F-pretraining--training-systems)

---

## 🎯 RLHF & Alignment

### 📄 [Deep reinforcement learning from human preferences](https://arxiv.org/abs/1706.03741) ![Hall of Fame](https://img.shields.io/badge/⭐-Hall%20of%20Fame-ff1493?style=flat&labelColor=000000)

**Authors:** Paul Christiano et al.<br>
**Contribution:** `🏗️ Foundation`

> Learns **reward models from human comparisons of trajectory segments** and uses them to train deep-RL agents. A foundational preference-learning demonstration in simulated control/Atari, providing lineage for later language-model RLHF rather than originating all human-feedback learning.

---

### 📄 [Training language models to follow instructions with human feedback](https://arxiv.org/abs/2203.02155) ![Hall of Fame](https://img.shields.io/badge/⭐-Hall%20of%20Fame-ff1493?style=flat&labelColor=000000)

**Authors:** Long Ouyang et al.<br>
**Contribution:** `🧑‍🏫 Instruction Following`

> Trains **InstructGPT** through human demonstrations, preference reward modeling and PPO, with a pretraining-mix variant. Labelers preferred a 1.3B aligned model to 175B GPT-3 on the tested prompt distribution; this is not universal capability superiority. [Detailed summary](../summaries/RLHF%20Training%20with%20Human%20Feedback.md).

---

### 📄 [Direct Preference Optimization: Your Language Model is Secretly a Reward Model](https://arxiv.org/abs/2305.18290) ![Hall of Fame](https://img.shields.io/badge/⭐-Hall%20of%20Fame-ff1493?style=flat&labelColor=000000)

**Authors:** Rafael Rafailov et al.<br>
**Contribution:** `⚡ Simplified Alignment`

> Derives an **offline preference objective through the policy’s implicit reward relation**, avoiding a separately fitted reward model and online RL loop. DPO simplifies preference training in studied settings; data quality, reference policy and distribution shift still matter.

---

### 📄 [Constitutional AI: Harmlessness from AI Feedback](https://arxiv.org/abs/2212.08073) ![Hall of Fame](https://img.shields.io/badge/⭐-Hall%20of%20Fame-ff1493?style=flat&labelColor=000000)

**Authors:** Yuntao Bai et al. (Anthropic)<br>
**Contribution:** `🛡️ Scalable Safety`

> Uses constitutional principles for **critique/revision and AI harmlessness preferences**, while retaining human helpfulness feedback. The reported preference trade-off is an alignment experiment, not a proof of harmlessness. [Detailed summary](../summaries/Constitutional%20AI%20Harmlessness%20from%20AI%20Feedback.md).

---

### 📄 [Learning to Summarize from Human Feedback](https://arxiv.org/abs/2009.01325)

**Authors:** Stiennon et al.<br>
**Contribution:** `🧑‍🏫 Preference Learning`

> Trains a **summary preference model** from human comparisons, then optimizes a summarizer against it. A concrete precursor to instruction-oriented RLHF; the experiments concern summarization and selected labelers, not all forms of human intent.

---

### 📄 [Scaling Laws for Reward Model Overoptimization](https://arxiv.org/abs/2210.10760)

**Authors:** Gao, Schulman & Hilton<br>
**Contribution:** `⚠️ Proxy Optimization`

> See the main entry in [Analysis](analysis.md) for the method, evidence and limitations.

---

### 📄 [Let's Verify Step by Step](https://arxiv.org/abs/2305.20050)

**Authors:** Lightman et al.<br>
**Contribution:** `✅ Process Supervision`

> See the main entry in [Reasoning](reasoning.md) for the method, evidence and limitations.

---

## 🔧 Parameter-Efficient Fine-Tuning (PEFT)

### 📄 [LoRA: Low-Rank Adaptation of Large Language Models](https://arxiv.org/abs/2106.09685) ![Hall of Fame](https://img.shields.io/badge/⭐-Hall%20of%20Fame-ff1493?style=flat&labelColor=000000)

**Authors:** Edward J. Hu et al.<br>
**Contribution:** `💡 Efficient Adaptation`

> Freezes pretrained weights and trains **low-rank updates** to selected weight matrices. LoRA reduces trainable parameters and optimizer memory; the reduction depends on rank, model and target layers, while the base model still needs to fit in memory.

---

### 📄 [Prefix-Tuning: Optimizing Continuous Prompts for Generation](https://arxiv.org/abs/2101.00190)

**Authors:** Xiang Lisa Li et al.<br>
**Contribution:** `🎛️ Soft Prompts`

> Learns **continuous prefixes of activations** while keeping the pretrained model frozen. Prefix-tuning makes a small adaptation footprint practical for studied generation tasks; the reported parameter fraction and transfer quality depend on task and model.

---

### 📄 [QLoRA: Efficient Finetuning of Quantized LLMs](https://arxiv.org/abs/2305.14314)

**Authors:** Tim Dettmers et al.<br>
**Contribution:** `🗜️ Memory Efficiency`

> Combined 4-bit quantization with LoRA to enable **fine-tuning of 65B parameter models on a single 48GB GPU**. QLoRA introduced innovations like 4-bit NormalFloat quantization and Double Quantization, reducing memory usage without sacrificing performance. This democratized fine-tuning of large models, making it accessible to researchers without massive compute resources.

---

## 📚 Instruction Tuning

### 📄 [Finetuned Language Models Are Zero-Shot Learners](https://arxiv.org/abs/2109.01652) ![Hall of Fame](https://img.shields.io/badge/⭐-Hall%20of%20Fame-ff1493?style=flat&labelColor=000000)

**Authors:** Jason Wei et al. (Google)<br>
**Contribution:** `🎯 Task Generalization`

> Fine-tunes a language model on **tasks expressed through natural-language instructions** and evaluates held-out task families. FLAN makes instruction tuning a generalization strategy; task mixture, holdout design and base-model capability determine the observed transfer.

---

### 📄 [Scaling Instruction-Finetuned Language Models](https://arxiv.org/abs/2210.11416)

**Authors:** Hyung Won Chung et al. (Google)<br>
**Contribution:** `📈 Scaling Instructions`

> Scaled instruction tuning to 1,800+ tasks and demonstrated that **instruction tuning benefits scale with both model size and number of tasks**. The resulting Flan-T5 and Flan-PaLM models showed substantial improvements over their base versions, with Flan-PaLM achieving state-of-the-art on many benchmarks and outperforming larger models.

---

### 📄 [Stanford Alpaca: An Instruction-following LLaMA Model](https://github.com/tatsu-lab/stanford_alpaca)

**Authors:** Rohan Taori et al. (Stanford)<br>
**Contribution:** `🦙 Accessible Fine-tuning`

> An **official project resource** demonstrating instruction adaptation of LLaMA using 52K generated examples. Alpaca’s preliminary evaluations and data/fine-tuning cost estimates exclude inherited pretraining; original research-use restrictions and known reliability issues matter.

---

### 📄 [Self-Instruct: Aligning Language Models with Self-Generated Instructions](https://arxiv.org/abs/2212.10560)

**Authors:** Yizhong Wang et al.<br>
**Contribution:** `🔄 Self-Generated Data`

> Bootstraps **instructions, inputs and responses** from a small human-written seed, filters them and fine-tunes on the resulting synthetic data. Self-Instruct provides an influential data-generation recipe; quality depends on the generator, filtering and seed coverage.

---

## 🔄 Self-Improvement

### 📄 [Self-Play Fine-Tuning Converts Weak Language Models to Strong Language Models](https://arxiv.org/abs/2401.01335)

**Authors:** Zixiang Chen et al.<br>
**Contribution:** `♾️ Self-Play`

> Iteratively trains a policy to distinguish **human demonstration responses from its own generated responses**. SPIN reuses a supervised seed dataset; improvements in tested iterations are not evidence of unlimited self-improvement without human data.

---

### 📄 [Self-Rewarding Language Models](https://arxiv.org/abs/2401.10020)

**Authors:** Weizhe Yuan et al.<br>
**Contribution:** `🎯 Self-Reward`

> Uses an **LLM-as-judge to create preference pairs** for iterative DPO. Self-rewarding models study a coupled generator/judge loop, which still inherits the pretrained model, seed training and evaluation distribution; judging errors can reinforce weak preferences.

---

### 📄 [Direct Language Model Alignment from Online AI Feedback](https://arxiv.org/abs/2402.04792)

**Authors:** Shangmin Guo et al.<br>
**Contribution:** `🔄 Online Learning`

> Generates **online preference comparisons with an AI judge** while adapting the language model. OAIF studies refreshing feedback rather than relying entirely on a fixed preference dataset; gains depend on the judge, sampling distribution and evaluated training setup.

---

### 📄 [STaR: Bootstrapping Reasoning With Reasoning](https://arxiv.org/abs/2203.14465)

**Authors:** Zelikman et al.<br>
**Contribution:** `🔄 Rationale Bootstrapping`

> Iterates **answer-filtered rationale generation and fine-tuning**, using known answers to rationalize failed attempts. Each round restarts fine-tuning from the original base model; seed rationales and correct-answer access distinguish this from autonomous learning without supervision.

---

### 📄 [Absolute Zero: Reinforced Self-play Reasoning with Zero Data](https://arxiv.org/abs/2505.03335)

**Authors:** Andrew Zhao et al.<br>
**Contribution:** `🔄 Executor-Guided Self-Play`

> Uses an executor to validate **self-proposed coding reasoning tasks** and trains through reinforced self-play. “Zero data” refers to no external task examples in this stage, not the removal of pretrained models, compute or execution-based assumptions.

---

## 🆕 Recent Breakthroughs

### 📄 [ORPO: Monolithic Preference Optimization without Reference Model](https://arxiv.org/abs/2403.07691)

**Authors:** Jiwoo Hong, Noah Lee and James Thorne<br>
**Contribution:** `🎯 Simplified Training`

> Combines a **supervised likelihood objective with an odds-ratio preference penalty** in one reference-free training stage. ORPO offers a compact alignment recipe; the evaluated comparisons depend on the base model, data and preference-training configuration.

---

### 📄 [KTO: Model Alignment as Prospect Theoretic Optimization](https://arxiv.org/abs/2402.01306)

**Authors:** Kawin Ethayarajh et al.<br>
**Contribution:** `📊 Human-Aligned Loss`

> Derives **Kahneman–Tversky Optimization**, a utility-inspired objective that uses desirable/undesirable labels rather than paired preferences. KTO makes a different feedback format practical; loss choice and gains depend on the training setting rather than a universal human-value model.

---

### 📄 [SimPO: Simple Preference Optimization with a Reference-Free Reward](https://arxiv.org/abs/2405.14734)

**Authors:** Yu Meng et al.<br>
**Contribution:** `⚡ Reference-Free Alignment`

> Optimizes preferences using **length-normalized sequence log probabilities and a target reward margin**, without a reference model. SimPO offers a useful comparison to DPO under the authors’ training/evaluation setups; those results do not establish universal stability or default adoption.

---

### 📄 [Close the Loop: Synthesizing Infinite Tool-Use Data via Multi-Agent Role-Playing](https://arxiv.org/abs/2512.23611)

**Authors:** Yuwen Li et al.<br>
**Contribution:** `🔧 Tool-Use Training` `🤖 Multi-Agent Synthesis`

> Introduces **InfTool**, combining synthetic API trajectories with gated-reward GRPO. Qwen2.5-32B scores 19.8% → 70.9% on the authors’ BFCL V3 setup (51.1 percentage points); the iterative loop adds 65.3% → 70.9% over SFT. Data generation still depends on inherited models and trajectory judges.

---

### 📄 [IQuest-Coder-V1 Technical Report](https://github.com/IQuestLab/IQuest-Coder-V1/blob/main/papers/IQuest_Coder_Technical_Report.pdf)

**Authors:** IQuest Coder Team / Yang et al.<br>
**Contribution:** `🔄 Code-Flow Training` `🎯 Bifurcated Post-Training`

> An **official technical report** on repository-evolution Code-Flow training and separate Instruct/Thinking post-training. The later paper reports 76.2% SWE-bench Verified for the 40B-Loop variants and 71.2% for plain 40B-Thinking; these are model-plus-agent evaluations, not an isolated causal effect of Code-Flow.

---

## 🏗️ Pretraining & Training Systems

### 📄 [A Neural Probabilistic Language Model](https://jmlr.org/papers/v3/bengio03a.html) ![Hall of Fame](https://img.shields.io/badge/⭐-Hall%20of%20Fame-ff1493?style=flat&labelColor=000000)

**Authors:** Bengio, Ducharme & Vincent (NIPS 2000); with Jauvin (JMLR 2003)<br>
**Contribution:** `🧠 Learned Word Representations`

> See the main entry in [Architectures](architectures.md) for the method, evidence and limitations.

---

### 📄 [Outrageously Large Neural Networks: The Sparsely-Gated Mixture-of-Experts Layer](https://arxiv.org/abs/1701.06538) ![Hall of Fame](https://img.shields.io/badge/⭐-Hall%20of%20Fame-ff1493?style=flat&labelColor=000000)

**Authors:** Shazeer et al.<br>
**Contribution:** `🧩 Conditional Computation`

> See the main entry in [Architectures](architectures.md) for the method, evidence and limitations.

---

### 📄 [Deep Contextualized Word Representations](https://arxiv.org/abs/1802.05365) ![Hall of Fame](https://img.shields.io/badge/⭐-Hall%20of%20Fame-ff1493?style=flat&labelColor=000000)

**Authors:** Peters et al.<br>
**Contribution:** `🧠 Contextual Representations`

> **ELMo** combines internal layers of a bidirectional language model into context-dependent word representations for downstream systems. Read it as a bridge from static embeddings to contextual pretraining, not the first contextual representation method; earlier public OpenReview posting predates NAACL 2018.

---

### 📄 [Pythia: A Suite for Analyzing Large Language Models Across Training and Scaling](https://arxiv.org/abs/2304.01373)

**Authors:** Biderman et al.<br>
**Contribution:** `🔬 Controlled Model Suite`

> See the main entry in [Analysis](analysis.md) for the method, evidence and limitations.

---

### 📄 [DeepSeek-V3 Technical Report](https://arxiv.org/abs/2412.19437)

**Authors:** DeepSeek-AI<br>
**Contribution:** `🧩 Sparse Model Systems`

> See the main entry in [Architectures](architectures.md) for the method, evidence and limitations.

---

### 📄 [s1: Simple Test-Time Scaling](https://arxiv.org/abs/2501.19393)

**Authors:** Muennighoff et al.<br>
**Contribution:** `⏱️ Budget Forcing`

> See the main entry in [Reasoning](reasoning.md) for the method, evidence and limitations.

---

### 📄 [Large Language Diffusion Models](https://arxiv.org/abs/2502.09992)

**Authors:** Nie et al.<br>
**Contribution:** `🌫️ Masked Diffusion`

> See the main entry in [Architectures](architectures.md) for the method, evidence and limitations.

---

### 📄 [OLMo: Accelerating the Science of Language Models](https://arxiv.org/abs/2402.00838) ![Hall of Fame](https://img.shields.io/badge/⭐-Hall%20of%20Fame-ff1493?style=flat&labelColor=000000)

**Authors:** Dirk Groeneveld et al. (AI2)<br>
**Contribution:** `🔬 Open Research Stack`

> Releases **OLMo weights, training code, data and evaluation tooling** to support open language-model research. Its central contribution is an inspectable research stack; benchmark comparisons are competitive within the reported models and setups.

---

### 📄 [Megatron-LM: Training Multi-Billion Parameter Language Models Using Model Parallelism](https://arxiv.org/abs/1909.08053) ![Hall of Fame](https://img.shields.io/badge/⭐-Hall%20of%20Fame-ff1493?style=flat&labelColor=000000)

**Authors:** Mohammad Shoeybi et al.<br>
**Contribution:** `⚙️ Tensor Parallelism`

> See the main entry in [Efficiency](efficiency.md) for the method, evidence and limitations.

---

<div align="center">

### 🌟 Contributing

Feel free to submit PRs to add more training and alignment papers or improve existing entries!

### 📜 License

This repository is licensed under CC0 License.

### 🙏 Acknowledgments

Thanks to all researchers advancing the science of training and aligning language models.

---

⭐ If you find this repository helpful, please consider giving it a star!

</div>
