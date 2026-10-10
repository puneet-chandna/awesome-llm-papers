# 🔬 Analysis & Theory: Understanding How LLMs Work

<div align="center">

[![Awesome](https://awesome.re/badge-flat2.svg)](https://awesome.re)
[![Works](https://img.shields.io/badge/Works-22-blue.svg)](all-papers.md)
[![Years](https://img.shields.io/badge/Years-2020--2025-green.svg)](all-papers.md)
[![License: CC0](https://img.shields.io/badge/License-CC0-yellow.svg)](../LICENSE)
[![PRs Welcome](https://img.shields.io/badge/PRs-welcome-brightgreen.svg?style=flat-square)](../CONTRIBUTING.md)

### A curated collection of papers on interpretability, mechanistic analysis, and evaluation of Large Language Models

_Understanding the inner workings of LLMs—from circuit-level analysis to emergent behaviors and rigorous evaluation methodologies._

</div>

---

## 📑 Table of Contents

- [🔍 Interpretability](#-interpretability)
- [🪄 Emergent Abilities](#-emergent-abilities)
- [📏 Scaling Laws](#-scaling-laws)
- [📊 Evaluation](#-evaluation)
- [📖 Foundations & Perspectives](#-foundations--perspectives)

---

## 🔍 Interpretability

### 📄 [A Mathematical Framework for Transformer Circuits](https://transformer-circuits.pub/2021/framework/index.html)

**Authors:** Nelson Elhage et al. (Anthropic)<br>
**Contribution:** `🔬 Mechanistic Interpretability`

> An **author research article** developing a circuit view of attention-only Transformers, including residual streams and information movement through heads. Its toy-model analysis provides reusable tools while leaving full-model and MLP explanations open.

---

### 📄 [In-context Learning and Induction Heads](https://transformer-circuits.pub/2022/in-context-learning-and-induction-heads/index.html)

**Authors:** Catherine Olsson et al. (Anthropic)<br>
**Contribution:** `🧩 Circuit Discovery`

> Studies **induction-head circuits** that match and continue repeated patterns, with evidence linking their formation to aspects of in-context learning. The strongest causal results concern small attention-only models; they do not explain every form of in-context learning.

---

### 📄 [Scaling Monosemanticity: Extracting Interpretable Features from Claude 3 Sonnet](https://transformer-circuits.pub/2024/scaling-monosemanticity/)

**Authors:** Adly Templeton et al. (Anthropic)<br>
**Contribution:** `🔎 Feature Extraction`

> Uses **sparse autoencoders to extract learned features** from Claude 3 Sonnet activations. Interpretable features are directions in a learned decomposition, not necessarily single neurons, and identifying them does not fully explain the model’s computation.

---

### 📄 [Scaling and evaluating sparse autoencoders](https://arxiv.org/abs/2406.04093) ![Hall of Fame](https://img.shields.io/badge/⭐-Hall%20of%20Fame-ff1493?style=flat&labelColor=000000)

**Authors:** Leo Gao et al. (OpenAI)<br>
**Contribution:** `🔬 Interpretability at Scale`

> Scales **k-sparse autoencoders** and develops evaluation tools for interpreting learned activation features. The study includes a 16M-latent GPT-4 autoencoder trained on 40B tokens, building on earlier k-sparse methods; learned features still have incomplete interpretability and context limitations.

---

### 📄 [Representation Engineering: A Top-Down Approach to AI Transparency](https://arxiv.org/abs/2310.01405)

**Authors:** Andy Zou et al.<br>
**Contribution:** `🎛️ Representation Control`

> Uses **representation reading and control** to identify and steer high-level concepts in model activations. RepE offers a complementary approach to circuit analysis; demonstrated steering does not establish complete interpretability or safe control in every context.

---

## 🪄 Emergent Abilities

### 📄 [Emergent Abilities of Large Language Models](https://arxiv.org/abs/2206.07682) ![Hall of Fame](https://img.shields.io/badge/⭐-Hall%20of%20Fame-ff1493?style=flat&labelColor=000000)

**Authors:** Jason Wei et al.<br>
**Contribution:** `🪄 Emergence Theory`

> Catalogues **emergent abilities as measured on selected tasks**, where scores appear abruptly with scale. It provides a useful historical framework; metric-dependent interpretations should be read alongside the later Mirage analysis.

---

### 📄 [Are Emergent Abilities of Large Language Models a Mirage?](https://arxiv.org/abs/2304.15004)

**Authors:** Rylan Schaeffer, Brando Miranda and Sanmi Koyejo<br>
**Contribution:** `🔬 Critical Analysis`

> Shows how **metric choice can create apparent emergence** in studied tasks and model families. Continuous measures can reveal smoother progress hidden by thresholded scores; these cases do not explain every possible emergent behavior.

---

### 📄 [Language Models Don't Always Say What They Think: Unfaithful Explanations in Chain-of-Thought Prompting](https://arxiv.org/abs/2305.04388)

**Authors:** Miles Turpin et al.<br>
**Contribution:** `⚠️ Faithfulness Analysis`

> Introduces biasing features that alter answers without being acknowledged in **generated chain-of-thought explanations**. These controlled counterexamples show why readable rationales need faithfulness evaluation; they do not establish that every rationale is unfaithful.

---

## 📏 Scaling Laws

### 📄 [Scaling Laws for Neural Language Models](https://arxiv.org/abs/2001.08361) ![Hall of Fame](https://img.shields.io/badge/⭐-Hall%20of%20Fame-ff1493?style=flat&labelColor=000000)

**Authors:** Jared Kaplan et al. (OpenAI)<br>
**Contribution:** `📊 Foundational Scaling`

> Fits empirical **language-model loss scaling** with parameters, data and compute over measured regimes. A quantitative framework for training allocation; loss fits should be distinguished from laws of general capability or unlimited extrapolation.

---

### 📄 [Scaling Laws for Code: Every Programming Language Matters](https://arxiv.org/abs/2512.13472)

**Authors:** Jian Yang et al.<br>
**Contribution:** `💻 Language-Specific Scaling`

> Studies **language-specific code scaling** and multilingual data proportions across seven programming languages. The fitted loss relations guide allocation within the tested models, corpora and tokenizers; irreducible loss should not be treated as an intrinsic measure of programming-language complexity.

---

### 📄 [Scaling Language Models: Methods, Analysis & Insights from Training Gopher](https://arxiv.org/abs/2112.11446) ![Hall of Fame](https://img.shields.io/badge/⭐-Hall%20of%20Fame-ff1493?style=flat&labelColor=000000)

**Authors:** Jack W. Rae et al.<br>
**Contribution:** `📊 Scaling Analysis`

> An **official Gopher report** studying a 280B model across a broad task suite. Scale helps reading comprehension and fact-checking more than selected logic/math tasks; data, bias and task-dependent failures remain central to its analysis.

---

### 📄 [Training Compute-Optimal Large Language Models](https://arxiv.org/abs/2203.15556) ![Hall of Fame](https://img.shields.io/badge/⭐-Hall%20of%20Fame-ff1493?style=flat&labelColor=000000)

**Authors:** Jordan Hoffmann et al.<br>
**Contribution:** `⚖️ Compute Allocation`

> Studies **compute-optimal allocation between parameter count and training tokens** under a fixed pretraining budget. Chinchilla shows why many contemporary large models were undertrained; deployment cost and inference frequency can change the preferred allocation.

---

## 📊 Evaluation

### 📄 [Measuring Massive Multitask Language Understanding](https://arxiv.org/abs/2009.03300)

**Authors:** Dan Hendrycks et al.<br>
**Contribution:** `📏 Benchmark`

> Introduces **MMLU**, multiple-choice evaluation across 57 academic and professional subjects. It exposes broad but uneven performance and calibration gaps; an aggregate score is not a complete measure of understanding.

---

### 📄 [Beyond the Imitation Game: Quantifying and extrapolating the capabilities of language models](https://arxiv.org/abs/2206.04615)

**Authors:** Aarohi Srivastava et al. (BIG-bench collaboration)<br>
**Contribution:** `🎯 Comprehensive Evaluation`

> Introduces **BIG-bench**, a collaborative collection of over 200 tasks probing diverse language-model capabilities. It highlights uneven scaling and challenging evaluations; task design and metric brittleness shape apparent transitions.

---

### 📄 [Holistic Evaluation of Language Models](https://arxiv.org/abs/2211.09110)

**Authors:** Percy Liang et al.<br>
**Contribution:** `🔄 Holistic Assessment`

> Proposed **HELM**, a framework for evaluating LLMs across multiple dimensions simultaneously—accuracy, calibration, robustness, fairness, efficiency, and more. Rather than optimizing for a single metric, HELM provides a comprehensive view of model capabilities and limitations, enabling more informed comparisons and highlighting trade-offs between different aspects of performance.

---

### 📄 [Judging LLM-as-a-Judge with MT-Bench and Chatbot Arena](https://arxiv.org/abs/2306.05685)

**Authors:** Lianmin Zheng et al.<br>
**Contribution:** `⚖️ LLM Evaluation`

> Studies **LLM judging, MT-Bench and crowdsourced pairwise Chatbot Arena comparisons**. Strong judges agree with human preferences in the tested settings, while position, verbosity, self-enhancement and reasoning biases limit their reliability.

---

### 📄 [The Illusion of Thinking: Understanding the Strengths and Limitations of Reasoning Models via the Lens of Problem Complexity](https://arxiv.org/abs/2506.06941)

**Authors:** Parshin Shojaee et al.<br>
**Contribution:** `🔬 Reasoning Analysis`

> Studies reasoning models on controlled puzzles of increasing complexity, observing task-dependent gains and eventual failures. Read the **revised protocols and output constraints** before interpreting collapse: these experiments do not prove reasoning is impossible or that explanations are universally illusory.

---

### 📄 [Training Verifiers to Solve Math Word Problems](https://arxiv.org/abs/2110.14168) ![Hall of Fame](https://img.shields.io/badge/⭐-Hall%20of%20Fame-ff1493?style=flat&labelColor=000000)

**Authors:** Cobbe et al.<br>
**Contribution:** `✅ GSM8K & Verifiers`

> See the main entry in [Reasoning](reasoning.md) for the method, evidence and limitations.

---

### 📄 [Scaling Laws for Reward Model Overoptimization](https://arxiv.org/abs/2210.10760)

**Authors:** Gao, Schulman & Hilton<br>
**Contribution:** `⚠️ Proxy Optimization`

> Measures how stronger optimization of an imperfect **proxy reward** can eventually reduce a synthetic gold-model reward under best-of-N and PPO. A useful failure model for alignment; the gold reward is not actual human values and the fitted relations are setup-dependent.

---

### 📄 [Pythia: A Suite for Analyzing Large Language Models Across Training and Scaling](https://arxiv.org/abs/2304.01373)

**Authors:** Biderman et al.<br>
**Contribution:** `🔬 Controlled Model Suite`

> Releases **model suites, training checkpoints and data-order tooling** for studying learning dynamics and scale. Compare models within the original or deduplicated Pile cohort; the two cohorts do not share an identical data sequence, and frontier-scale extrapolation needs fresh evidence.

---

### 📄 [Lost in the Middle: How Language Models Use Long Contexts](https://arxiv.org/abs/2307.03172)

**Authors:** Liu et al.<br>
**Contribution:** `📍 Context Utilization`

> See the main entry in [Rag](rag.md) for the method, evidence and limitations.

---

## 📖 Foundations & Perspectives

### 📄 [On the Opportunities and Risks of Foundation Models](https://arxiv.org/abs/2108.07258) ![Hall of Fame](https://img.shields.io/badge/⭐-Hall%20of%20Fame-ff1493?style=flat&labelColor=000000)

**Authors:** Rishi Bommasani et al.<br>
**Contribution:** `📖 Research Perspective`

> A **research report and perspective** defining foundation models and examining adaptation, homogenization and societal risks. It supplies a shared framework for inherited downstream capabilities and failures rather than a new training experiment.

---

<div align="center">

### 🌟 Contributing

Feel free to submit PRs to add more analysis and theory papers or improve existing entries!

### 📜 License

This repository is licensed under CC0 License.

### 🙏 Acknowledgments

This list honors the researchers working to understand and evaluate the systems that are reshaping our world.

---

⭐ If you find this repository helpful, please consider giving it a star!

</div>
