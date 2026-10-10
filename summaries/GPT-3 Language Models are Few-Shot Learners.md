# GPT-3: Language Models are Few-Shot Learners - Detailed Summary

📄 **Paper:** [Language Models are Few-Shot Learners](https://arxiv.org/abs/2005.14165)<br>
👥 **Authors:** Tom B. Brown, Benjamin Mann, Nick Ryder, Melanie Subbiah, et al. · OpenAI<br>
📅 **First public version:** May 2020 · NeurIPS 2020

---

## 🎯 One-Line Summary

GPT-3 evaluates whether large autoregressive models can perform tasks from prompt examples without task-specific gradient updates.

## 💡 Key Innovation: Scale + In-Context Learning

| Setting | Prompt supplies | Evaluation weight update |
| :-- | :-- | :-- |
| **Zero-shot** | Task description, no demonstrations | None |
| **One-shot** | One demonstration | None |
| **Few-shot** | Several demonstrations within context capacity | None |

### The GPT-3 Model Family

[Version 4, Table 2.1](https://arxiv.org/pdf/2005.14165v4):

| Model | Parameters | Layers | Hidden size |
| :-- | --: | --: | --: |
| Small | 125M | 12 | 768 |
| Medium | 350M | 24 | 1024 |
| Large | 760M | 24 | 1536 |
| XL | 1.3B | 24 | 2048 |
| 2.7B | 2.7B | 32 | 2560 |
| 6.7B | 6.7B | 32 | 4096 |
| 13B | 13B | 40 | 5140 |
| GPT-3 | 175B | 96 | 12288 |

## 📊 Results & Impact

The authors evaluate language modeling, question answering, translation, arithmetic and other tasks. Few-shot performance improves with scale on many tested tasks while others remain weak. The study helped establish prompting a general model as an alternative to separate task training.

**When reading a score:** check zero-/one-/few-shot setup, example count, evaluation split and contamination analysis. Web-trained models can encounter benchmark material during pretraining.

## 💻 Implementation

Prompt-format illustration:

```text
Translate English to French:
sea otter => loutre de mer
peppermint => menthe poivrée
cheese =>
```

The model continues the text; examples do not update its weights. A plausible completion is not guaranteed correct.

## 📏 Relationship to Scaling Laws

[Kaplan et al.](https://arxiv.org/abs/2001.08361) separately studied empirical loss scaling. GPT-3 does not establish unlimited improvement, universal sudden emergence, or that prompting always beats fine-tuning.

## ⚠️ Limitations & Concerns

- Training and inference are expensive; no dollar cost is inferred from unreported prices.
- Contamination, bias and unreliable factual outputs complicate evaluation.
- Strong benchmark scores do not establish general intelligence or reliable multi-step reasoning.
- Prompt adaptation differs from training an instruction-following assistant.

## 🔮 What Came After

[Codex](https://arxiv.org/abs/2107.03374) studies code models and execution-based evaluation. [InstructGPT](RLHF%20Training%20with%20Human%20Feedback.md) addresses instruction following with demonstrations and preferences.

## 🎓 Key Takeaways

Separate pretraining scale, prompt examples and post-training: their effects need different baselines.

## 📚 Essential Resources

- [Original paper and revisions](https://arxiv.org/abs/2005.14165)
- [Configurations and evaluations — version 4](https://arxiv.org/pdf/2005.14165v4)
- [Language model families](../categories/architectures.md#-language-model-families)

---

Part of [Awesome LLM Papers](../README.md). Summary reviewed 10 October 2026 against the linked source version.
