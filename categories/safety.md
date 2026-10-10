# 🛡️ Safety & Security: Attacks, Alignment & Robustness

[![Awesome](https://awesome.re/badge-flat2.svg)](https://awesome.re)

Papers that make safety claims testable: attack mechanisms, engineered backdoors and the limits of alignment.

**Start here:** an attack can reveal a weakness; passing an evaluation cannot certify safety in every setting.

---

## 📑 Table of Contents

- [🔓 Attacks & Robustness](#-attacks--robustness)
- [🛡️ Safety Training & Backdoors](#%EF%B8%8F-safety-training--backdoors)
- [⚖️ Safety Evaluation & Alignment](#%EF%B8%8F-safety-evaluation--alignment)

---

## 🔓 Attacks & Robustness

### 📄 [Universal and Transferable Adversarial Attacks on Aligned Language Models](https://arxiv.org/abs/2307.15043)

**Authors:** Andy Zou et al.<br>
**Contribution:** `🔓 Adversarial Suffixes`

> Optimizes **adversarial suffixes** against aligned models and studies their transfer across models and interfaces. The experiments reveal shared attack surfaces in the tested systems; historical transfer rates require reevaluation against newer defenses.

---

### 📄 [Jailbroken: How Does LLM Safety Training Fail?](https://arxiv.org/abs/2307.02483)

**Authors:** Alexander Wei, Nika Haghtalab and Jacob Steinhardt (UC Berkeley)<br>
**Contribution:** `🛡️ Alignment Failure Modes`

> Analyzes **competing objectives and mismatched generalization** as two routes to jailbreak failures. The Berkeley authors connect conceptual failure modes with attacks on tested aligned models; the framework is not an exhaustive taxonomy of all current exploits.

---

### 📄 [Universal Adversarial Triggers for Attacking and Analyzing NLP](https://arxiv.org/abs/1908.07125)

**Authors:** Eric Wallace et al.<br>
**Contribution:** `🔓 Input-Agnostic Triggers`

> Finds **input-agnostic adversarial token triggers** that degrade tested NLP systems and expose learned associations. “Universal” refers to reuse across inputs in the studied tasks, with success and transfer depending on model and distribution.

---

### 📄 [Many-shot Jailbreaking](https://www-cdn.anthropic.com/af5633c94ed2beb282f6a53c595eb437e8e7b630/Many_Shot_Jailbreaking__2024_04_02_0936.pdf)

**Authors:** Cem Anil et al. (Anthropic)<br>
**Contribution:** `🔓 In-Context Attacks`

> An **author research report** studying how many in-context demonstrations can induce harmful responses. It links attack success with context length and model/task settings; no single example-count threshold universally overrides safety training.

---

## 🛡️ Safety Training & Backdoors

### 📄 [Sleeper Agents: Training Deceptive LLMs that Persist Through Safety Training](https://arxiv.org/abs/2401.05566)

**Authors:** Hubinger et al.<br>
**Contribution:** `🛡️ Backdoor Persistence`

> Constructs **trigger-dependent backdoors** and tests their persistence through supervised, reinforcement and adversarial safety training. It challenges assumptions about removing engineered behaviors; the study does not estimate how often such behavior arises naturally.

---

## ⚖️ Safety Evaluation & Alignment

---

### 📄 [Constitutional AI: Harmlessness from AI Feedback](https://arxiv.org/abs/2212.08073) ![Hall of Fame](https://img.shields.io/badge/⭐-Hall%20of%20Fame-ff1493?style=flat&labelColor=000000)

**Authors:** Yuntao Bai et al. (Anthropic)<br>
**Contribution:** `🛡️ Scalable Safety`

> See the main entry in [Training](training.md) for the method, evidence and limitations.

---

### 📄 [OpenAI o1 System Card](https://arxiv.org/abs/2412.16720)

**Authors:** OpenAI (Aaron Jaech et al.)<br>
**Contribution:** `🎯 Reasoning at Scale`

> See the main entry in [Reasoning](reasoning.md) for the method, evidence and limitations.

---

### 🌟 Contributing

Suggest a paper or correction through the [contribution guide](../CONTRIBUTING.md).

### 📜 License

This repository is licensed under CC0.
