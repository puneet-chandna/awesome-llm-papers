# 🎨 Multimodal Models: Vision, Language & Beyond

<div align="center">

[![Awesome](https://awesome.re/badge-flat2.svg)](https://awesome.re)
[![Works](https://img.shields.io/badge/Works-18-blue.svg)](all-papers.md)
[![Years](https://img.shields.io/badge/Years-2021--2025-green.svg)](all-papers.md)
[![License: CC0](https://img.shields.io/badge/License-CC0-yellow.svg)](../LICENSE)
[![PRs Welcome](https://img.shields.io/badge/PRs-welcome-brightgreen.svg?style=flat-square)](../CONTRIBUTING.md)

### A curated collection of groundbreaking papers bridging vision, language, and other modalities

_From foundational vision-language models to cutting-edge video understanding and generation systems._

</div>

---

## 📑 Table of Contents

- [👁️ Vision-Language Models](#%EF%B8%8F-vision-language-models)
- [🎨 Image Generation](#-image-generation)
- [🎬 Video Understanding & Generation](#-video-understanding--generation)
- [🆕 Recent Breakthroughs](#-recent-breakthroughs)

---

## 👁️ Vision-Language Models

### 📄 [Learning Transferable Visual Models From Natural Language Supervision](https://arxiv.org/abs/2103.00020) ![Hall of Fame](https://img.shields.io/badge/⭐-Hall%20of%20Fame-ff1493?style=flat&labelColor=000000)

**Authors:** Alec Radford et al. (OpenAI)<br>
**Contribution:** `🔗 Vision-Language Foundation`

> Learns **joint image/text embeddings through contrastive supervision** and evaluates zero-shot transfer using text descriptions of categories. CLIP connects language supervision to visual recognition; performance varies with distribution and remains limited on counting and abstract tasks.

---

### 📄 [Visual Instruction Tuning](https://arxiv.org/abs/2304.08485)

**Authors:** Haotian Liu et al.<br>
**Contribution:** `🎯 Visual Instruction Following`

> Connects a **CLIP vision encoder to a language model** and trains with synthetic visual instructions. LLaVA’s original data pipeline gives language-only GPT-4 captions and bounding boxes; its multimodal-chat results depend on data and evaluation design.

---

### 📄 [GPT-4 Technical Report](https://arxiv.org/abs/2303.08774) ![Hall of Fame](https://img.shields.io/badge/⭐-Hall%20of%20Fame-ff1493?style=flat&labelColor=000000)

**Authors:** OpenAI et al.<br>
**Contribution:** `🏆 Multimodal Intelligence`

> Documents **GPT-4**, a model accepting image and text inputs with text outputs, alongside capability and safety evaluations. The report limits disclosure of training and architecture; it should be distinguished from the later GPT-4V product and system card.

---

### 📄 [Flamingo: a Visual Language Model for Few-Shot Learning](https://arxiv.org/abs/2204.14198)

**Authors:** Jean-Baptiste Alayrac et al. (DeepMind)<br>
**Contribution:** `🦩 Few-Shot Visual Learning`

> Introduced **Flamingo**, a family of visual language models capable of rapid adaptation to new tasks from just a few examples. By using a novel architecture that interleaves frozen pre-trained vision and language models with learnable cross-attention layers, Flamingo achieved state-of-the-art few-shot performance on a wide range of vision-language tasks, demonstrating that in-context learning extends powerfully to the multimodal domain.

---

### 📄 [BLIP-2: Bootstrapping Language-Image Pre-training with Frozen Image Encoders and Large Language Models](https://arxiv.org/abs/2301.12597)

**Authors:** Li et al.<br>
**Contribution:** `🌉 Frozen-Model Bridge`

> Trains a **Q-Former bridge** between frozen vision and language models in two stages. It makes interface learning a practical multimodal strategy; fewer trainable parameters exclude inherited backbone training and do not imply lower total lifetime compute.

---

## 🎨 Image Generation

### 📄 [Hierarchical Text-Conditional Image Generation with CLIP Latents](https://arxiv.org/abs/2204.06125)

**Authors:** Aditya Ramesh et al.<br>
**Contribution:** `🖼️ Text-to-Image Generation`

> Generates **CLIP image latents from text, then decodes them with a diffusion model**. The DALL-E 2 paper compares prior formulations and image diversity/quality; text fidelity and fine visual details remain limitations.

---

### 📄 [High-Resolution Image Synthesis with Latent Diffusion Models](https://arxiv.org/abs/2112.10752)

**Authors:** Robin Rombach et al.<br>
**Contribution:** `🎨 Efficient Diffusion`

> Moves **diffusion into a learned compressed latent space**, reducing the cost of high-resolution image synthesis and supporting conditional generation. The original LDM paper is the research foundation for later Stable Diffusion releases, whose dates and deployment properties should be distinguished.

---

## 🎬 Video Understanding & Generation

### 📄 [VideoMAE: Masked Autoencoders are Data-Efficient Learners for Self-Supervised Video Pre-Training](https://arxiv.org/abs/2203.12602)

**Authors:** Zhan Tong et al.<br>
**Contribution:** `🎥 Video Self-Supervision`

> Extended masked autoencoding to video, demonstrating that **extremely high masking ratios (90-95%)** work remarkably well for video due to temporal redundancy. VideoMAE showed that self-supervised pre-training on video can achieve competitive results with far less data than supervised approaches, establishing an efficient paradigm for video representation learning.

---

### 📄 [Video generation models as world simulators](https://openai.com/index/video-generation-models-as-world-simulators/)

**Authors:** OpenAI<br>
**Contribution:** `🌍 World Simulation`

> An **official technical report** on Sora’s diffusion-transformer video generation and spatiotemporal patches. Its qualitative demonstrations motivate world-simulation research while explicitly showing failures in physics, object permanence and interactions.

---

### 📄 [CogVideo: Large-scale Pretraining for Text-to-Video Generation via Transformers](https://arxiv.org/abs/2205.15868)

**Authors:** Wenyi Hong et al.<br>
**Contribution:** `📹 Text-to-Video`

> Adapts a text-to-image model through **multi-frame-rate hierarchical video training**. CogVideo is a useful early large-scale text-to-video system; generated temporal coherence does not establish physical-world understanding.

---

## 🆕 Recent Breakthroughs

### 📄 [Gemini 1.5: Unlocking multimodal understanding across millions of tokens of context](https://arxiv.org/abs/2403.05530)

**Authors:** Gemini Team (Google)<br>
**Contribution:** `📚 Long-Context Multimodal`

> An **official Gemini 1.5 report** studying long multimodal context and model capabilities. Ten-million-token input is a research evaluation; strong needle-retrieval results differ from reliable reasoning over arbitrary documents and the production API window.

---

### 📄 [LLaVA-NeXT: Improved reasoning, OCR, and world knowledge](https://llava-vl.github.io/blog/2024-01-30-llava-next/)

**Authors:** Haotian Liu et al.<br>
**Contribution:** `📈 Enhanced Visual Reasoning`

> An **official LLaVA-NeXT release post** on higher-resolution visual processing and improved instruction data. Its benchmark comparisons are task-specific; the release post and available artifacts should be distinguished from a complete peer-reviewed training study.

---

### 📄 [InternVL: Scaling up Vision Foundation Models and Aligning for Generic Visual-Linguistic Tasks](https://arxiv.org/abs/2312.14238)

**Authors:** Zhe Chen et al.<br>
**Contribution:** `🔬 Scaled Vision-Language`

> Scales a **vision encoder and progressively aligns it with language models** for generic visual-linguistic tasks. InternVL offers evidence about vision-model scale and interface training; task-specific ablations should guide conclusions about which component is necessary.

---

### 📄 [Chameleon: Mixed-Modal Early-Fusion Foundation Models](https://arxiv.org/abs/2405.09818)

**Authors:** Chameleon Team (Meta FAIR)<br>
**Contribution:** `🔀 Early Fusion`

> Trains **mixed discrete image and text tokens in one early-fusion model**, with methods for stable multimodal training and interleaved generation. Chameleon extends earlier token-based multimodal work, including CM3 and CM3Leon; evaluation still exposes task and modality trade-offs.

---

### 📄 [MM1: Methods, Analysis & Insights from Multimodal LLM Pre-training](https://arxiv.org/abs/2403.09611)

**Authors:** Brandon McKinzie et al.<br>
**Contribution:** `🔬 Scientific Analysis`

> Ablates **vision encoders, image resolution/token counts, connectors and training-data mixtures** in multimodal pretraining. MM1 is valuable for experimental design: findings are tied to the authors’ tasks and model family, with smaller connector effects than several encoder/data choices.

---

### 📄 [Janus-Pro: Unified Multimodal Understanding and Generation with Data and Model Scaling](https://arxiv.org/abs/2501.17811)

**Authors:** Xiaokang Chen et al. (DeepSeek)<br>
**Contribution:** `🎭 Decoupled Pathways`

> Improves the Janus framework through **training strategy, data and model scaling** for multimodal understanding and generation. Separate visual encoders are inherited from Janus; Janus-Pro does not originate that separation or eliminate every understanding/generation trade-off.

---

### 📄 [DeepSeek-OCR: Contexts Optical Compression](https://arxiv.org/abs/2510.18234)

**Authors:** Haoran Wei, Yaofeng Sun and Yukun Li (DeepSeek)<br>
**Contribution:** `🗜️ Vision-Text Compression`

> Investigates **optical compression of text** using a vision encoder and decoder. OCR precision and throughput vary with compression ratio, page layout and hardware; preserving document text does not by itself establish downstream long-context reasoning quality.

---

### 📄 [VL-JEPA: Joint Embedding Predictive Architecture for Vision-language](https://arxiv.org/abs/2512.10942)

**Authors:** Delong Chen et al.<br>
**Contribution:** `👁️ Vision-Language Embeddings`

> Predicts **target text embeddings conditioned on visual input and a text query**, with selective text decoding. VL-JEPA studies vision-language representation learning and efficient inference; its experiments do not establish physical simulation or causal world modeling.

---

<div align="center">

### 🌟 Contributing

Feel free to submit PRs to add more multimodal papers or improve existing entries!

### 📜 License

This repository is licensed under CC0 License.

### 🙏 Acknowledgments

This list celebrates the researchers pushing the boundaries of multimodal AI.

---

⭐ If you find this repository helpful, please consider giving it a star!

</div>
