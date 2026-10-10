# 📚 RAG & Knowledge: Retrieval-Augmented Generation

<div align="center">

[![Awesome](https://awesome.re/badge-flat2.svg)](https://awesome.re)
[![Works](https://img.shields.io/badge/Works-17-blue.svg)](all-papers.md)
[![Years](https://img.shields.io/badge/Years-2019--2025-green.svg)](all-papers.md)
[![License: CC0](https://img.shields.io/badge/License-CC0-yellow.svg)](../LICENSE)
[![PRs Welcome](https://img.shields.io/badge/PRs-welcome-brightgreen.svg?style=flat-square)](../CONTRIBUTING.md)

### Papers on retrieval-augmented generation, long context modeling, and memory-augmented systems

_From foundational RAG architectures to million-token context windows and persistent memory systems._

</div>

---

## 📑 Table of Contents

- [🔍 RAG Foundations](#-rag-foundations)
- [📏 Long Context](#-long-context)
- [🧠 Memory Systems](#-memory-systems)

---

## 🔍 RAG Foundations

### 📄 [Retrieval-Augmented Generation for Knowledge-Intensive NLP Tasks](https://arxiv.org/abs/2005.11401) ![Hall of Fame](https://img.shields.io/badge/⭐-Hall%20of%20Fame-ff1493?style=flat&labelColor=000000)

**Authors:** Patrick Lewis et al.<br>
**Contribution:** `🔍 RAG Architecture`

> Combines a **dense retriever with a sequence generator**, marginalizing over retrieved passages for knowledge-intensive tasks. The paper establishes an influential RAG formulation alongside earlier retrieval-enhanced work; retrieval can support factuality but does not guarantee it.

---

### 📄 [REALM: Retrieval-Augmented Language Model Pre-Training](https://arxiv.org/abs/2002.08909)

**Authors:** Kelvin Guu et al. (Google Research)<br>
**Contribution:** `🎓 Pre-training with Retrieval`

> Pioneered the concept of **pre-training language models with retrieval**. REALM learns to retrieve documents that help predict masked tokens during pre-training, creating a model that inherently knows how to use external knowledge. This end-to-end approach to learning retrieval alongside language modeling laid crucial groundwork for modern RAG systems.

---

### 📄 [Self-RAG: Learning to Retrieve, Generate, and Critique through Self-Reflection](https://arxiv.org/abs/2310.11511)

**Authors:** Akari Asai et al.<br>
**Contribution:** `🪞 Self-Reflective RAG` 🆕

> Trains a model to generate **retrieval and reflection tokens**, allowing adaptive retrieval and assessment of passages and answers. Self-RAG studies improved factuality and citation quality in selected tasks; learned critique is a useful signal rather than a correctness guarantee.

---

### 📄 [RAPTOR: Recursive Abstractive Processing for Tree-Organized Retrieval](https://arxiv.org/abs/2401.18059)

**Authors:** Parth Sarthi et al.<br>
**Contribution:** `🌳 Hierarchical Retrieval` 🆕

> Proposed a novel approach to organizing retrieved information in a **hierarchical tree structure**. RAPTOR recursively clusters and summarizes text chunks, creating multi-level abstractions that enable retrieval at different granularities. This allows the model to answer questions requiring both fine-grained details and high-level synthesis across large document collections.

---

## 📏 Long Context

### 📄 [RoFormer: Enhanced Transformer with Rotary Position Embedding](https://arxiv.org/abs/2104.09864)

**Authors:** Jianlin Su et al.<br>
**Contribution:** `🔄 Position Encoding`

> Introduces **rotary positional embeddings (RoPE)**, combining absolute rotations with relative-position effects in attention scores. RoFormer supplies the mathematical foundation for a widely reused positional scheme; extending context still needs suitable training and evaluation.

---

### 📄 [LongLoRA: Efficient Fine-tuning of Long-Context Large Language Models](https://arxiv.org/abs/2309.12307)

**Authors:** Yukang Chen et al.<br>
**Contribution:** `⚡ Efficient Long Context` 🆕

> Combines **shifted sparse attention during fine-tuning** with parameter-efficient adaptation for long context. LongLoRA also trains embeddings and normalization parameters; sparse training does not imply the same attention pattern at inference.

---

### 📄 [Ring Attention with Blockwise Transformers for Near-Infinite Context](https://arxiv.org/abs/2310.01889)

**Authors:** Hao Liu et al.<br>
**Contribution:** `♾️ Infinite Context` 🆕

> Distributes blockwise attention across devices in a **ring**, overlapping computation with communication. Longer sequences become feasible as device resources grow; memory, communication and arithmetic costs still bound the achievable context.

---

### 📄 [Extending Context Window of Large Language Models via Positional Interpolation](https://arxiv.org/abs/2306.15595)

**Authors:** Shouyuan Chen et al. (Meta AI)<br>
**Contribution:** `📐 Context Extension` 🆕

> Extends RoPE-based context through **position interpolation**, mapping positions back into the original range before fine-tuning. The paper studies 2,048 → 32,768 tokens; extended capacity still needs task-specific utilization and quality checks.

---

### 📄 [Transformer-XL: Attentive Language Models Beyond a Fixed-Length Context](https://arxiv.org/abs/1901.02860) ![Hall of Fame](https://img.shields.io/badge/⭐-Hall%20of%20Fame-ff1493?style=flat&labelColor=000000)

**Authors:** Dai et al.<br>
**Contribution:** `🔁 Segment Recurrence`

> Combines **segment-level recurrence and relative positional encoding** to reuse prior hidden states beyond a fixed training segment. It explains context fragmentation and recurrent reuse; finite cached states and memory costs still constrain context.

---

### 📄 [Lost in the Middle: How Language Models Use Long Contexts](https://arxiv.org/abs/2307.03172)

**Authors:** Liu et al.<br>
**Contribution:** `📍 Context Utilization`

> Varies relevant-information position in **multi-document QA and key-value retrieval**, finding weaker use of middle positions in many tested models. Context capacity is not context utilization; these 2023 model versions motivate retesting rather than a permanent verdict on every long-context model.

---

## 🧠 Memory Systems

### 📄 [MemGPT: Towards LLMs as Operating Systems](https://arxiv.org/abs/2310.08560)

**Authors:** Charles Packer et al.<br>
**Contribution:** `💾 Virtual Memory` 🆕

> Treats context as a **managed memory hierarchy**, paging between a bounded prompt and external storage. MemGPT studies document analysis and conversation memory; external capacity and reliable retrieval are different properties.

---

### 📄 [Memorizing Transformers](https://arxiv.org/abs/2203.08913)

**Authors:** Yuhuai Wu, Markus N. Rabe, DeLesley Hutchins and Christian Szegedy (Google)<br>
**Contribution:** `🗄️ External Memory`

> Augmented Transformers with a **kNN-based external memory** that stores and retrieves past key-value pairs. This approach allows the model to attend over a massive corpus of past activations without increasing computational cost proportionally. The technique demonstrated significant improvements on language modeling tasks, especially for rare patterns and long-range dependencies.

---

### 📄 [Augmenting Language Models with Long-Term Memory](https://arxiv.org/abs/2306.07174)

**Authors:** Weizhi Wang et al.<br>
**Contribution:** `🧠 Long-Term Memory` 🆕

> Uses a **frozen backbone as memory encoder** and a trainable SideNet to retrieve and read cached representations. LongMem separates storage from adaptation to reduce stale-memory issues; retrieval, storage and side-network training remain costs.

---

### 📄 [Leave No Context Behind: Efficient Infinite Context Transformers with Infini-attention](https://arxiv.org/abs/2404.07143)

**Authors:** Tsendsuren Munkhdalai et al.<br>
**Contribution:** `∞ Compressive Memory` 🆕

> Combines **local attention and compressive memory** to process successive segments with bounded working memory. Infini-attention can extend the processed sequence, but total computation grows with input length and compressed history can lose detail.

---

### 📄 [From Local to Global: A Graph RAG Approach to Query-Focused Summarization](https://arxiv.org/abs/2404.16130)

**Authors:** Darren Edge et al. (Microsoft)<br>
**Contribution:** `🕸️ Knowledge Graph RAG`

> Builds entity graphs and hierarchical community summaries for **global, query-focused summarization**. It improves coverage and diversity in the authors’ comparison with conventional RAG; graph construction and summarization add cost, and benefits depend on the corpus and question type.

---

### 📄 [Retrieval Augmented Generation or Long-Context LLMs? A Comprehensive Study and Hybrid Approach](https://arxiv.org/abs/2407.16833)

**Authors:** Zhuowan Li et al.<br>
**Contribution:** `🔬 RAG vs Long-Context`

> Compares retrieval-augmented generation with long-context models. With sufficient resources, **long context performs better on average in the tested setups**, while RAG is substantially cheaper; Self-Route combines the approaches. Model, retrieval quality, task and budget determine the trade-off.

---

### 📄 [Recursive Language Models](https://arxiv.org/abs/2512.24601)

**Authors:** Zhang, Kraska & Khattab<br>
**Contribution:** `🔁 Context as Environment`

> Exposes a long input through a **programmable environment** and allows recursive model calls over selected pieces. RLM studies managing context outside a single prompt; recursion is not always beneficial, and call costs and latency have long tails.

---

<div align="center">

### 🌟 Contributing

Feel free to submit PRs to add more RAG, long context, or memory papers!

### 📜 License

This repository is licensed under CC0 License.

### 🙏 Acknowledgments

Thanks to all researchers pushing the boundaries of how LLMs access and utilize knowledge.

---

⭐ If you find this repository helpful, please consider giving it a star!

</div>
