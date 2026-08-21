---
permalink: /
title: ""
excerpt: ""
author_profile: true
redirect_from: 
  - /about/
  - /about.html
---

<span class='anchor' id='about-me'></span>
{% if site.google_scholar_stats_use_cdn %}
{% assign gsDataBaseUrl = "https://cdn.jsdelivr.net/gh/" | append: site.repository | append: "@" %}
{% else %}
{% assign gsDataBaseUrl = "https://raw.githubusercontent.com/" | append: site.repository | append: "/" %}
{% endif %}
{% assign scholarBadgeUrl = gsDataBaseUrl | append: "google-scholar-stats/gs_data_shieldsio.json" %}

<div id="lang-switcher" style="margin: 8px 0 16px 0;">
  <button onclick="setAboutLang('en')" id="btn-en" style="padding: 4px 10px; cursor: pointer;">English</button>
  <button onclick="setAboutLang('zh')" id="btn-zh" style="padding: 4px 10px; margin-right: 8px; cursor: pointer;">中文</button>
</div>


<div id="about-en" markdown="1">

My name is **Zehao Wang**. I am a Ph.D. student in Software Engineering at Tianjin University. My research focuses on **LLM-based Multi-Agent Systems (MAS), Agent Reinforcement Learning, and Risk Reasoning**.

My current research explores how to build **reliable, self-improving multi-agent systems** through better workflow design, epistemic calibration, causal reasoning, and reinforcement learning. In particular, I am interested in how agents coordinate, reason about failures, and learn better strategies from interaction and experience.

# 🎓 Education

- *2024.09 - 2028.06*, Tianjin University, Ph.D. in Software Engineering
- *2021.09 - 2024.06*, Hangzhou Dianzi University, M.S. in Computer Technology
- *2016.09 - 2020.06*, Xidian University, B.Eng. in Communication Engineering


# 🔬 Research Interests

### Multi-Agent Systems

- LLM-based multi-agent workflows and collaboration
- Planner–Executor–Verifier and hierarchical agent architectures
- Workflow reliability and epistemic calibration
- Failure attribution and causal reasoning in agent collaboration
- Risk reasoning and active defense in multi-agent systems

### Agent Reinforcement Learning

- Reinforcement learning for LLM-based agents
- Exploration and exploitation in long-horizon agent trajectories
- Outcome- and process-level reward modeling
- Entropy-aware exploration and policy optimization
- Self-improving and self-evolving agent systems

### Reliable AI & Risk Control

- Risk reasoning and defense for LLM-based systems
- LLM safety and adversarial robustness
- Graph and temporal anomaly detection
- User behavior modeling and illicit-account detection


# 📝 Selected Publications

- **Zehao Wang**, Shilong Jin, Zhao Cao, Lanjun Wang. *When Planning Fails Despite Correct Execution: On Epistemic Calibration for LLM-Based Multi-Agent Systems*. **ICML 2026** (CCF-A)

- **Zehao Wang**, Lanjun Wang, Shilong Jin, Junjie Chen, Yanghua Xiao. *DCFA: Dual-view Causal Attribution for Failure Reasoning in LLM-based Multi-agent Systems*. **EMNLP 2026** (CCF-B)

- **Zehao Wang**, Lanjun Wang, Fuxia Guo, Yanjie Dong. *Pattern-aware Illicit Account Detection based on User Behavior Sequences*. **WWW 2026** (CCF-A)

- **Zehao Wang**, Lanjun Wang. *NK-GAD: Neighbor Knowledge-Enhanced Unsupervised Graph Anomaly Detection*. **DASFAA 2026** (CCF-B)

- **Zehao Wang**, Lanjun Wang. *Reasoning-targeted Jailbreak Attacks on Large Reasoning Models via Semantic Triggers and Psychological Framing*. **Machine Intelligence Research 2026** (JCR Q1)

- Jin Fan, **Zehao Wang** $^{\star}$, Feiwei Qin, Huifeng Wu, Danfeng Sun, Jia Wu. *A distribution feature extracting network with dual correlation for long sequence time-series forecasting*. **Neurocomputing 2025** (CCF-C, JCR Q1)

- Lanjun Wang, **Zehao Wang**, Le Wu, An-An Liu. *Bots Shield Fake News: Adversarial Attack on User Engagement-based Fake News Detection*. **CIKM 2024** (CCF-B)

- **Zehao Wang**, Jin Fan, Huifeng Wu, Danfeng Sun, Jia Wu. *Representing Multi-view Time-series Graph Structures for Multivariate Long-term Time-series Forecasting*. **IEEE TAI 2024** (JCR Q1)

- Jin Fan, **Zehao Wang**, Huifeng Wu, Danfeng Sun, Jia Wu, Xin Lu. *An Adversarial Time-Frequency Reconstruction Network for Unsupervised Anomaly Detection*. **Neural Networks 2023** (CCF-B, JCR Q1)

- **Zehao Wang**, Huifeng Wu, Jin Fan, Danfeng Sun, Jia Wu. *A robust feature reinforcement framework for heterogeneous graphs neural networks*. **FGCS 2023** (JCR Q1)

