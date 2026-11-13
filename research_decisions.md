# Literature-to-Experiment Decisions

## Verified Gap
Prior literature (Errica et al., 2025; Sclar et al., 2024) proves single-turn LLMs are highly sensitive to surface formatting and semantic phrasing. However, there is a gap in evaluating how these single-turn vulnerabilities compound in multi-stage agentic pipelines where conclusions are extracted rather than simple labels.

## Design Decisions
1.  **Dataset:** `qiaojin/PubMedQA` was chosen for its strict biomedical reasoning requirements and explicit yes/no/maybe conclusions.
2.  **Models:** `Qwen2.5-0.5B-Instruct` and `Qwen2.5-1.5B-Instruct` were selected to provide a comparative analysis of scale versus stability.
3.  **Metrics:** Conclusion Agreement Rate (CAR) and Normalized Entropy ($S_\tau$) were chosen over standard accuracy to decouple lexical variance from structural claim drift.
