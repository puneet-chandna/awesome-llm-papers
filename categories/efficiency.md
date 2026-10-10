# Awesome Efficiency & Scaling

[![Awesome](https://awesome.re/badge-flat2.svg)](https://awesome.re)
[![PRs Welcome](https://img.shields.io/badge/PRs-welcome-brightgreen.svg?style=flat-square)](../CONTRIBUTING.md)

Essential papers on making LLMs faster, smaller, and more deployable.

_From quantization breakthroughs to attention optimization, these papers enable running powerful models on limited hardware._

---

## 📑 Table of Contents

- [🔢 Quantization](#-quantization)
- [⚡ Attention Optimization](#-attention-optimization)
- [🚀 Inference Optimization](#-inference-optimization)
- [✂️ Pruning & Sparsity](#%EF%B8%8F-pruning--sparsity)
- [⚙️ Training Efficiency](#%EF%B8%8F-training-efficiency)

---

## 🔢 Quantization

### 📄 [GPTQ: Accurate Post-Training Quantization for Generative Pre-trained Transformers](https://arxiv.org/abs/2210.17323)

**Authors:** Elias Frantar et al.<br>
**Contribution:** `🔢 Post-Training Quantization`

> Uses approximate second-order information for **one-shot, layer-wise weight quantization**. GPTQ demonstrates low-bit compression in evaluated GPT/OPT models; accuracy and speed depend on bit width, calibration and GPU kernels.

---

### 📄 [QLoRA: Efficient Finetuning of Quantized LLMs](https://arxiv.org/abs/2305.14314)

**Authors:** Tim Dettmers et al.<br>
**Contribution:** `🗜️ Memory Efficiency`

> Combined 4-bit quantization with LoRA to enable **fine-tuning of 65B parameter models on a single 48GB GPU**. QLoRA introduced innovations like 4-bit NormalFloat quantization and Double Quantization, reducing memory usage without sacrificing performance. This democratized fine-tuning of large models, making it accessible to researchers without massive compute resources.

---

### 📄 [AWQ: Activation-aware Weight Quantization for LLM Compression and Acceleration](https://arxiv.org/abs/2306.00978)

**Authors:** Ji Lin et al.<br>
**Contribution:** `🧠 Activation-Aware Compression`

> Uses activation statistics to identify **quantization-sensitive channels**, then scales channels to reduce low-bit error. AWQ studies hardware-aware deployment with efficient kernels; accuracy and latency gains depend on calibration, model and device.

---

### 📄 [The Era of 1-bit LLMs: All Large Language Models are in 1.58 Bits](https://arxiv.org/abs/2402.17764)

**Authors:** Shuming Ma et al. (Microsoft Research)<br>
**Contribution:** `🔢 1-bit Quantization`

> Studies **BitNet b1.58**, whose trained weights are ternary (−1, 0, +1) with quantization-aware computation. It presents a low-bit training approach, not evidence that arbitrary pretrained models can be converted to 1.58 bits without retraining or loss.

---

## ⚡ Attention Optimization

### 📄 [FlashAttention: Fast and Memory-Efficient Exact Attention with IO-Awareness](https://arxiv.org/abs/2205.14135) ![Hall of Fame](https://img.shields.io/badge/⭐-Hall%20of%20Fame-ff1493?style=flat&labelColor=000000)

**Authors:** Tri Dao et al.<br>
**Contribution:** `💾 IO-Aware Algorithm`

> Computes **exact attention with an IO-aware tiled algorithm**, reducing transfers between GPU memory and on-chip SRAM. FlashAttention’s speed and memory benefits depend on hardware and sequence length; it preserves dense attention rather than changing its quadratic arithmetic.

---

### 📄 [FlashAttention-2: Faster Attention with Better Parallelism and Work Partitioning](https://arxiv.org/abs/2307.08691)

**Authors:** Tri Dao<br>
**Contribution:** `🚀 Optimized Parallelism`

> Improves exact attention through **work partitioning and GPU parallelism**. FlashAttention-2 reports substantial gains over the original algorithm on evaluated hardware/workloads; kernel efficiency remains sensitive to hardware and tensor shape.

---

## 🚀 Inference Optimization

### 📄 [Fast Inference from Transformers via Speculative Decoding](https://arxiv.org/abs/2211.17192)

**Authors:** Yaniv Leviathan et al.<br>
**Contribution:** `🎯 Parallel Decoding`

> Uses a **draft model and parallel target-model verification** with a distribution-preserving correction procedure. Speculative decoding reduces latency when drafts are accepted efficiently; gains depend on acceptance, implementation and hardware.

---

### 📄 [Efficient Memory Management for Large Language Model Serving with PagedAttention](https://arxiv.org/abs/2309.06180)

**Authors:** Woosuk Kwon et al.<br>
**Contribution:** `💾 Memory Management`

> Introduces **PagedAttention** for non-contiguous KV-cache storage and sharing in vLLM. The reported 2–4× serving throughput is against FasterTransformer/Orca at comparable latency in tested workloads; deployment gains depend on request mix and hardware.

---

## ✂️ Pruning & Sparsity

### 📄 [SparseGPT: Massive Language Models Can Be Accurately Pruned in One-Shot](https://arxiv.org/abs/2301.00774)

**Authors:** Elias Frantar et al.<br>
**Contribution:** `✂️ One-Shot Pruning`

> Uses approximate sparse regression for **one-shot pruning** of large language models, with substantial unstructured sparsity in tested OPT/BLOOM models. SparseGPT studies compression quality without retraining; faster execution additionally needs supported sparse kernels.

---

### 📄 [A Simple and Effective Pruning Approach for Large Language Models](https://arxiv.org/abs/2306.11695)

**Authors:** Mingjie Sun et al.<br>
**Contribution:** `🎯 Simple Pruning`

> Prunes using **weight magnitude multiplied by input activation norm**, avoiding weight updates during pruning. Wanda is a simple baseline to compare with SparseGPT; calibration, sparsity pattern and supported hardware determine quality and actual inference savings.

---

### 📄 [The Unreasonable Ineffectiveness of the Deeper Layers](https://arxiv.org/abs/2403.17887)

**Authors:** Andrey Gromov et al.<br>
**Contribution:** `🔬 Layer Pruning`

> Finds that substantial blocks of deeper layers can be removed from tested LLMs with **healing fine-tuning** while preserving selected task scores. Sensitivity differs across benchmarks, especially reasoning, so pruning is not a universally lossless operation.

---

### 📄 [HAPE: Hardware-Aware LLM Pruning For Efficient On-Device Inference Optimization](https://dl.acm.org/doi/epdf/10.1145/3744244)

**Authors:** Wenqian Zhao, Lancheng Zou, Zixiao Wang, Xufeng Yao and Bei Yu (CUHK)<br>
**Contribution:** `⚙️ Hardware-Specific Pruning`

> Studies **hardware-aware structured pruning** with an optimization model for latency, sparsity and quality. The reported Llama-2-7B experiments use a Xeon 4210R CPU and H800 GPU; they do not establish phone, laptop or energy-efficiency results.

---

## ⚙️ Training Efficiency

### 📄 [Conditional Memory via Scalable Lookup: A New Axis of Sparsity for Large Language Models](https://arxiv.org/abs/2601.07372)

**Authors:** Cheng et al.<br>
**Contribution:** `🗂️ Conditional Memory`

> See the main entry in [Architectures](architectures.md) for the method, evidence and limitations.

---

### 📄 [Megatron-LM: Training Multi-Billion Parameter Language Models Using Model Parallelism](https://arxiv.org/abs/1909.08053) ![Hall of Fame](https://img.shields.io/badge/⭐-Hall%20of%20Fame-ff1493?style=flat&labelColor=000000)

**Authors:** Mohammad Shoeybi et al.<br>
**Contribution:** `⚙️ Tensor Parallelism`

> Introduces efficient **intra-layer tensor model parallelism** for multi-billion-parameter Transformer training. The original Megatron-LM report explains how to split attention and feed-forward computation across GPUs; pipeline parallelism belongs to later work.

---

### 📄 [ZeRO: Memory Optimizations Toward Training Trillion Parameter Models](https://arxiv.org/abs/1910.02054) ![Hall of Fame](https://img.shields.io/badge/⭐-Hall%20of%20Fame-ff1493?style=flat&labelColor=000000)

**Authors:** Samyam Rajbhandari, Jeff Rasley, Olatunji Ruwase and Yuxiong He (Microsoft)<br>
**Contribution:** `💾 State Partitioning`

> Partitions **optimizer states, gradients and parameters** across data-parallel workers to reduce redundant memory. ZeRO explains how memory savings interact with communication and parallelism; its trillion-parameter capacity analysis is distinct from demonstrating a trained trillion-parameter model.

---

<div align="center">

### 🌟 Contributing

Feel free to submit PRs to add more efficiency papers or improve existing entries!

### 📜 License

This repository is licensed under CC0 License.

### 🙏 Acknowledgments

Thanks to all researchers pushing the boundaries of efficient AI.

---

⭐ If you find this repository helpful, please consider giving it a star!

</div>
