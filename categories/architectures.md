# Awesome Model Architectures

[![Awesome](https://awesome.re/badge-flat2.svg)](https://awesome.re)
[![PRs Welcome](https://img.shields.io/badge/PRs-welcome-brightgreen.svg?style=flat-square)](../CONTRIBUTING.md)

A curated collection of papers defining the core architectures that power modern language models.

_From the original Transformer to State Space Models and Mixture of Experts, these papers represent the fundamental innovations in neural network design for language understanding._

---

## 📑 Table of Contents

- [🏛️ Foundational Architectures](#%EF%B8%8F-foundational-architectures)
- [🐍 State Space Models](#-state-space-models)
- [🧩 Mixture of Experts](#-mixture-of-experts)
- [🆕 Recent Breakthroughs](#-recent-breakthroughs)
- [📚 Language Model Families](#-language-model-families)

---

## 🏛️ Foundational Architectures

### 📄 [Attention Is All You Need](https://arxiv.org/abs/1706.03762) ![Hall of Fame](https://img.shields.io/badge/⭐-Hall%20of%20Fame-ff1493?style=flat&labelColor=000000)

**Authors:** Ashish Vaswani et al.<br>
**Contribution:** `🏗️ Transformer`

> Introduced the attention-based **Transformer** for sequence transduction, removing recurrent and convolutional sequence layers. Parallel training and shorter dependency paths helped establish the architecture used by BERT and GPT; autoregressive generation remains sequential. [Detailed summary](../summaries/Attention%20Is%20All%20You%20Need%20.md).

---

### 📄 [BERT: Pre-training of Deep Bidirectional Transformers for Language Understanding](https://arxiv.org/abs/1810.04805) ![Hall of Fame](https://img.shields.io/badge/⭐-Hall%20of%20Fame-ff1493?style=flat&labelColor=000000)

**Authors:** Jacob Devlin et al. (Google)<br>
**Contribution:** `🧠 Bidirectional`

> Pretrains a **bidirectional Transformer encoder** with masked-language modeling and a sentence-level objective, then adapts it to downstream tasks. BERT established an influential contextual pretraining recipe; masking and fine-tuning distinguish its use from autoregressive generation.

---

### 📄 [Language Models are Unsupervised Multitask Learners](https://cdn.openai.com/better-language-models/language_models_are_unsupervised_multitask_learners.pdf) ![Hall of Fame](https://img.shields.io/badge/⭐-Hall%20of%20Fame-ff1493?style=flat&labelColor=000000)

**Authors:** Alec Radford et al. (OpenAI)<br>
**Contribution:** `🎯 Decoder-Only`

> An **official GPT-2 report** evaluating autoregressive language modeling as unsupervised multitask learning. It studies zero-shot transfer using task-formatted text; results vary widely across tasks, motivating investigation of scale rather than proving universal emergent capability.

---

### 📄 [A Neural Probabilistic Language Model](https://jmlr.org/papers/v3/bengio03a.html) ![Hall of Fame](https://img.shields.io/badge/⭐-Hall%20of%20Fame-ff1493?style=flat&labelColor=000000)

**Authors:** Bengio, Ducharme & Vincent (NIPS 2000); with Jauvin (JMLR 2003)<br>
**Contribution:** `🧠 Learned Word Representations`

> Learns distributed word representations jointly with a **neural next-word predictor**, sharing statistical strength across similar word sequences. A historical foundation for neural language modeling; the fixed context and computational limits differ from modern LLMs. The NIPS 2000 precursor predates the expanded JMLR 2003 paper. [NIPS 2000 record](https://papers.nips.cc/paper/2000/hash/728f206c2a01bf572b5940d7d9a8fa4c-Abstract.html).

---

### 📄 [Deep Contextualized Word Representations](https://arxiv.org/abs/1802.05365) ![Hall of Fame](https://img.shields.io/badge/⭐-Hall%20of%20Fame-ff1493?style=flat&labelColor=000000)

**Authors:** Peters et al.<br>
**Contribution:** `🧠 Contextual Representations`

> See the main entry in [Training](training.md) for the method, evidence and limitations.

---

### 📄 [Transformer-XL: Attentive Language Models Beyond a Fixed-Length Context](https://arxiv.org/abs/1901.02860) ![Hall of Fame](https://img.shields.io/badge/⭐-Hall%20of%20Fame-ff1493?style=flat&labelColor=000000)

**Authors:** Dai et al.<br>
**Contribution:** `🔁 Segment Recurrence`

> See the main entry in [Rag](rag.md) for the method, evidence and limitations.

---

### 📄 [Neural Machine Translation by Jointly Learning to Align and Translate](https://arxiv.org/abs/1409.0473)

**Authors:** Bahdanau, Cho & Bengio<br>
**Contribution:** `🎯 Learned Alignment`

> Learns **soft alignment over encoder states** while generating translations, addressing a fixed-vector bottleneck. A crucial attention precursor to the Transformer; its recurrent translation setting differs from later self-attention language models.

---

## 🐍 State Space Models

### 📄 [Mamba: Linear-Time Sequence Modeling with Selective State Spaces](https://arxiv.org/abs/2312.00752) ![Hall of Fame](https://img.shields.io/badge/⭐-Hall%20of%20Fame-ff1493?style=flat&labelColor=000000)

**Authors:** Albert Gu and Tri Dao<br>
**Contribution:** `🐍 SSM Architecture`

> Makes **state-space parameters input-dependent** and uses a hardware-aware scan for sequence modeling. Mamba studies selective information propagation with linear sequence scaling; throughput and quality comparisons are tied to the tested models and workloads, with finite-state recall limits.

---

### 📄 [Transformers are SSMs: Generalized Models and Efficient Algorithms Through Structured State Space Duality](https://arxiv.org/abs/2405.21060)

**Authors:** Tri Dao et al.<br>
**Contribution:** `🔄 Unified Theory`

> Develops **structured state-space duality** connecting a class of state-space models and attention formulations. Mamba-2 uses this structure for efficient algorithms; the reported kernel speedups should not be read as end-to-end training speedups for every model.

---

## 🧩 Mixture of Experts

### 📄 [Switch Transformers: Scaling to Trillion Parameter Models with Simple and Efficient Sparsity](https://arxiv.org/abs/2101.03961) ![Hall of Fame](https://img.shields.io/badge/⭐-Hall%20of%20Fame-ff1493?style=flat&labelColor=000000)

**Authors:** William Fedus, Barret Zoph and Noam Shazeer (Google)<br>
**Contribution:** `🧩 Sparse MoE`

> Simplifies sparse MoE routing to **one selected expert per token**, with training and load-balancing methods for large models. Switch separates total capacity from active compute while building on earlier MoE/Transformer research; expert storage and communication remain costs.

---

### 📄 [Mixtral of Experts](https://arxiv.org/abs/2401.04088)

**Authors:** Albert Q. Jiang et al. (Mistral AI)<br>
**Contribution:** `⚡ Efficient MoE`

> Reports **Mixtral 8×7B**, routing each token to two experts with about 13B active of 46.7B total parameters. Its evaluated quality/compute trade-offs are useful for sparse models; all expert weights still require storage and comparator results are benchmark-specific.

---

### 📄 [Outrageously Large Neural Networks: The Sparsely-Gated Mixture-of-Experts Layer](https://arxiv.org/abs/1701.06538) ![Hall of Fame](https://img.shields.io/badge/⭐-Hall%20of%20Fame-ff1493?style=flat&labelColor=000000)

**Authors:** Shazeer et al.<br>
**Contribution:** `🧩 Conditional Computation`

> Introduces a **sparsely gated expert layer** that activates a small subset of networks per input. It separates total capacity from active compute while exposing load balancing and communication as central engineering problems; a key precursor to Switch and modern MoE models.

---

### 📄 [DeepSeek-V3 Technical Report](https://arxiv.org/abs/2412.19437)

**Authors:** DeepSeek-AI<br>
**Contribution:** `🧩 Sparse Model Systems`

> Combines **MoE, multi-head latent attention, load balancing and FP8 training** in a large model system. Read it for the interaction of architecture and training infrastructure; reported training costs exclude earlier research and do not represent total development cost.

---

## 🆕 Recent Breakthroughs

### 📄 [Jamba: A Hybrid Transformer-Mamba Language Model](https://arxiv.org/abs/2403.19887)

**Authors:** Opher Lieber et al.<br>
**Contribution:** `🔀 Hybrid Architecture`

> Combines **attention, Mamba and MoE layers** in a hybrid language model. Jamba explores balancing long-context throughput and quality, with up to 256K context; its single-GPU demonstration uses a particular 80GB configuration.

---

### 📄 [Titans: Learning to Memorize at Test Time](https://arxiv.org/abs/2501.00663) ![Hall of Fame](https://img.shields.io/badge/⭐-Hall%20of%20Fame-ff1493?style=flat&labelColor=000000)

**Authors:** Ali Behrouz, Peilin Zhong, Vahab Mirrokni<br>
**Contribution:** `🧠 Neural Memory`

> Combines local attention with **gradient-updated neural memory**, using surprise-sensitive updates, momentum and decay. MAC, MAG and MAL offer different integrations; long-context demonstrations do not establish perfect recall or a universal winning variant. [Detailed summary](../summaries/Titans%20Learning%20to%20Memorize%20at%20Test%20Time.md).

---

### 📄 [Mixture-of-Depths: Dynamically allocating compute in transformer-based language models](https://arxiv.org/abs/2404.02258)

**Authors:** David Raposo et al.<br>
**Contribution:** `⚡ Dynamic Compute`

> Uses learned token routing with a **fixed top-k compute budget** at selected layers. Mixture-of-Depths studies allocating computation across tokens; routing scores are not a validated classifier of which tokens are intellectually difficult.

---

### 📄 [Retentive Network: A Successor to Transformer for Large Language Models](https://arxiv.org/abs/2307.08621)

**Authors:** Yutao Sun et al.<br>
**Contribution:** `🔄 Retention Mechanism`

> Introduces **retention** with parallel training, recurrent decoding and chunkwise computation. RetNet studies an architectural alternative to attention; constant-state/per-step recurrent decoding is relative to prior sequence length, while total sequence processing still grows with length.

---

### 📄 [Hyena Hierarchy: Towards Larger Convolutional Language Models](https://arxiv.org/abs/2302.10866)

**Authors:** Michael Poli et al.<br>
**Contribution:** `🌊 Subquadratic Attention`

> Proposes **Hyena**, a subquadratic replacement for attention based on long convolutions and data-controlled gating. Achieves comparable quality to Transformers while reducing compute requirements significantly for long sequences. Demonstrates that attention is not the only path to high-quality language modeling, opening new architectural possibilities.

---

### 📄 [RWKV: Reinventing RNNs for the Transformer Era](https://arxiv.org/abs/2305.13048)

**Authors:** Bo Peng et al.<br>
**Contribution:** `🔁 Linear RNN`

> Combines parallelizable training with **recurrent decoding and a fixed-size state**. RWKV explores language modeling without retaining a full attention cache; state and per-token cost are constant relative to history length, while producing a sequence takes linear total steps.

---

### 📄 [DeepSeek-V3.2: Pushing the Frontier of Open Large Language Models](https://arxiv.org/abs/2512.02556)

**Authors:** DeepSeek-AI et al.<br>
**Contribution:** `🧠 Sparse Attention & Reasoning`

> Combines **DeepSeek Sparse Attention**, scaled reinforcement learning and synthetic agent tasks in an open-weight model family. The technical report provides reasoning and agent evaluations; performance depends on model variant, test-time budget and harness, rather than a universal cost advantage.

---

### 📄 [mHC: Manifold-Constrained Hyper-Connections](https://arxiv.org/abs/2512.24880)

**Authors:** Zhenda Xie et al. (DeepSeek)<br>
**Contribution:** `📐 Stable Residuals`

> Constrains expanded residual mixing through **doubly stochastic projections** to improve stability while preserving useful connectivity. The 27B BBH comparison is 48.9% → 51.0% over HC, a 2.1 percentage-point gain; the reported 6.7% training overhead applies to an optimized expansion-rate-4 configuration.

---

### 📄 [Training Large Language Models to Reason in a Continuous Latent Space](https://arxiv.org/abs/2412.06769)

**Authors:** Hao et al.<br>
**Contribution:** `🌀 Continuous Reasoning`

> See the main entry in [Reasoning](reasoning.md) for the method, evidence and limitations.

---

### 📄 [Scaling up Test-Time Compute with Latent Reasoning: A Recurrent Depth Approach](https://arxiv.org/abs/2502.05171)

**Authors:** Geiping et al.<br>
**Contribution:** `🌀 Recurrent Depth`

> Trains a **shared recurrent core** so inference can spend additional computation in hidden states without emitting more reasoning tokens. It extends earlier recurrent-depth architectures; data and compute differences in baselines limit claims of universal efficiency.

---

### 📄 [Large Language Diffusion Models](https://arxiv.org/abs/2502.09992)

**Authors:** Nie et al.<br>
**Contribution:** `🌫️ Masked Diffusion`

> **LLaDA** learns masked-token denoising and generates through iterative unmasking, offering a scaled alternative to autoregressive language modeling. Its 8B comparisons are informative but do not establish superiority under fully matched training data and compute.

---

### 📄 [Conditional Memory via Scalable Lookup: A New Axis of Sparsity for Large Language Models](https://arxiv.org/abs/2601.07372)

**Authors:** Cheng et al.<br>
**Contribution:** `🗂️ Conditional Memory`

> **Engram** uses hashed n-gram lookup with contextual gating alongside neural computation. Matched-budget MoE studies support this separation of memory and computation; related over-encoding work predates it, and offload throughput tests do not imply universal overhead.

---

### 📄 [Attention Residuals](https://arxiv.org/abs/2603.15031)

**Authors:** Kimi Team (Guangyu Chen et al.)<br>
**Contribution:** `🔀 Depth Aggregation`

> Uses **input-dependent aggregation across depth**, with Block AttnRes and systems optimizations for scaled training. Read it as a practical engineering advance in a family including earlier depth-mixing methods; superiority to Dynamic Cross Attention is not established by a head-to-head comparison.

---

## 📚 Language Model Families

### 📄 [Improving Language Understanding by Generative Pre-Training](https://cdn.openai.com/research-covers/language-unsupervised/language_understanding_paper.pdf) ![Hall of Fame](https://img.shields.io/badge/⭐-Hall%20of%20Fame-ff1493?style=flat&labelColor=000000)

**Authors:** Alec Radford, Karthik Narasimhan, Tim Salimans and Ilya Sutskever<br>
**Contribution:** `🌱 Generative Pretraining`

> Studies **generative pretraining on BooksCorpus followed by task-specific supervised adaptation** in GPT-1. It demonstrates useful transfer from a decoder language model, building on earlier language pretraining rather than originating the two-stage idea.

---

### 📄 [Language Models are Few-Shot Learners](https://arxiv.org/abs/2005.14165) ![Hall of Fame](https://img.shields.io/badge/⭐-Hall%20of%20Fame-ff1493?style=flat&labelColor=000000)

**Authors:** Tom B. Brown et al.<br>
**Contribution:** `🚀 In-Context Learning`

> Evaluated **GPT-3** across zero-, one- and few-shot tasks without task-specific weight updates. It made in-context task adaptation a central research direction, while retaining substantial reasoning, bias and contamination limitations. [Detailed summary](../summaries/GPT-3%20Language%20Models%20are%20Few-Shot%20Learners.md).

---

### 📄 [Exploring the Limits of Transfer Learning with a Unified Text-to-Text Transformer](https://arxiv.org/abs/1910.10683) ![Hall of Fame](https://img.shields.io/badge/⭐-Hall%20of%20Fame-ff1493?style=flat&labelColor=000000)

**Authors:** Colin Raffel et al.<br>
**Contribution:** `🔄 Text-to-Text Transfer`

> Studies a **unified text-to-text task format**, pretraining objectives, data and transfer learning in T5. The controlled comparisons and C4 corpus are its reader value; the 2019 preprint precedes the JMLR 2020 publication.

---

### 📄 [LaMDA: Language Models for Dialog Applications](https://arxiv.org/abs/2201.08239) ![Hall of Fame](https://img.shields.io/badge/⭐-Hall%20of%20Fame-ff1493?style=flat&labelColor=000000)

**Authors:** Romal Thoppilan et al.<br>
**Contribution:** `💬 Dialogue`

> An **official LaMDA dialogue-model report**, combining web/dialogue pretraining, fine-tuning and tools for factual grounding. It makes quality, safety and groundedness separate evaluation targets; human-rated metrics are evidence rather than safety guarantees.

---

### 📄 [PaLM: Scaling Language Modeling with Pathways](https://arxiv.org/abs/2204.02311) ![Hall of Fame](https://img.shields.io/badge/⭐-Hall%20of%20Fame-ff1493?style=flat&labelColor=000000)

**Authors:** Aakanksha Chowdhery et al.<br>
**Contribution:** `📈 Model Scaling`

> Reports **PaLM**, a 540B dense model trained with Pathways, and evaluates few-shot language and reasoning tasks. Useful for studying scaling and prompting together; the report also examines bias, toxicity and memorization rather than establishing unrestricted capability.

---

### 📄 [BLOOM: A 176B-Parameter Open-Access Multilingual Language Model](https://arxiv.org/abs/2211.05100) ![Hall of Fame](https://img.shields.io/badge/⭐-Hall%20of%20Fame-ff1493?style=flat&labelColor=000000)

**Authors:** BigScience Workshop et al.<br>
**Contribution:** `🌍 Multilingual Research`

> An **official report on BLOOM**, a 176B multilingual model developed through the BigScience collaboration. It documents collaborative training and access to model artifacts; its Responsible AI License and disclosed resources should be distinguished from unrestricted licensing or full reproducibility.

---

### 📄 [LLaMA: Open and Efficient Foundation Language Models](https://arxiv.org/abs/2302.13971) ![Hall of Fame](https://img.shields.io/badge/⭐-Hall%20of%20Fame-ff1493?style=flat&labelColor=000000)

**Authors:** Hugo Touvron et al.<br>
**Contribution:** `🦙 Model Access`

> Releases **LLaMA research-access model weights** and studies data-efficient autoregressive training across several sizes. A pivotal access milestone for language-model research; the original research license and partially disclosed data differ from unrestricted open-source reproducibility.

---

### 📄 [Llama 2: Open Foundation and Fine-Tuned Chat Models](https://arxiv.org/abs/2307.09288) ![Hall of Fame](https://img.shields.io/badge/⭐-Hall%20of%20Fame-ff1493?style=flat&labelColor=000000)

**Authors:** Hugo Touvron et al. (Meta)<br>
**Contribution:** `🦙 Open-Weight Models`

> An **official Llama 2 report** on pretrained and chat-tuned open-weight models, including preference training and safety evaluations. It broadened research/commercial access under its license; released weights differ from fully disclosed training data.

---

### 📄 [Mistral 7B](https://arxiv.org/abs/2310.06825) ![Hall of Fame](https://img.shields.io/badge/⭐-Hall%20of%20Fame-ff1493?style=flat&labelColor=000000)

**Authors:** Albert Q. Jiang et al.<br>
**Contribution:** `⚡ Model Efficiency`

> Combines **grouped-query attention and sliding-window attention** in the Mistral 7B model. The report compares favorably with Llama 2 13B on its evaluated suite; these architectural ingredients predate Mistral and gains remain benchmark-specific.

---

### 📄 [The Llama 3 Herd of Models](https://arxiv.org/abs/2407.21783) ![Hall of Fame](https://img.shields.io/badge/⭐-Hall%20of%20Fame-ff1493?style=flat&labelColor=000000)

**Authors:** Aaron Grattafiori et al.<br>
**Contribution:** `🦙 Model Systems`

> An **official Llama 3 model-family report** covering models through 405B parameters, 128K context, post-training and safety evaluations. Useful for large-scale model development; released weights do not imply publication of all training data, and multimodal integrations include research experiments.

---

<div align="center">

### 🌟 Contributing

Feel free to submit PRs to add more architecture papers or improve existing entries!

### 📜 License

This repository is licensed under CC0 License.

### 🙏 Acknowledgments

This collection celebrates the researchers pushing the boundaries of neural network design for language understanding.

---

⭐ If you find this repository helpful, please consider giving it a star!

</div>
