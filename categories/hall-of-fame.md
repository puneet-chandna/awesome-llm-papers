# 🏆 Hall of Fame: Foundational LLM Papers

<div align="center">

[![Awesome](https://awesome.re/badge-flat2.svg)](https://awesome.re)
[![Works](https://img.shields.io/badge/Works-46-blue.svg)](all-papers.md)
[![Years](https://img.shields.io/badge/Years-2000--2025-green.svg)](all-papers.md)

**Established works with lasting influence. Promising new breakthroughs remain in the main categories until their influence is clearer.**

</div>

[2025](#%EF%B8%8F-2025) • [2024](#%EF%B8%8F-2024) • [2023](#%EF%B8%8F-2023) • [2022](#%EF%B8%8F-2022) • [2021](#%EF%B8%8F-2021) • [2020](#%EF%B8%8F-2020) • [2019](#%EF%B8%8F-2019) • [2018](#%EF%B8%8F-2018) • [2017](#%EF%B8%8F-2017) • [2000](#%EF%B8%8F-2000)

Dates follow the earliest public paper/resource record verified in this audit; venue and revision years can differ. NNLM includes its NIPS 2000 and expanded JMLR 2003 versions as one work. ELMo’s 2017 date follows the authors’ stated OpenReview appearance.

---

## 🏛️ 2025

### 📄 [DeepSeek-R1: Incentivizing Reasoning Capability in LLMs via Reinforcement Learning](https://arxiv.org/abs/2501.12948) ![Hall of Fame](https://img.shields.io/badge/⭐-Hall%20of%20Fame-ff1493?style=flat&labelColor=000000)

**Authors:** DeepSeek-AI et al.<br>
**Contribution:** `🧠 Advanced Reasoning`

> Studies reasoning-oriented reinforcement learning: **R1-Zero uses rule-based final-answer accuracy and format rewards**, rather than labels on each intermediate step. R1 adds cold-start and further training stages; verification, readability and reward design remain important limitations.

---

## 🏛️ 2024

### 📄 [Titans: Learning to Memorize at Test Time](https://arxiv.org/abs/2501.00663) ![Hall of Fame](https://img.shields.io/badge/⭐-Hall%20of%20Fame-ff1493?style=flat&labelColor=000000)

**Authors:** Ali Behrouz, Peilin Zhong, Vahab Mirrokni<br>
**Contribution:** `🧠 Neural Memory`

> Combines local attention with **gradient-updated neural memory**, using surprise-sensitive updates, momentum and decay. MAC, MAG and MAL offer different integrations; long-context demonstrations do not establish perfect recall or a universal winning variant. [Detailed summary](../summaries/Titans%20Learning%20to%20Memorize%20at%20Test%20Time.md).

---

### 📄 [The Llama 3 Herd of Models](https://arxiv.org/abs/2407.21783) ![Hall of Fame](https://img.shields.io/badge/⭐-Hall%20of%20Fame-ff1493?style=flat&labelColor=000000)

**Authors:** Aaron Grattafiori et al.<br>
**Contribution:** `🦙 Model Systems`

> An **official Llama 3 model-family report** covering models through 405B parameters, 128K context, post-training and safety evaluations. Useful for large-scale model development; released weights do not imply publication of all training data, and multimodal integrations include research experiments.

---

### 📄 [Scaling and evaluating sparse autoencoders](https://arxiv.org/abs/2406.04093) ![Hall of Fame](https://img.shields.io/badge/⭐-Hall%20of%20Fame-ff1493?style=flat&labelColor=000000)

**Authors:** Leo Gao et al. (OpenAI)<br>
**Contribution:** `🔬 Interpretability at Scale`

> Scales **k-sparse autoencoders** and develops evaluation tools for interpreting learned activation features. The study includes a 16M-latent GPT-4 autoencoder trained on 40B tokens, building on earlier k-sparse methods; learned features still have incomplete interpretability and context limitations.

---

### 📄 [DeepSeekMath: Pushing the Limits of Mathematical Reasoning in Open Language Models](https://arxiv.org/abs/2402.03300) ![Hall of Fame](https://img.shields.io/badge/⭐-Hall%20of%20Fame-ff1493?style=flat&labelColor=000000)

**Authors:** Zhihong Shao et al.<br>
**Contribution:** `🧮 Mathematical Reasoning`

> Presents DeepSeekMath and **Group Relative Policy Optimization (GRPO)**, which estimates relative advantages from groups of sampled solutions without a separate critic. Its math results depend on training and inference setup; avoid treating the model as the first open system near GPT-4 on every math benchmark.

---

### 📄 [OLMo: Accelerating the Science of Language Models](https://arxiv.org/abs/2402.00838) ![Hall of Fame](https://img.shields.io/badge/⭐-Hall%20of%20Fame-ff1493?style=flat&labelColor=000000)

**Authors:** Dirk Groeneveld et al. (AI2)<br>
**Contribution:** `🔬 Open Research Stack`

> Releases **OLMo weights, training code, data and evaluation tooling** to support open language-model research. Its central contribution is an inspectable research stack; benchmark comparisons are competitive within the reported models and setups.

---

## 🏛️ 2023

### 📄 [Mamba: Linear-Time Sequence Modeling with Selective State Spaces](https://arxiv.org/abs/2312.00752) ![Hall of Fame](https://img.shields.io/badge/⭐-Hall%20of%20Fame-ff1493?style=flat&labelColor=000000)

**Authors:** Albert Gu and Tri Dao<br>
**Contribution:** `🐍 SSM Architecture`

> Makes **state-space parameters input-dependent** and uses a hardware-aware scan for sequence modeling. Mamba studies selective information propagation with linear sequence scaling; throughput and quality comparisons are tied to the tested models and workloads, with finite-state recall limits.

---

### 📄 [Mistral 7B](https://arxiv.org/abs/2310.06825) ![Hall of Fame](https://img.shields.io/badge/⭐-Hall%20of%20Fame-ff1493?style=flat&labelColor=000000)

**Authors:** Albert Q. Jiang et al.<br>
**Contribution:** `⚡ Model Efficiency`

> Combines **grouped-query attention and sliding-window attention** in the Mistral 7B model. The report compares favorably with Llama 2 13B on its evaluated suite; these architectural ingredients predate Mistral and gains remain benchmark-specific.

---

### 📄 [Llama 2: Open Foundation and Fine-Tuned Chat Models](https://arxiv.org/abs/2307.09288) ![Hall of Fame](https://img.shields.io/badge/⭐-Hall%20of%20Fame-ff1493?style=flat&labelColor=000000)

**Authors:** Hugo Touvron et al. (Meta)<br>
**Contribution:** `🦙 Open-Weight Models`

> An **official Llama 2 report** on pretrained and chat-tuned open-weight models, including preference training and safety evaluations. It broadened research/commercial access under its license; released weights differ from fully disclosed training data.

---

### 📄 [Direct Preference Optimization: Your Language Model is Secretly a Reward Model](https://arxiv.org/abs/2305.18290) ![Hall of Fame](https://img.shields.io/badge/⭐-Hall%20of%20Fame-ff1493?style=flat&labelColor=000000)

**Authors:** Rafael Rafailov et al.<br>
**Contribution:** `⚡ Simplified Alignment`

> Derives an **offline preference objective through the policy’s implicit reward relation**, avoiding a separately fitted reward model and online RL loop. DPO simplifies preference training in studied settings; data quality, reference policy and distribution shift still matter.

---

### 📄 [GPT-4 Technical Report](https://arxiv.org/abs/2303.08774) ![Hall of Fame](https://img.shields.io/badge/⭐-Hall%20of%20Fame-ff1493?style=flat&labelColor=000000)

**Authors:** OpenAI et al.<br>
**Contribution:** `🏆 Multimodal Intelligence`

> Documents **GPT-4**, a model accepting image and text inputs with text outputs, alongside capability and safety evaluations. The report limits disclosure of training and architecture; it should be distinguished from the later GPT-4V product and system card.

---

### 📄 [LLaMA: Open and Efficient Foundation Language Models](https://arxiv.org/abs/2302.13971) ![Hall of Fame](https://img.shields.io/badge/⭐-Hall%20of%20Fame-ff1493?style=flat&labelColor=000000)

**Authors:** Hugo Touvron et al.<br>
**Contribution:** `🦙 Model Access`

> Releases **LLaMA research-access model weights** and studies data-efficient autoregressive training across several sizes. A pivotal access milestone for language-model research; the original research license and partially disclosed data differ from unrestricted open-source reproducibility.

---

## 🏛️ 2022

### 📄 [Constitutional AI: Harmlessness from AI Feedback](https://arxiv.org/abs/2212.08073) ![Hall of Fame](https://img.shields.io/badge/⭐-Hall%20of%20Fame-ff1493?style=flat&labelColor=000000)

**Authors:** Yuntao Bai et al. (Anthropic)<br>
**Contribution:** `🛡️ Scalable Safety`

> Uses constitutional principles for **critique/revision and AI harmlessness preferences**, while retaining human helpfulness feedback. The reported preference trade-off is an alignment experiment, not a proof of harmlessness. [Detailed summary](../summaries/Constitutional%20AI%20Harmlessness%20from%20AI%20Feedback.md).

---

### 📄 [BLOOM: A 176B-Parameter Open-Access Multilingual Language Model](https://arxiv.org/abs/2211.05100) ![Hall of Fame](https://img.shields.io/badge/⭐-Hall%20of%20Fame-ff1493?style=flat&labelColor=000000)

**Authors:** BigScience Workshop et al.<br>
**Contribution:** `🌍 Multilingual Research`

> An **official report on BLOOM**, a 176B multilingual model developed through the BigScience collaboration. It documents collaborative training and access to model artifacts; its Responsible AI License and disclosed resources should be distinguished from unrestricted licensing or full reproducibility.

---

### 📄 [Emergent Abilities of Large Language Models](https://arxiv.org/abs/2206.07682) ![Hall of Fame](https://img.shields.io/badge/⭐-Hall%20of%20Fame-ff1493?style=flat&labelColor=000000)

**Authors:** Jason Wei et al.<br>
**Contribution:** `🪄 Emergence Theory`

> Catalogues **emergent abilities as measured on selected tasks**, where scores appear abruptly with scale. It provides a useful historical framework; metric-dependent interpretations should be read alongside the later Mirage analysis.

---

### 📄 [FlashAttention: Fast and Memory-Efficient Exact Attention with IO-Awareness](https://arxiv.org/abs/2205.14135) ![Hall of Fame](https://img.shields.io/badge/⭐-Hall%20of%20Fame-ff1493?style=flat&labelColor=000000)

**Authors:** Tri Dao et al.<br>
**Contribution:** `💾 IO-Aware Algorithm`

> Computes **exact attention with an IO-aware tiled algorithm**, reducing transfers between GPU memory and on-chip SRAM. FlashAttention’s speed and memory benefits depend on hardware and sequence length; it preserves dense attention rather than changing its quadratic arithmetic.

---

### 📄 [Large Language Models are Zero-Shot Reasoners](https://arxiv.org/abs/2205.11916) ![Hall of Fame](https://img.shields.io/badge/⭐-Hall%20of%20Fame-ff1493?style=flat&labelColor=000000)

**Authors:** Kojima et al.<br>
**Contribution:** `💭 Zero-Shot CoT`

> Uses a **reasoning instruction followed by answer extraction** without worked demonstrations. This separates zero-shot CoT from Wei et al.’s few-shot method; gains vary with model and task, and generated explanations may be wrong.

---

### 📄 [PaLM: Scaling Language Modeling with Pathways](https://arxiv.org/abs/2204.02311) ![Hall of Fame](https://img.shields.io/badge/⭐-Hall%20of%20Fame-ff1493?style=flat&labelColor=000000)

**Authors:** Aakanksha Chowdhery et al.<br>
**Contribution:** `📈 Model Scaling`

> Reports **PaLM**, a 540B dense model trained with Pathways, and evaluates few-shot language and reasoning tasks. Useful for studying scaling and prompting together; the report also examines bias, toxicity and memorization rather than establishing unrestricted capability.

---

### 📄 [Training Compute-Optimal Large Language Models](https://arxiv.org/abs/2203.15556) ![Hall of Fame](https://img.shields.io/badge/⭐-Hall%20of%20Fame-ff1493?style=flat&labelColor=000000)

**Authors:** Jordan Hoffmann et al.<br>
**Contribution:** `⚖️ Compute Allocation`

> Studies **compute-optimal allocation between parameter count and training tokens** under a fixed pretraining budget. Chinchilla shows why many contemporary large models were undertrained; deployment cost and inference frequency can change the preferred allocation.

---

### 📄 [Self-Consistency Improves Chain of Thought Reasoning in Language Models](https://arxiv.org/abs/2203.11171) ![Hall of Fame](https://img.shields.io/badge/⭐-Hall%20of%20Fame-ff1493?style=flat&labelColor=000000)

**Authors:** Wang et al.<br>
**Contribution:** `🗳️ Answer Aggregation`

> Samples **diverse reasoning paths and aggregates final answers** rather than using a single greedy chain. A foundational test-time-compute baseline; voting adds generation cost and is not a correctness certificate.

---

### 📄 [Training language models to follow instructions with human feedback](https://arxiv.org/abs/2203.02155) ![Hall of Fame](https://img.shields.io/badge/⭐-Hall%20of%20Fame-ff1493?style=flat&labelColor=000000)

**Authors:** Long Ouyang et al.<br>
**Contribution:** `🧑‍🏫 Instruction Following`

> Trains **InstructGPT** through human demonstrations, preference reward modeling and PPO, with a pretraining-mix variant. Labelers preferred a 1.3B aligned model to 175B GPT-3 on the tested prompt distribution; this is not universal capability superiority. [Detailed summary](../summaries/RLHF%20Training%20with%20Human%20Feedback.md).

---

### 📄 [Chain-of-Thought Prompting Elicits Reasoning in Large Language Models](https://arxiv.org/abs/2201.11903) ![Hall of Fame](https://img.shields.io/badge/⭐-Hall%20of%20Fame-ff1493?style=flat&labelColor=000000)

**Authors:** Jason Wei et al. (Google)<br>
**Contribution:** `🧮 Reasoning`

> Shows that **worked reasoning demonstrations** can improve arithmetic, commonsense and symbolic tasks without weight updates. Distinguish this few-shot method from Kojima et al.’s zero-shot reasoning instruction; extra tokens cost inference compute and explanations need not be faithful. [Detailed summary](../summaries/Chain-of-Thought%20Prompting.md).

---

### 📄 [LaMDA: Language Models for Dialog Applications](https://arxiv.org/abs/2201.08239) ![Hall of Fame](https://img.shields.io/badge/⭐-Hall%20of%20Fame-ff1493?style=flat&labelColor=000000)

**Authors:** Romal Thoppilan et al.<br>
**Contribution:** `💬 Dialogue`

> An **official LaMDA dialogue-model report**, combining web/dialogue pretraining, fine-tuning and tools for factual grounding. It makes quality, safety and groundedness separate evaluation targets; human-rated metrics are evidence rather than safety guarantees.

---

## 🏛️ 2021

### 📄 [Scaling Language Models: Methods, Analysis & Insights from Training Gopher](https://arxiv.org/abs/2112.11446) ![Hall of Fame](https://img.shields.io/badge/⭐-Hall%20of%20Fame-ff1493?style=flat&labelColor=000000)

**Authors:** Jack W. Rae et al.<br>
**Contribution:** `📊 Scaling Analysis`

> An **official Gopher report** studying a 280B model across a broad task suite. Scale helps reading comprehension and fact-checking more than selected logic/math tasks; data, bias and task-dependent failures remain central to its analysis.

---

### 📄 [Training Verifiers to Solve Math Word Problems](https://arxiv.org/abs/2110.14168) ![Hall of Fame](https://img.shields.io/badge/⭐-Hall%20of%20Fame-ff1493?style=flat&labelColor=000000)

**Authors:** Cobbe et al.<br>
**Contribution:** `✅ GSM8K & Verifiers`

> Introduces **GSM8K and learned verification** to select among sampled math solutions. It separates proposing an answer from ranking candidates; gains require sampling compute, and larger search can exploit verifier errors.

---

### 📄 [Finetuned Language Models Are Zero-Shot Learners](https://arxiv.org/abs/2109.01652) ![Hall of Fame](https://img.shields.io/badge/⭐-Hall%20of%20Fame-ff1493?style=flat&labelColor=000000)

**Authors:** Jason Wei et al. (Google)<br>
**Contribution:** `🎯 Task Generalization`

> Fine-tunes a language model on **tasks expressed through natural-language instructions** and evaluates held-out task families. FLAN makes instruction tuning a generalization strategy; task mixture, holdout design and base-model capability determine the observed transfer.

---

### 📄 [On the Opportunities and Risks of Foundation Models](https://arxiv.org/abs/2108.07258) ![Hall of Fame](https://img.shields.io/badge/⭐-Hall%20of%20Fame-ff1493?style=flat&labelColor=000000)

**Authors:** Rishi Bommasani et al.<br>
**Contribution:** `📖 Research Perspective`

> A **research report and perspective** defining foundation models and examining adaptation, homogenization and societal risks. It supplies a shared framework for inherited downstream capabilities and failures rather than a new training experiment.

---

### 📄 [Evaluating Large Language Models Trained on Code](https://arxiv.org/abs/2107.03374) ![Hall of Fame](https://img.shields.io/badge/⭐-Hall%20of%20Fame-ff1493?style=flat&labelColor=000000)

**Authors:** Mark Chen et al. (OpenAI)<br>
**Contribution:** `💻 Functional Code Evaluation`

> Studies **Codex code generation** and introduces HumanEval with execution-based functional correctness and sampling metrics. It makes candidate sampling and test-based evaluation central; passing limited tests differs from proving program correctness or broad reasoning ability.

---

### 📄 [LoRA: Low-Rank Adaptation of Large Language Models](https://arxiv.org/abs/2106.09685) ![Hall of Fame](https://img.shields.io/badge/⭐-Hall%20of%20Fame-ff1493?style=flat&labelColor=000000)

**Authors:** Edward J. Hu et al.<br>
**Contribution:** `💡 Efficient Adaptation`

> Freezes pretrained weights and trains **low-rank updates** to selected weight matrices. LoRA reduces trainable parameters and optimizer memory; the reduction depends on rank, model and target layers, while the base model still needs to fit in memory.

---

### 📄 [Switch Transformers: Scaling to Trillion Parameter Models with Simple and Efficient Sparsity](https://arxiv.org/abs/2101.03961) ![Hall of Fame](https://img.shields.io/badge/⭐-Hall%20of%20Fame-ff1493?style=flat&labelColor=000000)

**Authors:** William Fedus, Barret Zoph and Noam Shazeer (Google)<br>
**Contribution:** `🧩 Sparse MoE`

> Simplifies sparse MoE routing to **one selected expert per token**, with training and load-balancing methods for large models. Switch separates total capacity from active compute while building on earlier MoE/Transformer research; expert storage and communication remain costs.

---

### 📄 [Learning Transferable Visual Models From Natural Language Supervision](https://arxiv.org/abs/2103.00020) ![Hall of Fame](https://img.shields.io/badge/⭐-Hall%20of%20Fame-ff1493?style=flat&labelColor=000000)

**Authors:** Alec Radford et al. (OpenAI)<br>
**Contribution:** `🔗 Vision-Language Foundation`

> Learns **joint image/text embeddings through contrastive supervision** and evaluates zero-shot transfer using text descriptions of categories. CLIP connects language supervision to visual recognition; performance varies with distribution and remains limited on counting and abstract tasks.

---

## 🏛️ 2020

### 📄 [Language Models are Few-Shot Learners](https://arxiv.org/abs/2005.14165) ![Hall of Fame](https://img.shields.io/badge/⭐-Hall%20of%20Fame-ff1493?style=flat&labelColor=000000)

**Authors:** Tom B. Brown et al.<br>
**Contribution:** `🚀 In-Context Learning`

> Evaluated **GPT-3** across zero-, one- and few-shot tasks without task-specific weight updates. It made in-context task adaptation a central research direction, while retaining substantial reasoning, bias and contamination limitations. [Detailed summary](../summaries/GPT-3%20Language%20Models%20are%20Few-Shot%20Learners.md).

---

### 📄 [Retrieval-Augmented Generation for Knowledge-Intensive NLP Tasks](https://arxiv.org/abs/2005.11401) ![Hall of Fame](https://img.shields.io/badge/⭐-Hall%20of%20Fame-ff1493?style=flat&labelColor=000000)

**Authors:** Patrick Lewis et al.<br>
**Contribution:** `🔍 RAG Architecture`

> Combines a **dense retriever with a sequence generator**, marginalizing over retrieved passages for knowledge-intensive tasks. The paper establishes an influential RAG formulation alongside earlier retrieval-enhanced work; retrieval can support factuality but does not guarantee it.

---

### 📄 [Scaling Laws for Neural Language Models](https://arxiv.org/abs/2001.08361) ![Hall of Fame](https://img.shields.io/badge/⭐-Hall%20of%20Fame-ff1493?style=flat&labelColor=000000)

**Authors:** Jared Kaplan et al. (OpenAI)<br>
**Contribution:** `📊 Foundational Scaling`

> Fits empirical **language-model loss scaling** with parameters, data and compute over measured regimes. A quantitative framework for training allocation; loss fits should be distinguished from laws of general capability or unlimited extrapolation.

---

## 🏛️ 2019

### 📄 [Exploring the Limits of Transfer Learning with a Unified Text-to-Text Transformer](https://arxiv.org/abs/1910.10683) ![Hall of Fame](https://img.shields.io/badge/⭐-Hall%20of%20Fame-ff1493?style=flat&labelColor=000000)

**Authors:** Colin Raffel et al.<br>
**Contribution:** `🔄 Text-to-Text Transfer`

> Studies a **unified text-to-text task format**, pretraining objectives, data and transfer learning in T5. The controlled comparisons and C4 corpus are its reader value; the 2019 preprint precedes the JMLR 2020 publication.

---

### 📄 [ZeRO: Memory Optimizations Toward Training Trillion Parameter Models](https://arxiv.org/abs/1910.02054) ![Hall of Fame](https://img.shields.io/badge/⭐-Hall%20of%20Fame-ff1493?style=flat&labelColor=000000)

**Authors:** Samyam Rajbhandari, Jeff Rasley, Olatunji Ruwase and Yuxiong He (Microsoft)<br>
**Contribution:** `💾 State Partitioning`

> Partitions **optimizer states, gradients and parameters** across data-parallel workers to reduce redundant memory. ZeRO explains how memory savings interact with communication and parallelism; its trillion-parameter capacity analysis is distinct from demonstrating a trained trillion-parameter model.

---

### 📄 [Megatron-LM: Training Multi-Billion Parameter Language Models Using Model Parallelism](https://arxiv.org/abs/1909.08053) ![Hall of Fame](https://img.shields.io/badge/⭐-Hall%20of%20Fame-ff1493?style=flat&labelColor=000000)

**Authors:** Mohammad Shoeybi et al.<br>
**Contribution:** `⚙️ Tensor Parallelism`

> Introduces efficient **intra-layer tensor model parallelism** for multi-billion-parameter Transformer training. The original Megatron-LM report explains how to split attention and feed-forward computation across GPUs; pipeline parallelism belongs to later work.

---

### 📄 [Language Models are Unsupervised Multitask Learners](https://cdn.openai.com/better-language-models/language_models_are_unsupervised_multitask_learners.pdf) ![Hall of Fame](https://img.shields.io/badge/⭐-Hall%20of%20Fame-ff1493?style=flat&labelColor=000000)

**Authors:** Alec Radford et al. (OpenAI)<br>
**Contribution:** `🎯 Decoder-Only`

> An **official GPT-2 report** evaluating autoregressive language modeling as unsupervised multitask learning. It studies zero-shot transfer using task-formatted text; results vary widely across tasks, motivating investigation of scale rather than proving universal emergent capability.

---

### 📄 [Transformer-XL: Attentive Language Models Beyond a Fixed-Length Context](https://arxiv.org/abs/1901.02860) ![Hall of Fame](https://img.shields.io/badge/⭐-Hall%20of%20Fame-ff1493?style=flat&labelColor=000000)

**Authors:** Dai et al.<br>
**Contribution:** `🔁 Segment Recurrence`

> Combines **segment-level recurrence and relative positional encoding** to reuse prior hidden states beyond a fixed training segment. It explains context fragmentation and recurrent reuse; finite cached states and memory costs still constrain context.

---

## 🏛️ 2018

### 📄 [BERT: Pre-training of Deep Bidirectional Transformers for Language Understanding](https://arxiv.org/abs/1810.04805) ![Hall of Fame](https://img.shields.io/badge/⭐-Hall%20of%20Fame-ff1493?style=flat&labelColor=000000)

**Authors:** Jacob Devlin et al. (Google)<br>
**Contribution:** `🧠 Bidirectional`

> Pretrains a **bidirectional Transformer encoder** with masked-language modeling and a sentence-level objective, then adapts it to downstream tasks. BERT established an influential contextual pretraining recipe; masking and fine-tuning distinguish its use from autoregressive generation.

---

### 📄 [Improving Language Understanding by Generative Pre-Training](https://cdn.openai.com/research-covers/language-unsupervised/language_understanding_paper.pdf) ![Hall of Fame](https://img.shields.io/badge/⭐-Hall%20of%20Fame-ff1493?style=flat&labelColor=000000)

**Authors:** Alec Radford, Karthik Narasimhan, Tim Salimans and Ilya Sutskever<br>
**Contribution:** `🌱 Generative Pretraining`

> Studies **generative pretraining on BooksCorpus followed by task-specific supervised adaptation** in GPT-1. It demonstrates useful transfer from a decoder language model, building on earlier language pretraining rather than originating the two-stage idea.

---

## 🏛️ 2017

### 📄 [Deep Contextualized Word Representations](https://arxiv.org/abs/1802.05365) ![Hall of Fame](https://img.shields.io/badge/⭐-Hall%20of%20Fame-ff1493?style=flat&labelColor=000000)

**Authors:** Peters et al.<br>
**Contribution:** `🧠 Contextual Representations`

> **ELMo** combines internal layers of a bidirectional language model into context-dependent word representations for downstream systems. Read it as a bridge from static embeddings to contextual pretraining, not the first contextual representation method; earlier public OpenReview posting predates NAACL 2018.

---

### 📄 [Deep reinforcement learning from human preferences](https://arxiv.org/abs/1706.03741) ![Hall of Fame](https://img.shields.io/badge/⭐-Hall%20of%20Fame-ff1493?style=flat&labelColor=000000)

**Authors:** Paul Christiano et al.<br>
**Contribution:** `🏗️ Foundation`

> Learns **reward models from human comparisons of trajectory segments** and uses them to train deep-RL agents. A foundational preference-learning demonstration in simulated control/Atari, providing lineage for later language-model RLHF rather than originating all human-feedback learning.

---

### 📄 [Attention Is All You Need](https://arxiv.org/abs/1706.03762) ![Hall of Fame](https://img.shields.io/badge/⭐-Hall%20of%20Fame-ff1493?style=flat&labelColor=000000)

**Authors:** Ashish Vaswani et al.<br>
**Contribution:** `🏗️ Transformer`

> Introduced the attention-based **Transformer** for sequence transduction, removing recurrent and convolutional sequence layers. Parallel training and shorter dependency paths helped establish the architecture used by BERT and GPT; autoregressive generation remains sequential. [Detailed summary](../summaries/Attention%20Is%20All%20You%20Need%20.md).

---

### 📄 [Outrageously Large Neural Networks: The Sparsely-Gated Mixture-of-Experts Layer](https://arxiv.org/abs/1701.06538) ![Hall of Fame](https://img.shields.io/badge/⭐-Hall%20of%20Fame-ff1493?style=flat&labelColor=000000)

**Authors:** Shazeer et al.<br>
**Contribution:** `🧩 Conditional Computation`

> Introduces a **sparsely gated expert layer** that activates a small subset of networks per input. It separates total capacity from active compute while exposing load balancing and communication as central engineering problems; a key precursor to Switch and modern MoE models.

---

## 🏛️ 2000

### 📄 [A Neural Probabilistic Language Model](https://jmlr.org/papers/v3/bengio03a.html) ![Hall of Fame](https://img.shields.io/badge/⭐-Hall%20of%20Fame-ff1493?style=flat&labelColor=000000)

**Authors:** Bengio, Ducharme & Vincent (NIPS 2000); with Jauvin (JMLR 2003)<br>
**Contribution:** `🧠 Learned Word Representations`

> Learns distributed word representations jointly with a **neural next-word predictor**, sharing statistical strength across similar word sequences. A historical foundation for neural language modeling; the fixed context and computational limits differ from modern LLMs. The NIPS 2000 precursor predates the expanded JMLR 2003 paper. [NIPS 2000 record](https://papers.nips.cc/paper/2000/hash/728f206c2a01bf572b5940d7d9a8fa4c-Abstract.html).

---

[← Browse the collection](../README.md) · [Suggest a paper or correction](../CONTRIBUTING.md)
