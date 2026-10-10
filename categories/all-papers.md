# 📚 All Papers - Chronological Index

<div align="center">

[![Awesome](https://awesome.re/badge-flat2.svg)](https://awesome.re)
[![Works](https://img.shields.io/badge/Works-148-blue.svg)](all-papers.md)
[![Years](https://img.shields.io/badge/Years-2000--2026-green.svg)](all-papers.md)

**One record per curated work, with useful cross-category navigation. Papers, technical reports and author research resources are labeled in their entries.**

</div>

[2026](#-2026) • [2025](#-2025) • [2024](#-2024) • [2023](#-2023) • [2022](#-2022) • [2021](#-2021) • [2020](#-2020) • [2019](#-2019) • [2018](#-2018) • [2017](#-2017) • [2014](#-2014) • [2000](#-2000)

Dates follow the earliest public paper/resource record verified in this audit; venue and revision years can differ. NNLM includes its NIPS 2000 and expanded JMLR 2003 versions as one work. ELMo’s 2017 date follows the authors’ stated OpenReview appearance. IQuest’s first report date remains uncertain; it is listed with its dated 2026 release.

---

## 📅 2026

### [Attention Residuals](https://arxiv.org/abs/2603.15031)

**Kimi Team (Guangyu Chen et al.)** • [Architectures](architectures.md)

> Uses **input-dependent aggregation across depth**, with Block AttnRes and systems optimizations for scaled training.

### [Conditional Memory via Scalable Lookup: A New Axis of Sparsity for Large Language Models](https://arxiv.org/abs/2601.07372)

**Cheng et al.** • [Architectures](architectures.md) [Efficiency](efficiency.md)

> **Engram** uses hashed n-gram lookup with contextual gating alongside neural computation.

### [IQuest-Coder-V1 Technical Report](https://github.com/IQuestLab/IQuest-Coder-V1/blob/main/papers/IQuest_Coder_Technical_Report.pdf)

**IQuest Coder Team / Yang et al.** • [Reasoning](reasoning.md) [Training](training.md)

> An **official technical report** on repository-evolution Code-Flow training and separate Instruct/Thinking post-training.

---

## 📅 2025

### [mHC: Manifold-Constrained Hyper-Connections](https://arxiv.org/abs/2512.24880)

**Zhenda Xie et al. (DeepSeek)** • [Architectures](architectures.md)

> Constrains expanded residual mixing through **doubly stochastic projections** to improve stability while preserving useful connectivity.

### [Recursive Language Models](https://arxiv.org/abs/2512.24601)

**Zhang, Kraska & Khattab** • [Rag](rag.md) [Reasoning](reasoning.md)

> Exposes a long input through a **programmable environment** and allows recursive model calls over selected pieces.

### [Close the Loop: Synthesizing Infinite Tool-Use Data via Multi-Agent Role-Playing](https://arxiv.org/abs/2512.23611)

**Yuwen Li et al.** • [Training](training.md)

> Introduces **InfTool**, combining synthetic API trajectories with gated-reward GRPO.

### [Context as a Tool: Context Management for Long-Horizon SWE-Agents](https://arxiv.org/abs/2512.22087)

**Shukai Liu et al.** • [Reasoning](reasoning.md)

> Makes **context management a callable action** for long-horizon software agents.

### [Scaling Laws for Code: Every Programming Language Matters](https://arxiv.org/abs/2512.13472)

**Jian Yang et al.** • [Analysis](analysis.md)

> Studies **language-specific code scaling** and multilingual data proportions across seven programming languages.

### [VL-JEPA: Joint Embedding Predictive Architecture for Vision-language](https://arxiv.org/abs/2512.10942)

**Delong Chen et al.** • [Multimodal](multimodal.md)

> Predicts **target text embeddings conditioned on visual input and a text query**, with selective text decoding.

### [DeepSeek-V3.2: Pushing the Frontier of Open Large Language Models](https://arxiv.org/abs/2512.02556)

**DeepSeek-AI et al.** • [Architectures](architectures.md)

> Combines **DeepSeek Sparse Attention**, scaled reinforcement learning and synthetic agent tasks in an open-weight model family.

### [DeepSeek-OCR: Contexts Optical Compression](https://arxiv.org/abs/2510.18234)

**Haoran Wei, Yaofeng Sun and Yukun Li (DeepSeek)** • [Multimodal](multimodal.md)

> Investigates **optical compression of text** using a vision encoder and decoder.

### [HAPE: Hardware-Aware LLM Pruning For Efficient On-Device Inference Optimization](https://dl.acm.org/doi/epdf/10.1145/3744244)

**Wenqian Zhao, Lancheng Zou, Zixiao Wang, Xufeng Yao and Bei Yu (CUHK)** • [Efficiency](efficiency.md)

> Studies **hardware-aware structured pruning** with an optimization model for latency, sparsity and quality.

### [The Illusion of Thinking: Understanding the Strengths and Limitations of Reasoning Models via the Lens of Problem Complexity](https://arxiv.org/abs/2506.06941)

**Parshin Shojaee et al.** • [Analysis](analysis.md)

> Studies reasoning models on controlled puzzles of increasing complexity, observing task-dependent gains and eventual failures.

### [Absolute Zero: Reinforced Self-play Reasoning with Zero Data](https://arxiv.org/abs/2505.03335)

**Andrew Zhao et al.** • [Training](training.md) [Reasoning](reasoning.md)

> Uses an executor to validate **self-proposed coding reasoning tasks** and trains through reinforced self-play.

### [Large Language Diffusion Models](https://arxiv.org/abs/2502.09992)

**Nie et al.** • [Architectures](architectures.md) [Training](training.md)

> **LLaDA** learns masked-token denoising and generates through iterative unmasking, offering a scaled alternative to autoregressive language modeling.

### [Scaling up Test-Time Compute with Latent Reasoning: A Recurrent Depth Approach](https://arxiv.org/abs/2502.05171)

**Geiping et al.** • [Architectures](architectures.md) [Reasoning](reasoning.md)

> Trains a **shared recurrent core** so inference can spend additional computation in hidden states without emitting more reasoning tokens.

### [s1: Simple Test-Time Scaling](https://arxiv.org/abs/2501.19393)

**Muennighoff et al.** • [Reasoning](reasoning.md) [Training](training.md)

> Distills a small curated reasoning set into a pretrained model and uses **budget forcing**, including “Wait” continuations, to control test-time reasoning length.

### [Janus-Pro: Unified Multimodal Understanding and Generation with Data and Model Scaling](https://arxiv.org/abs/2501.17811)

**Xiaokang Chen et al. (DeepSeek)** • [Multimodal](multimodal.md)

> Improves the Janus framework through **training strategy, data and model scaling** for multimodal understanding and generation.

### [DeepSeek-R1: Incentivizing Reasoning Capability in LLMs via Reinforcement Learning](https://arxiv.org/abs/2501.12948)

**DeepSeek-AI et al.** • [Reasoning](reasoning.md) • ![Hall of Fame](https://img.shields.io/badge/⭐-Hall%20of%20Fame-ff1493?style=flat&labelColor=000000)

> Studies reasoning-oriented reinforcement learning: **R1-Zero uses rule-based final-answer accuracy and format rewards**, rather than labels on each intermediate step.

---

## 📅 2024

### [Titans: Learning to Memorize at Test Time](https://arxiv.org/abs/2501.00663)

**Ali Behrouz, Peilin Zhong, Vahab Mirrokni** • [Architectures](architectures.md) • ![Hall of Fame](https://img.shields.io/badge/⭐-Hall%20of%20Fame-ff1493?style=flat&labelColor=000000)

> Combines local attention with **gradient-updated neural memory**, using surprise-sensitive updates, momentum and decay.

### [DeepSeek-V3 Technical Report](https://arxiv.org/abs/2412.19437)

**DeepSeek-AI** • [Architectures](architectures.md) [Training](training.md)

> Combines **MoE, multi-head latent attention, load balancing and FP8 training** in a large model system.

### [Training Large Language Models to Reason in a Continuous Latent Space](https://arxiv.org/abs/2412.06769)

**Hao et al.** • [Reasoning](reasoning.md) [Architectures](architectures.md)

> **Coconut** feeds continuous hidden states back as input embeddings and trains through a curriculum replacing verbal reasoning steps.

### [OpenAI o1 System Card](https://arxiv.org/abs/2412.16720)

**OpenAI (Aaron Jaech et al.)** • [Reasoning](reasoning.md) [Safety](safety.md)

> An **official system card** documenting o1’s capabilities, safety evaluations and mitigations.

### [Scaling LLM Test-Time Compute Optimally can be More Effective than Scaling Model Parameters](https://arxiv.org/abs/2408.03314)

**Snell et al.** • [Reasoning](reasoning.md)

> Studies **difficulty-dependent allocation** between answer revision and verifier-guided search.

### [The Llama 3 Herd of Models](https://arxiv.org/abs/2407.21783)

**Aaron Grattafiori et al.** • [Architectures](architectures.md) • ![Hall of Fame](https://img.shields.io/badge/⭐-Hall%20of%20Fame-ff1493?style=flat&labelColor=000000)

> An **official Llama 3 model-family report** covering models through 405B parameters, 128K context, post-training and safety evaluations.

### [Retrieval Augmented Generation or Long-Context LLMs? A Comprehensive Study and Hybrid Approach](https://arxiv.org/abs/2407.16833)

**Zhuowan Li et al.** • [Rag](rag.md)

> Compares retrieval-augmented generation with long-context models.

### [Scaling and evaluating sparse autoencoders](https://arxiv.org/abs/2406.04093)

**Leo Gao et al. (OpenAI)** • [Analysis](analysis.md) • ![Hall of Fame](https://img.shields.io/badge/⭐-Hall%20of%20Fame-ff1493?style=flat&labelColor=000000)

> Scales **k-sparse autoencoders** and develops evaluation tools for interpreting learned activation features.

### [Transformers are SSMs: Generalized Models and Efficient Algorithms Through Structured State Space Duality](https://arxiv.org/abs/2405.21060)

**Tri Dao et al.** • [Architectures](architectures.md)

> Develops **structured state-space duality** connecting a class of state-space models and attention formulations.

### [SimPO: Simple Preference Optimization with a Reference-Free Reward](https://arxiv.org/abs/2405.14734)

**Yu Meng et al.** • [Training](training.md)

> Optimizes preferences using **length-normalized sequence log probabilities and a target reward margin**, without a reference model.

### [Scaling Monosemanticity: Extracting Interpretable Features from Claude 3 Sonnet](https://transformer-circuits.pub/2024/scaling-monosemanticity/)

**Adly Templeton et al. (Anthropic)** • [Analysis](analysis.md)

> Uses **sparse autoencoders to extract learned features** from Claude 3 Sonnet activations.

### [Chameleon: Mixed-Modal Early-Fusion Foundation Models](https://arxiv.org/abs/2405.09818)

**Chameleon Team (Meta FAIR)** • [Multimodal](multimodal.md)

> Trains **mixed discrete image and text tokens in one early-fusion model**, with methods for stable multimodal training and interleaved generation.

### [From Local to Global: A Graph RAG Approach to Query-Focused Summarization](https://arxiv.org/abs/2404.16130)

**Darren Edge et al. (Microsoft)** • [Rag](rag.md)

> Builds entity graphs and hierarchical community summaries for **global, query-focused summarization**.

### [Leave No Context Behind: Efficient Infinite Context Transformers with Infini-attention](https://arxiv.org/abs/2404.07143)

**Tsendsuren Munkhdalai et al.** • [Rag](rag.md)

> Combines **local attention and compressive memory** to process successive segments with bounded working memory.

### [Mixture-of-Depths: Dynamically allocating compute in transformer-based language models](https://arxiv.org/abs/2404.02258)

**David Raposo et al.** • [Architectures](architectures.md)

> Uses learned token routing with a **fixed top-k compute budget** at selected layers.

### [Many-shot Jailbreaking](https://www-cdn.anthropic.com/af5633c94ed2beb282f6a53c595eb437e8e7b630/Many_Shot_Jailbreaking__2024_04_02_0936.pdf)

**Cem Anil et al. (Anthropic)** • [Safety](safety.md)

> An **author research report** studying how many in-context demonstrations can induce harmful responses.

### [Jamba: A Hybrid Transformer-Mamba Language Model](https://arxiv.org/abs/2403.19887)

**Opher Lieber et al.** • [Architectures](architectures.md)

> Combines **attention, Mamba and MoE layers** in a hybrid language model.

### [The Unreasonable Ineffectiveness of the Deeper Layers](https://arxiv.org/abs/2403.17887)

**Andrey Gromov et al.** • [Efficiency](efficiency.md)

> Finds that substantial blocks of deeper layers can be removed from tested LLMs with **healing fine-tuning** while preserving selected task scores.

### [MM1: Methods, Analysis & Insights from Multimodal LLM Pre-training](https://arxiv.org/abs/2403.09611)

**Brandon McKinzie et al.** • [Multimodal](multimodal.md)

> Ablates **vision encoders, image resolution/token counts, connectors and training-data mixtures** in multimodal pretraining.

### [ORPO: Monolithic Preference Optimization without Reference Model](https://arxiv.org/abs/2403.07691)

**Jiwoo Hong, Noah Lee and James Thorne** • [Training](training.md)

> Combines a **supervised likelihood objective with an odds-ratio preference penalty** in one reference-free training stage.

### [The Era of 1-bit LLMs: All Large Language Models are in 1.58 Bits](https://arxiv.org/abs/2402.17764)

**Shuming Ma et al. (Microsoft Research)** • [Efficiency](efficiency.md)

> Studies **BitNet b1.58**, whose trained weights are ternary (−1, 0, +1) with quantization-aware computation.

### [Video generation models as world simulators](https://openai.com/index/video-generation-models-as-world-simulators/)

**OpenAI** • [Multimodal](multimodal.md)

> An **official technical report** on Sora’s diffusion-transformer video generation and spatiotemporal patches.

### [Gemini 1.5: Unlocking multimodal understanding across millions of tokens of context](https://arxiv.org/abs/2403.05530)

**Gemini Team (Google)** • [Multimodal](multimodal.md)

> An **official Gemini 1.5 report** studying long multimodal context and model capabilities.

### [Direct Language Model Alignment from Online AI Feedback](https://arxiv.org/abs/2402.04792)

**Shangmin Guo et al.** • [Training](training.md)

> Generates **online preference comparisons with an AI judge** while adapting the language model.

### [DeepSeekMath: Pushing the Limits of Mathematical Reasoning in Open Language Models](https://arxiv.org/abs/2402.03300)

**Zhihong Shao et al.** • [Reasoning](reasoning.md) • ![Hall of Fame](https://img.shields.io/badge/⭐-Hall%20of%20Fame-ff1493?style=flat&labelColor=000000)

> Presents DeepSeekMath and **Group Relative Policy Optimization (GRPO)**, which estimates relative advantages from groups of sampled solutions without a separate critic.

### [KTO: Model Alignment as Prospect Theoretic Optimization](https://arxiv.org/abs/2402.01306)

**Kawin Ethayarajh et al.** • [Training](training.md)

> Derives **Kahneman–Tversky Optimization**, a utility-inspired objective that uses desirable/undesirable labels rather than paired preferences.

### [OLMo: Accelerating the Science of Language Models](https://arxiv.org/abs/2402.00838)

**Dirk Groeneveld et al. (AI2)** • [Training](training.md) • ![Hall of Fame](https://img.shields.io/badge/⭐-Hall%20of%20Fame-ff1493?style=flat&labelColor=000000)

> Releases **OLMo weights, training code, data and evaluation tooling** to support open language-model research.

### [LLaVA-NeXT: Improved reasoning, OCR, and world knowledge](https://llava-vl.github.io/blog/2024-01-30-llava-next/)

**Haotian Liu et al.** • [Multimodal](multimodal.md)

> An **official LLaVA-NeXT release post** on higher-resolution visual processing and improved instruction data.

### [Self-Rewarding Language Models](https://arxiv.org/abs/2401.10020)

**Weizhe Yuan et al.** • [Training](training.md)

> Uses an **LLM-as-judge to create preference pairs** for iterative DPO.

### [Sleeper Agents: Training Deceptive LLMs that Persist Through Safety Training](https://arxiv.org/abs/2401.05566)

**Hubinger et al.** • [Safety](safety.md)

> Constructs **trigger-dependent backdoors** and tests their persistence through supervised, reinforcement and adversarial safety training.

### [Mixtral of Experts](https://arxiv.org/abs/2401.04088)

**Albert Q. Jiang et al. (Mistral AI)** • [Architectures](architectures.md)

> Reports **Mixtral 8×7B**, routing each token to two experts with about 13B active of 46.7B total parameters.

### [Self-Play Fine-Tuning Converts Weak Language Models to Strong Language Models](https://arxiv.org/abs/2401.01335)

**Zixiang Chen et al.** • [Training](training.md)

> Iteratively trains a policy to distinguish **human demonstration responses from its own generated responses**.

### [RAPTOR: Recursive Abstractive Processing for Tree-Organized Retrieval](https://arxiv.org/abs/2401.18059)

**Parth Sarthi et al.** • [Rag](rag.md)

> Proposed a novel approach to organizing retrieved information in a **hierarchical tree structure**.

---

## 📅 2023

### [InternVL: Scaling up Vision Foundation Models and Aligning for Generic Visual-Linguistic Tasks](https://arxiv.org/abs/2312.14238)

**Zhe Chen et al.** • [Multimodal](multimodal.md)

> Scales a **vision encoder and progressively aligns it with language models** for generic visual-linguistic tasks.

### [Mamba: Linear-Time Sequence Modeling with Selective State Spaces](https://arxiv.org/abs/2312.00752)

**Albert Gu and Tri Dao** • [Architectures](architectures.md) • ![Hall of Fame](https://img.shields.io/badge/⭐-Hall%20of%20Fame-ff1493?style=flat&labelColor=000000)

> Makes **state-space parameters input-dependent** and uses a hardware-aware scan for sequence modeling.

### [Self-RAG: Learning to Retrieve, Generate, and Critique through Self-Reflection](https://arxiv.org/abs/2310.11511)

**Akari Asai et al.** • [Rag](rag.md)

> Trains a model to generate **retrieval and reflection tokens**, allowing adaptive retrieval and assessment of passages and answers.

### [MemGPT: Towards LLMs as Operating Systems](https://arxiv.org/abs/2310.08560)

**Charles Packer et al.** • [Rag](rag.md)

> Treats context as a **managed memory hierarchy**, paging between a bounded prompt and external storage.

### [Mistral 7B](https://arxiv.org/abs/2310.06825)

**Albert Q. Jiang et al.** • [Architectures](architectures.md) • ![Hall of Fame](https://img.shields.io/badge/⭐-Hall%20of%20Fame-ff1493?style=flat&labelColor=000000)

> Combines **grouped-query attention and sliding-window attention** in the Mistral 7B model.

### [Ring Attention with Blockwise Transformers for Near-Infinite Context](https://arxiv.org/abs/2310.01889)

**Hao Liu et al.** • [Rag](rag.md)

> Distributes blockwise attention across devices in a **ring**, overlapping computation with communication.

### [Representation Engineering: A Top-Down Approach to AI Transparency](https://arxiv.org/abs/2310.01405)

**Andy Zou et al.** • [Analysis](analysis.md)

> Uses **representation reading and control** to identify and steer high-level concepts in model activations.

### [LongLoRA: Efficient Fine-tuning of Long-Context Large Language Models](https://arxiv.org/abs/2309.12307)

**Yukang Chen et al.** • [Rag](rag.md)

> Combines **shifted sparse attention during fine-tuning** with parameter-efficient adaptation for long context.

### [Efficient Memory Management for Large Language Model Serving with PagedAttention](https://arxiv.org/abs/2309.06180)

**Woosuk Kwon et al.** • [Efficiency](efficiency.md)

> Introduces **PagedAttention** for non-contiguous KV-cache storage and sharing in vLLM.

### [Graph of Thoughts: Solving Elaborate Problems with Large Language Models](https://arxiv.org/abs/2308.09687)

**Maciej Besta et al.** • [Reasoning](reasoning.md)

> Organizes generated thoughts as a **graph**, supporting aggregation, refinement and reuse of intermediate solutions.

### [Universal and Transferable Adversarial Attacks on Aligned Language Models](https://arxiv.org/abs/2307.15043)

**Andy Zou et al.** • [Safety](safety.md)

> Optimizes **adversarial suffixes** against aligned models and studies their transfer across models and interfaces.

### [Llama 2: Open Foundation and Fine-Tuned Chat Models](https://arxiv.org/abs/2307.09288)

**Hugo Touvron et al. (Meta)** • [Architectures](architectures.md) • ![Hall of Fame](https://img.shields.io/badge/⭐-Hall%20of%20Fame-ff1493?style=flat&labelColor=000000)

> An **official Llama 2 report** on pretrained and chat-tuned open-weight models, including preference training and safety evaluations.

### [Retentive Network: A Successor to Transformer for Large Language Models](https://arxiv.org/abs/2307.08621)

**Yutao Sun et al.** • [Architectures](architectures.md)

> Introduces **retention** with parallel training, recurrent decoding and chunkwise computation.

### [FlashAttention-2: Faster Attention with Better Parallelism and Work Partitioning](https://arxiv.org/abs/2307.08691)

**Tri Dao** • [Efficiency](efficiency.md)

> Improves exact attention through **work partitioning and GPU parallelism**.

### [Lost in the Middle: How Language Models Use Long Contexts](https://arxiv.org/abs/2307.03172)

**Liu et al.** • [Rag](rag.md) [Analysis](analysis.md)

> Varies relevant-information position in **multi-document QA and key-value retrieval**, finding weaker use of middle positions in many tested models.

### [Jailbroken: How Does LLM Safety Training Fail?](https://arxiv.org/abs/2307.02483)

**Alexander Wei, Nika Haghtalab and Jacob Steinhardt (UC Berkeley)** • [Safety](safety.md)

> Analyzes **competing objectives and mismatched generalization** as two routes to jailbreak failures.

### [Extending Context Window of Large Language Models via Positional Interpolation](https://arxiv.org/abs/2306.15595)

**Shouyuan Chen et al. (Meta AI)** • [Rag](rag.md)

> Extends RoPE-based context through **position interpolation**, mapping positions back into the original range before fine-tuning.

### [A Simple and Effective Pruning Approach for Large Language Models](https://arxiv.org/abs/2306.11695)

**Mingjie Sun et al.** • [Efficiency](efficiency.md)

> Prunes using **weight magnitude multiplied by input activation norm**, avoiding weight updates during pruning.

### [Augmenting Language Models with Long-Term Memory](https://arxiv.org/abs/2306.07174)

**Weizhi Wang et al.** • [Rag](rag.md)

> Uses a **frozen backbone as memory encoder** and a trainable SideNet to retrieve and read cached representations.

### [Judging LLM-as-a-Judge with MT-Bench and Chatbot Arena](https://arxiv.org/abs/2306.05685)

**Lianmin Zheng et al.** • [Analysis](analysis.md)

> Studies **LLM judging, MT-Bench and crowdsourced pairwise Chatbot Arena comparisons**.

### [AWQ: Activation-aware Weight Quantization for LLM Compression and Acceleration](https://arxiv.org/abs/2306.00978)

**Ji Lin et al.** • [Efficiency](efficiency.md)

> Uses activation statistics to identify **quantization-sensitive channels**, then scales channels to reduce low-bit error.

### [Let's Verify Step by Step](https://arxiv.org/abs/2305.20050)

**Lightman et al.** • [Reasoning](reasoning.md) [Training](training.md)

> Compares **process and outcome supervision** for ranking math solutions and releases PRM800K step labels.

### [Direct Preference Optimization: Your Language Model is Secretly a Reward Model](https://arxiv.org/abs/2305.18290)

**Rafael Rafailov et al.** • [Training](training.md) • ![Hall of Fame](https://img.shields.io/badge/⭐-Hall%20of%20Fame-ff1493?style=flat&labelColor=000000)

> Derives an **offline preference objective through the policy’s implicit reward relation**, avoiding a separately fitted reward model and online RL loop.

### [QLoRA: Efficient Finetuning of Quantized LLMs](https://arxiv.org/abs/2305.14314)

**Tim Dettmers et al.** • [Efficiency](efficiency.md) [Training](training.md)

> Combined 4-bit quantization with LoRA to enable **fine-tuning of 65B parameter models on a single 48GB GPU**.

### [RWKV: Reinventing RNNs for the Transformer Era](https://arxiv.org/abs/2305.13048)

**Bo Peng et al.** • [Architectures](architectures.md)

> Combines parallelizable training with **recurrent decoding and a fixed-size state**.

### [Tree of Thoughts: Deliberate Problem Solving with Large Language Models](https://arxiv.org/abs/2305.10601)

**Shunyu Yao et al.** • [Reasoning](reasoning.md)

> Searches a **tree of candidate thoughts**, using evaluation and backtracking in tasks such as Game24 and mini crosswords.

### [Language Models Don't Always Say What They Think: Unfaithful Explanations in Chain-of-Thought Prompting](https://arxiv.org/abs/2305.04388)

**Miles Turpin et al.** • [Analysis](analysis.md)

> Introduces biasing features that alter answers without being acknowledged in **generated chain-of-thought explanations**.

### [Are Emergent Abilities of Large Language Models a Mirage?](https://arxiv.org/abs/2304.15004)

**Rylan Schaeffer, Brando Miranda and Sanmi Koyejo** • [Analysis](analysis.md)

> Shows how **metric choice can create apparent emergence** in studied tasks and model families.

### [Visual Instruction Tuning](https://arxiv.org/abs/2304.08485)

**Haotian Liu et al.** • [Multimodal](multimodal.md)

> Connects a **CLIP vision encoder to a language model** and trains with synthetic visual instructions.

### [Pythia: A Suite for Analyzing Large Language Models Across Training and Scaling](https://arxiv.org/abs/2304.01373)

**Biderman et al.** • [Analysis](analysis.md) [Training](training.md)

> Releases **model suites, training checkpoints and data-order tooling** for studying learning dynamics and scale.

### [Reflexion: Language Agents with Verbal Reinforcement Learning](https://arxiv.org/abs/2303.11366)

**Noah Shinn et al.** • [Reasoning](reasoning.md)

> Enabled agents to **learn from their mistakes through verbal self-reflection**.

### [GPT-4 Technical Report](https://arxiv.org/abs/2303.08774)

**OpenAI et al.** • [Multimodal](multimodal.md) • ![Hall of Fame](https://img.shields.io/badge/⭐-Hall%20of%20Fame-ff1493?style=flat&labelColor=000000)

> Documents **GPT-4**, a model accepting image and text inputs with text outputs, alongside capability and safety evaluations.

### [Stanford Alpaca: An Instruction-following LLaMA Model](https://github.com/tatsu-lab/stanford_alpaca)

**Rohan Taori et al. (Stanford)** • [Training](training.md)

> An **official project resource** demonstrating instruction adaptation of LLaMA using 52K generated examples.

### [LLaMA: Open and Efficient Foundation Language Models](https://arxiv.org/abs/2302.13971)

**Hugo Touvron et al.** • [Architectures](architectures.md) • ![Hall of Fame](https://img.shields.io/badge/⭐-Hall%20of%20Fame-ff1493?style=flat&labelColor=000000)

> Releases **LLaMA research-access model weights** and studies data-efficient autoregressive training across several sizes.

### [Hyena Hierarchy: Towards Larger Convolutional Language Models](https://arxiv.org/abs/2302.10866)

**Michael Poli et al.** • [Architectures](architectures.md)

> Proposes **Hyena**, a subquadratic replacement for attention based on long convolutions and data-controlled gating.

### [Toolformer: Language Models Can Teach Themselves to Use Tools](https://arxiv.org/abs/2302.04761)

**Timo Schick et al.** • [Reasoning](reasoning.md)

> Uses a few API demonstrations to seed **self-supervised tool-call generation and filtering**, then trains a model to use the retained calls.

### [BLIP-2: Bootstrapping Language-Image Pre-training with Frozen Image Encoders and Large Language Models](https://arxiv.org/abs/2301.12597)

**Li et al.** • [Multimodal](multimodal.md)

> Trains a **Q-Former bridge** between frozen vision and language models in two stages.

### [SparseGPT: Massive Language Models Can Be Accurately Pruned in One-Shot](https://arxiv.org/abs/2301.00774)

**Elias Frantar et al.** • [Efficiency](efficiency.md)

> Uses approximate sparse regression for **one-shot pruning** of large language models, with substantial unstructured sparsity in tested OPT/BLOOM models.

---

## 📅 2022

### [Self-Instruct: Aligning Language Models with Self-Generated Instructions](https://arxiv.org/abs/2212.10560)

**Yizhong Wang et al.** • [Training](training.md)

> Bootstraps **instructions, inputs and responses** from a small human-written seed, filters them and fine-tunes on the resulting synthetic data.

### [Constitutional AI: Harmlessness from AI Feedback](https://arxiv.org/abs/2212.08073)

**Yuntao Bai et al. (Anthropic)** • [Training](training.md) [Safety](safety.md) • ![Hall of Fame](https://img.shields.io/badge/⭐-Hall%20of%20Fame-ff1493?style=flat&labelColor=000000)

> Uses constitutional principles for **critique/revision and AI harmlessness preferences**, while retaining human helpfulness feedback.

### [Fast Inference from Transformers via Speculative Decoding](https://arxiv.org/abs/2211.17192)

**Yaniv Leviathan et al.** • [Efficiency](efficiency.md)

> Uses a **draft model and parallel target-model verification** with a distribution-preserving correction procedure.

### [Holistic Evaluation of Language Models](https://arxiv.org/abs/2211.09110)

**Percy Liang et al.** • [Analysis](analysis.md)

> Proposed **HELM**, a framework for evaluating LLMs across multiple dimensions simultaneously—accuracy, calibration, robustness, fairness, efficiency, and more.

### [BLOOM: A 176B-Parameter Open-Access Multilingual Language Model](https://arxiv.org/abs/2211.05100)

**BigScience Workshop et al.** • [Architectures](architectures.md) • ![Hall of Fame](https://img.shields.io/badge/⭐-Hall%20of%20Fame-ff1493?style=flat&labelColor=000000)

> An **official report on BLOOM**, a 176B multilingual model developed through the BigScience collaboration.

### [GPTQ: Accurate Post-Training Quantization for Generative Pre-trained Transformers](https://arxiv.org/abs/2210.17323)

**Elias Frantar et al.** • [Efficiency](efficiency.md)

> Uses approximate second-order information for **one-shot, layer-wise weight quantization**.

### [Scaling Instruction-Finetuned Language Models](https://arxiv.org/abs/2210.11416)

**Hyung Won Chung et al. (Google)** • [Training](training.md)

> Scaled instruction tuning to 1,800+ tasks and demonstrated that **instruction tuning benefits scale with both model size and number of tasks**.

### [Scaling Laws for Reward Model Overoptimization](https://arxiv.org/abs/2210.10760)

**Gao, Schulman & Hilton** • [Analysis](analysis.md) [Training](training.md)

> Measures how stronger optimization of an imperfect **proxy reward** can eventually reduce a synthetic gold-model reward under best-of-N and PPO.

### [ReAct: Synergizing Reasoning and Acting in Language Models](https://arxiv.org/abs/2210.03629)

**Shunyu Yao et al.** • [Reasoning](reasoning.md)

> Interleaves **reasoning traces, actions and observations** in knowledge and decision tasks.

### [Emergent Abilities of Large Language Models](https://arxiv.org/abs/2206.07682)

**Jason Wei et al.** • [Analysis](analysis.md) • ![Hall of Fame](https://img.shields.io/badge/⭐-Hall%20of%20Fame-ff1493?style=flat&labelColor=000000)

> Catalogues **emergent abilities as measured on selected tasks**, where scores appear abruptly with scale.

### [Beyond the Imitation Game: Quantifying and extrapolating the capabilities of language models](https://arxiv.org/abs/2206.04615)

**Aarohi Srivastava et al. (BIG-bench collaboration)** • [Analysis](analysis.md)

> Introduces **BIG-bench**, a collaborative collection of over 200 tasks probing diverse language-model capabilities.

### [CogVideo: Large-scale Pretraining for Text-to-Video Generation via Transformers](https://arxiv.org/abs/2205.15868)

**Wenyi Hong et al.** • [Multimodal](multimodal.md)

> Adapts a text-to-image model through **multi-frame-rate hierarchical video training**.

### [FlashAttention: Fast and Memory-Efficient Exact Attention with IO-Awareness](https://arxiv.org/abs/2205.14135)

**Tri Dao et al.** • [Efficiency](efficiency.md) • ![Hall of Fame](https://img.shields.io/badge/⭐-Hall%20of%20Fame-ff1493?style=flat&labelColor=000000)

> Computes **exact attention with an IO-aware tiled algorithm**, reducing transfers between GPU memory and on-chip SRAM.

### [Large Language Models are Zero-Shot Reasoners](https://arxiv.org/abs/2205.11916)

**Kojima et al.** • [Reasoning](reasoning.md) • ![Hall of Fame](https://img.shields.io/badge/⭐-Hall%20of%20Fame-ff1493?style=flat&labelColor=000000)

> Uses a **reasoning instruction followed by answer extraction** without worked demonstrations.

### [Flamingo: a Visual Language Model for Few-Shot Learning](https://arxiv.org/abs/2204.14198)

**Jean-Baptiste Alayrac et al. (DeepMind)** • [Multimodal](multimodal.md)

> Introduced **Flamingo**, a family of visual language models capable of rapid adaptation to new tasks from just a few examples.

### [Hierarchical Text-Conditional Image Generation with CLIP Latents](https://arxiv.org/abs/2204.06125)

**Aditya Ramesh et al.** • [Multimodal](multimodal.md)

> Generates **CLIP image latents from text, then decodes them with a diffusion model**.

### [PaLM: Scaling Language Modeling with Pathways](https://arxiv.org/abs/2204.02311)

**Aakanksha Chowdhery et al.** • [Architectures](architectures.md) • ![Hall of Fame](https://img.shields.io/badge/⭐-Hall%20of%20Fame-ff1493?style=flat&labelColor=000000)

> Reports **PaLM**, a 540B dense model trained with Pathways, and evaluates few-shot language and reasoning tasks.

### [Training Compute-Optimal Large Language Models](https://arxiv.org/abs/2203.15556)

**Jordan Hoffmann et al.** • [Analysis](analysis.md) • ![Hall of Fame](https://img.shields.io/badge/⭐-Hall%20of%20Fame-ff1493?style=flat&labelColor=000000)

> Studies **compute-optimal allocation between parameter count and training tokens** under a fixed pretraining budget.

### [STaR: Bootstrapping Reasoning With Reasoning](https://arxiv.org/abs/2203.14465)

**Zelikman et al.** • [Training](training.md) [Reasoning](reasoning.md)

> Iterates **answer-filtered rationale generation and fine-tuning**, using known answers to rationalize failed attempts.

### [VideoMAE: Masked Autoencoders are Data-Efficient Learners for Self-Supervised Video Pre-Training](https://arxiv.org/abs/2203.12602)

**Zhan Tong et al.** • [Multimodal](multimodal.md)

> Extended masked autoencoding to video, demonstrating that **extremely high masking ratios (90-95%)** work remarkably well for video due to temporal redundancy.

### [Self-Consistency Improves Chain of Thought Reasoning in Language Models](https://arxiv.org/abs/2203.11171)

**Wang et al.** • [Reasoning](reasoning.md) • ![Hall of Fame](https://img.shields.io/badge/⭐-Hall%20of%20Fame-ff1493?style=flat&labelColor=000000)

> Samples **diverse reasoning paths and aggregates final answers** rather than using a single greedy chain.

### [Training language models to follow instructions with human feedback](https://arxiv.org/abs/2203.02155)

**Long Ouyang et al.** • [Training](training.md) • ![Hall of Fame](https://img.shields.io/badge/⭐-Hall%20of%20Fame-ff1493?style=flat&labelColor=000000)

> Trains **InstructGPT** through human demonstrations, preference reward modeling and PPO, with a pretraining-mix variant.

### [In-context Learning and Induction Heads](https://transformer-circuits.pub/2022/in-context-learning-and-induction-heads/index.html)

**Catherine Olsson et al. (Anthropic)** • [Analysis](analysis.md)

> Studies **induction-head circuits** that match and continue repeated patterns, with evidence linking their formation to aspects of in-context learning.

### [Chain-of-Thought Prompting Elicits Reasoning in Large Language Models](https://arxiv.org/abs/2201.11903)

**Jason Wei et al. (Google)** • [Reasoning](reasoning.md) • ![Hall of Fame](https://img.shields.io/badge/⭐-Hall%20of%20Fame-ff1493?style=flat&labelColor=000000)

> Shows that **worked reasoning demonstrations** can improve arithmetic, commonsense and symbolic tasks without weight updates.

### [LaMDA: Language Models for Dialog Applications](https://arxiv.org/abs/2201.08239)

**Romal Thoppilan et al.** • [Architectures](architectures.md) • ![Hall of Fame](https://img.shields.io/badge/⭐-Hall%20of%20Fame-ff1493?style=flat&labelColor=000000)

> An **official LaMDA dialogue-model report**, combining web/dialogue pretraining, fine-tuning and tools for factual grounding.

### [Memorizing Transformers](https://arxiv.org/abs/2203.08913)

**Yuhuai Wu, Markus N. Rabe, DeLesley Hutchins and Christian Szegedy (Google)** • [Rag](rag.md)

> Augmented Transformers with a **kNN-based external memory** that stores and retrieves past key-value pairs.

---

## 📅 2021

### [A Mathematical Framework for Transformer Circuits](https://transformer-circuits.pub/2021/framework/index.html)

**Nelson Elhage et al. (Anthropic)** • [Analysis](analysis.md)

> An **author research article** developing a circuit view of attention-only Transformers, including residual streams and information movement through heads.

### [High-Resolution Image Synthesis with Latent Diffusion Models](https://arxiv.org/abs/2112.10752)

**Robin Rombach et al.** • [Multimodal](multimodal.md)

> Moves **diffusion into a learned compressed latent space**, reducing the cost of high-resolution image synthesis and supporting conditional generation.

### [Scaling Language Models: Methods, Analysis & Insights from Training Gopher](https://arxiv.org/abs/2112.11446)

**Jack W. Rae et al.** • [Analysis](analysis.md) • ![Hall of Fame](https://img.shields.io/badge/⭐-Hall%20of%20Fame-ff1493?style=flat&labelColor=000000)

> An **official Gopher report** studying a 280B model across a broad task suite.

### [Training Verifiers to Solve Math Word Problems](https://arxiv.org/abs/2110.14168)

**Cobbe et al.** • [Reasoning](reasoning.md) [Analysis](analysis.md) • ![Hall of Fame](https://img.shields.io/badge/⭐-Hall%20of%20Fame-ff1493?style=flat&labelColor=000000)

> Introduces **GSM8K and learned verification** to select among sampled math solutions.

### [Finetuned Language Models Are Zero-Shot Learners](https://arxiv.org/abs/2109.01652)

**Jason Wei et al. (Google)** • [Training](training.md) • ![Hall of Fame](https://img.shields.io/badge/⭐-Hall%20of%20Fame-ff1493?style=flat&labelColor=000000)

> Fine-tunes a language model on **tasks expressed through natural-language instructions** and evaluates held-out task families.

### [On the Opportunities and Risks of Foundation Models](https://arxiv.org/abs/2108.07258)

**Rishi Bommasani et al.** • [Analysis](analysis.md) • ![Hall of Fame](https://img.shields.io/badge/⭐-Hall%20of%20Fame-ff1493?style=flat&labelColor=000000)

> A **research report and perspective** defining foundation models and examining adaptation, homogenization and societal risks.

### [Evaluating Large Language Models Trained on Code](https://arxiv.org/abs/2107.03374)

**Mark Chen et al. (OpenAI)** • [Reasoning](reasoning.md) • ![Hall of Fame](https://img.shields.io/badge/⭐-Hall%20of%20Fame-ff1493?style=flat&labelColor=000000)

> Studies **Codex code generation** and introduces HumanEval with execution-based functional correctness and sampling metrics.

### [LoRA: Low-Rank Adaptation of Large Language Models](https://arxiv.org/abs/2106.09685)

**Edward J. Hu et al.** • [Training](training.md) • ![Hall of Fame](https://img.shields.io/badge/⭐-Hall%20of%20Fame-ff1493?style=flat&labelColor=000000)

> Freezes pretrained weights and trains **low-rank updates** to selected weight matrices.

### [RoFormer: Enhanced Transformer with Rotary Position Embedding](https://arxiv.org/abs/2104.09864)

**Jianlin Su et al.** • [Rag](rag.md)

> Introduces **rotary positional embeddings (RoPE)**, combining absolute rotations with relative-position effects in attention scores.

### [Switch Transformers: Scaling to Trillion Parameter Models with Simple and Efficient Sparsity](https://arxiv.org/abs/2101.03961)

**William Fedus, Barret Zoph and Noam Shazeer (Google)** • [Architectures](architectures.md) • ![Hall of Fame](https://img.shields.io/badge/⭐-Hall%20of%20Fame-ff1493?style=flat&labelColor=000000)

> Simplifies sparse MoE routing to **one selected expert per token**, with training and load-balancing methods for large models.

### [Learning Transferable Visual Models From Natural Language Supervision](https://arxiv.org/abs/2103.00020)

**Alec Radford et al. (OpenAI)** • [Multimodal](multimodal.md) • ![Hall of Fame](https://img.shields.io/badge/⭐-Hall%20of%20Fame-ff1493?style=flat&labelColor=000000)

> Learns **joint image/text embeddings through contrastive supervision** and evaluates zero-shot transfer using text descriptions of categories.

### [Prefix-Tuning: Optimizing Continuous Prompts for Generation](https://arxiv.org/abs/2101.00190)

**Xiang Lisa Li et al.** • [Training](training.md)

> Learns **continuous prefixes of activations** while keeping the pretrained model frozen.

---

## 📅 2020

### [Measuring Massive Multitask Language Understanding](https://arxiv.org/abs/2009.03300)

**Dan Hendrycks et al.** • [Analysis](analysis.md)

> Introduces **MMLU**, multiple-choice evaluation across 57 academic and professional subjects.

### [Learning to Summarize from Human Feedback](https://arxiv.org/abs/2009.01325)

**Stiennon et al.** • [Training](training.md)

> Trains a **summary preference model** from human comparisons, then optimizes a summarizer against it.

### [Language Models are Few-Shot Learners](https://arxiv.org/abs/2005.14165)

**Tom B. Brown et al.** • [Architectures](architectures.md) • ![Hall of Fame](https://img.shields.io/badge/⭐-Hall%20of%20Fame-ff1493?style=flat&labelColor=000000)

> Evaluated **GPT-3** across zero-, one- and few-shot tasks without task-specific weight updates.

### [Retrieval-Augmented Generation for Knowledge-Intensive NLP Tasks](https://arxiv.org/abs/2005.11401)

**Patrick Lewis et al.** • [Rag](rag.md) • ![Hall of Fame](https://img.shields.io/badge/⭐-Hall%20of%20Fame-ff1493?style=flat&labelColor=000000)

> Combines a **dense retriever with a sequence generator**, marginalizing over retrieved passages for knowledge-intensive tasks.

### [REALM: Retrieval-Augmented Language Model Pre-Training](https://arxiv.org/abs/2002.08909)

**Kelvin Guu et al. (Google Research)** • [Rag](rag.md)

> Pioneered the concept of **pre-training language models with retrieval**.

### [Scaling Laws for Neural Language Models](https://arxiv.org/abs/2001.08361)

**Jared Kaplan et al. (OpenAI)** • [Analysis](analysis.md) • ![Hall of Fame](https://img.shields.io/badge/⭐-Hall%20of%20Fame-ff1493?style=flat&labelColor=000000)

> Fits empirical **language-model loss scaling** with parameters, data and compute over measured regimes.

---

## 📅 2019

### [Exploring the Limits of Transfer Learning with a Unified Text-to-Text Transformer](https://arxiv.org/abs/1910.10683)

**Colin Raffel et al.** • [Architectures](architectures.md) • ![Hall of Fame](https://img.shields.io/badge/⭐-Hall%20of%20Fame-ff1493?style=flat&labelColor=000000)

> Studies a **unified text-to-text task format**, pretraining objectives, data and transfer learning in T5.

### [ZeRO: Memory Optimizations Toward Training Trillion Parameter Models](https://arxiv.org/abs/1910.02054)

**Samyam Rajbhandari, Jeff Rasley, Olatunji Ruwase and Yuxiong He (Microsoft)** • [Efficiency](efficiency.md) • ![Hall of Fame](https://img.shields.io/badge/⭐-Hall%20of%20Fame-ff1493?style=flat&labelColor=000000)

> Partitions **optimizer states, gradients and parameters** across data-parallel workers to reduce redundant memory.

### [Megatron-LM: Training Multi-Billion Parameter Language Models Using Model Parallelism](https://arxiv.org/abs/1909.08053)

**Mohammad Shoeybi et al.** • [Efficiency](efficiency.md) [Training](training.md) • ![Hall of Fame](https://img.shields.io/badge/⭐-Hall%20of%20Fame-ff1493?style=flat&labelColor=000000)

> Introduces efficient **intra-layer tensor model parallelism** for multi-billion-parameter Transformer training.

### [Universal Adversarial Triggers for Attacking and Analyzing NLP](https://arxiv.org/abs/1908.07125)

**Eric Wallace et al.** • [Safety](safety.md)

> Finds **input-agnostic adversarial token triggers** that degrade tested NLP systems and expose learned associations.

### [Language Models are Unsupervised Multitask Learners](https://cdn.openai.com/better-language-models/language_models_are_unsupervised_multitask_learners.pdf)

**Alec Radford et al. (OpenAI)** • [Architectures](architectures.md) • ![Hall of Fame](https://img.shields.io/badge/⭐-Hall%20of%20Fame-ff1493?style=flat&labelColor=000000)

> An **official GPT-2 report** evaluating autoregressive language modeling as unsupervised multitask learning.

### [Transformer-XL: Attentive Language Models Beyond a Fixed-Length Context](https://arxiv.org/abs/1901.02860)

**Dai et al.** • [Rag](rag.md) [Architectures](architectures.md) • ![Hall of Fame](https://img.shields.io/badge/⭐-Hall%20of%20Fame-ff1493?style=flat&labelColor=000000)

> Combines **segment-level recurrence and relative positional encoding** to reuse prior hidden states beyond a fixed training segment.

---

## 📅 2018

### [BERT: Pre-training of Deep Bidirectional Transformers for Language Understanding](https://arxiv.org/abs/1810.04805)

**Jacob Devlin et al. (Google)** • [Architectures](architectures.md) • ![Hall of Fame](https://img.shields.io/badge/⭐-Hall%20of%20Fame-ff1493?style=flat&labelColor=000000)

> Pretrains a **bidirectional Transformer encoder** with masked-language modeling and a sentence-level objective, then adapts it to downstream tasks.

### [Improving Language Understanding by Generative Pre-Training](https://cdn.openai.com/research-covers/language-unsupervised/language_understanding_paper.pdf)

**Alec Radford, Karthik Narasimhan, Tim Salimans and Ilya Sutskever** • [Architectures](architectures.md) • ![Hall of Fame](https://img.shields.io/badge/⭐-Hall%20of%20Fame-ff1493?style=flat&labelColor=000000)

> Studies **generative pretraining on BooksCorpus followed by task-specific supervised adaptation** in GPT-1.

---

## 📅 2017

### [Deep Contextualized Word Representations](https://arxiv.org/abs/1802.05365)

**Peters et al.** • [Training](training.md) [Architectures](architectures.md) • ![Hall of Fame](https://img.shields.io/badge/⭐-Hall%20of%20Fame-ff1493?style=flat&labelColor=000000)

> **ELMo** combines internal layers of a bidirectional language model into context-dependent word representations for downstream systems.

### [Deep reinforcement learning from human preferences](https://arxiv.org/abs/1706.03741)

**Paul Christiano et al.** • [Training](training.md) • ![Hall of Fame](https://img.shields.io/badge/⭐-Hall%20of%20Fame-ff1493?style=flat&labelColor=000000)

> Learns **reward models from human comparisons of trajectory segments** and uses them to train deep-RL agents.

### [Attention Is All You Need](https://arxiv.org/abs/1706.03762)

**Ashish Vaswani et al.** • [Architectures](architectures.md) • ![Hall of Fame](https://img.shields.io/badge/⭐-Hall%20of%20Fame-ff1493?style=flat&labelColor=000000)

> Introduced the attention-based **Transformer** for sequence transduction, removing recurrent and convolutional sequence layers.

### [Outrageously Large Neural Networks: The Sparsely-Gated Mixture-of-Experts Layer](https://arxiv.org/abs/1701.06538)

**Shazeer et al.** • [Architectures](architectures.md) [Training](training.md) • ![Hall of Fame](https://img.shields.io/badge/⭐-Hall%20of%20Fame-ff1493?style=flat&labelColor=000000)

> Introduces a **sparsely gated expert layer** that activates a small subset of networks per input.

---

## 📅 2014

### [Neural Machine Translation by Jointly Learning to Align and Translate](https://arxiv.org/abs/1409.0473)

**Bahdanau, Cho & Bengio** • [Architectures](architectures.md)

> Learns **soft alignment over encoder states** while generating translations, addressing a fixed-vector bottleneck.

---

## 📅 2000

### [A Neural Probabilistic Language Model](https://jmlr.org/papers/v3/bengio03a.html)

**Bengio, Ducharme & Vincent (NIPS 2000); with Jauvin (JMLR 2003)** • [Architectures](architectures.md) [Training](training.md) • ![Hall of Fame](https://img.shields.io/badge/⭐-Hall%20of%20Fame-ff1493?style=flat&labelColor=000000)

> Learns distributed word representations jointly with a **neural next-word predictor**, sharing statistical strength across similar word sequences.

---

[← Browse the collection](../README.md) · [Suggest a paper or correction](../CONTRIBUTING.md)