- Jin Fan, **Zehao Wang**, Danfeng Sun, Huifeng Wu. *Sepformer-based Models: More Efficient Models for Long Sequence Time-Series Forecasting*. **IEEE TETC 2022** (JCR Q1)

</div>


<div id="about-zh" markdown="1" style="display:none;">

我叫 **王则昊**，是天津大学软件工程专业博士研究生。我的研究主要聚焦于 **LLM-based Multi-Agent Systems（多智能体系统）、Agent Reinforcement Learning（智能体强化学习）与风险推理**。

目前，我主要研究如何通过**多智能体 Workflow、认知校准、因果推理与强化学习**，构建更加可靠、能够持续自我改进的智能体系统。重点关注智能体之间如何协作、如何理解和归因失败、如何从交互经验中学习更好的决策策略。


# 🎓 教育经历

- *2024.09 - 2028.06*，天津大学，博士（软件工程）
- *2021.09 - 2024.06*，杭州电子科技大学，硕士（计算机技术）
- *2016.09 - 2020.06*，西安电子科技大学，本科（通信工程）


# 🔬 研究方向

### 多智能体系统

- 基于大语言模型的多智能体 Workflow 与协作机制
- Planner–Executor–Verifier 等多智能体架构
- Workflow 可靠性与认知校准
- 多智能体协作中的失败归因与因果推理
- 多智能体系统中的风险推理与主动防御

### Agent Reinforcement Learning

- 面向 LLM Agent 的强化学习
- 长程 Agent Trajectory 中的探索与利用
- Outcome-level 与 Process-level Reward Modeling
- 基于 Entropy 的探索与策略优化
- Agent 的自我改进与自进化

### Reliable AI & 风险控制

- LLM 系统中的风险推理与安全防御
- 大模型安全与对抗鲁棒性
- 图异常检测与时序异常检测
- 用户行为建模与黑产账户检测


# 📝 代表论文

- **Zehao Wang**, Shilong Jin, Zhao Cao, Lanjun Wang. *When Planning Fails Despite Correct Execution: On Epistemic Calibration for LLM-Based Multi-Agent Systems*. **ICML 2026** (CCF-A)

- **Zehao Wang**, Lanjun Wang, Fuxia Guo, Yanjie Dong. *Pattern-aware Illicit Account Detection based on User Behavior Sequences*. **WWW 2026** (CCF-A)

- **Zehao Wang**, Lanjun Wang, Shilong Jin, Junjie Chen, Yanghua Xiao. *DCFA: Dual-view Causal Attribution for Failure Reasoning in LLM-based Multi-agent Systems*. **EMNLP 2026** (CCF-B)

- **Zehao Wang**, Lanjun Wang. *NK-GAD: Neighbor Knowledge-Enhanced Unsupervised Graph Anomaly Detection*. **DASFAA 2026** (CCF-B)

- **Zehao Wang**, Lanjun Wang. *Reasoning-targeted Jailbreak Attacks on Large Reasoning Models via Semantic Triggers and Psychological Framing*. **Machine Intelligence Research 2026** (JCR Q1)

- Jin Fan, **Zehao Wang** $^{\star}$, Feiwei Qin, Huifeng Wu, Danfeng Sun, Jia Wu. *A distribution feature extracting network with dual correlation for long sequence time-series forecasting*. **Neurocomputing 2025** (CCF-C, JCR Q1)

- Lanjun Wang, **Zehao Wang**, Le Wu, An-An Liu. *Bots Shield Fake News: Adversarial Attack on User Engagement-based Fake News Detection*. **CIKM 2024** (CCF-B)

- **Zehao Wang**, Jin Fan, Huifeng Wu, Danfeng Sun, Jia Wu. *Representing Multi-view Time-series Graph Structures for Multivariate Long-term Time-series Forecasting*. **IEEE TAI 2024** (JCR Q1)

- Jin Fan, **Zehao Wang**, Huifeng Wu, Danfeng Sun, Jia Wu, Xin Lu. *An Adversarial Time-Frequency Reconstruction Network for Unsupervised Anomaly Detection*. **Neural Networks 2023** (CCF-B, JCR Q1)

- **Zehao Wang**, Huifeng Wu, Jin Fan, Danfeng Sun, Jia Wu. *A robust feature reinforcement framework for heterogeneous graphs neural networks*. **FGCS 2023** (JCR Q1)

- Jin Fan, **Zehao Wang**, Danfeng Sun, Huifeng Wu. *Sepformer-based Models: More Efficient Models for Long Sequence Time-Series Forecasting*. **IEEE TETC 2022** (JCR Q1)

</div>


<script>
function setAboutLang(lang) {
  var en = document.getElementById('about-en');
  var zh = document.getElementById('about-zh');
  var btnZh = document.getElementById('btn-zh');
  var btnEn = document.getElementById('btn-en');
  var showEn = lang !== 'zh';

  zh.style.display = showEn ? 'none' : 'block';
  en.style.display = showEn ? 'block' : 'none';
  btnZh.style.fontWeight = showEn ? '400' : '700';
  btnEn.style.fontWeight = showEn ? '700' : '400';
}

setAboutLang('en');
</script>
