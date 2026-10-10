# Chain-of-Thought Prompting - Detailed Summary

📄 **Paper:** [Chain-of-Thought Prompting Elicits Reasoning in Large Language Models](https://arxiv.org/abs/2201.11903)<br>
👥 **Authors:** Jason Wei, Xuezhi Wang, Dale Schuurmans, Maarten Bosma, Brian Ichter, Fei Xia, Ed H. Chi, Quoc V. Le, Denny Zhou · Google Research<br>
📅 **First public version:** January 2022 · NeurIPS 2022

---

## 🎯 One-Line Summary

Adding worked reasoning steps to few-shot demonstrations improves several reasoning benchmarks without updating model weights.

## 💡 Key Innovation: Chain-of-Thought (CoT)

The original method shows examples containing **question → intermediate steps → answer**, then asks the model to continue a new question in that style.

| Standard demonstration | Chain-of-thought demonstration |
| :-- | :-- |
| Sam has 3 apples and gives away 1. **Answer: 2.** | Sam starts with 3 and gives away 1. **3 − 1 = 2. Answer: 2.** |

This is **few-shot CoT**. The separate [Kojima et al. zero-shot paper](https://arxiv.org/abs/2205.11916) studies a reasoning instruction followed by answer extraction without worked exemplars.

## 📊 Results & Impact

**PaLM 540B accuracy (%), standard versus CoT**, [version 6, Appendix Table 2](https://arxiv.org/pdf/2201.11903v6), page 21:

| Benchmark | Standard | CoT |
| :-- | --: | --: |
| GSM8K | 17.9 | 56.9 |
| SVAMP | 69.4 | 79.0 |
| AQuA | 25.2 | 35.8 |

These rows exclude the external calculator. Results are specific to the model, task and prompt, not universal gains or a hard parameter threshold.

## 💻 Implementation

Prompt-format illustration, not a model implementation:

```text
Q: A train travels 60 miles per hour for 2 hours. How far does it go?
A: Distance = speed × time. 60 × 2 = 120 miles. The answer is 120 miles.

Q: {new_question}
A:
```

Compare representative exemplars with a direct-answer baseline.

## ⚠️ Limitations & Challenges

- Extra reasoning tokens cost inference time; avoiding fine-tuning does not make inference free.
- Gains vary with model, task and demonstrations; plausible steps can be wrong.
- Visible explanations do not certify correctness or faithfully expose internal computation. See [the faithfulness study](https://arxiv.org/abs/2305.04388).

## 🔮 Variants & Extensions

| Next reading | What changes |
| :-- | :-- |
| [Zero-shot CoT](https://arxiv.org/abs/2205.11916), 2022 | Elicit reasoning without worked demonstrations. |
| [Self-consistency](https://arxiv.org/abs/2203.11171), 2022 preprint | Sample paths and aggregate final answers. |
| [Tree of Thoughts](https://arxiv.org/abs/2305.10601), 2023 | Explore and backtrack over candidate steps. |
| [ReAct](https://arxiv.org/abs/2210.03629), 2022 preprint | Interleave reasoning, actions and observations. |

## 🎓 Key Takeaways

The demonstrations' intermediate steps are the original intervention. Generating, selecting and verifying solutions answer different questions.

## 📚 Essential Resources

- [Original paper and revisions](https://arxiv.org/abs/2201.11903)
- [Full prompts and tables — version 6](https://arxiv.org/pdf/2201.11903v6)
- [Reasoning collection](../categories/reasoning.md)

---

Part of [Awesome LLM Papers](../README.md). Summary reviewed 10 October 2026 against the linked source version.
