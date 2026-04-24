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
  <button onclick="setAboutLang('zh')" id="btn-zh" style="padding: 4px 10px; margin-right: 8px; cursor: pointer;">中文</button>
  <button onclick="setAboutLang('en')" id="btn-en" style="padding: 4px 10px; cursor: pointer;">English</button>
</div>

<div id="about-zh" markdown="1">
我叫 **王则昊**，研究方向聚焦在**风控 AI、多智能体系统与异常检测**。当前主要围绕多智能体协作中的风险推理与防护、图与时序异常检测、以及大模型安全展开研究与实践。

联系方式：`wzhrslh@gmail.com`

Google Scholar: [LvP_YfYAAAAJ](https://scholar.google.com/citations?user=LvP_YfYAAAAJ&hl=en)
<a href='https://scholar.google.com/citations?user=LvP_YfYAAAAJ&hl=en'><img src="https://img.shields.io/endpoint?url={{ scholarBadgeUrl | url_encode }}&logo=Google%20Scholar&labelColor=f6f6f6&color=9cf&style=flat&label=citations"></a>

# 🎓 教育经历
- *2024.09 - 2028.06*，天津大学，博士（软件工程）
- *2021.09 - 2024.06*，杭州电子科技大学，硕士（计算机技术）
- *2016.09 - 2020.06*，西安电子科技大学，本科（通信工程）

# 🔬 研究方向与技能
- 多智能体系统：协作机制、失败归因、风险推理与主动防护
- 风控与异常检测：图异常检测（GNN）、时序异常检测、黑产用户行为建模
- 大模型与安全：对抗攻防、越狱攻击分析、风险评测

# 📝 代表论文
- Zehao Wang, et al. *Pattern-aware Illicit Account Detection based on User Behavior Sequences*. WWW 2026 (CCF-A)
- Zehao Wang, et al. *NK-GAD: Neighbor Knowledge-Enhanced Unsupervised Graph Anomaly Detection*. DASFAA 2026 (CCF-B)
- Lanjun Wang, Zehao Wang, et al. *Bots Shield Fake News: Adversarial Attack on User Engagement-based Fake News Detection*. CIKM 2024 (CCF-B)
- Zehao Wang, et al. *Reasoning-targeted Jailbreak Attacks on Large Reasoning Models via Semantic Triggers and Psychological Framing*. Machine Intelligence Research 2026 (SCI Q1)
- Zehao Wang, et al. *Representing Multi-view Time-series Graph Structures for Multivariate Long-term Time-series Forecasting*. IEEE TAI 2024 (JCR Q1)
- Zehao Wang, et al. *A robust feature reinforcement framework for heterogeneous graphs neural networks*. FGCS 2023 (SCI Q1)
- Jin Fan, Zehao Wang, et al. *An Adversarial Time-Frequency Reconstruction Network for Unsupervised Anomaly Detection*. Neural Networks 2023 (CCF-B, SCI Q1)
- Jin Fan, Zehao Wang, et al. *Sepformer-based Models: More Efficient Models for Long Sequence Time-Series Forecasting*. IEEE TETC 2022 (SCI Q1)
</div>

<div id="about-en" markdown="1" style="display:none;">
My name is **Zehao Wang**. My research focuses on **Risk Control AI, Multi-agent Systems, and Anomaly Detection**. I currently work on risk reasoning and defense in multi-agent collaboration, graph/time-series anomaly detection, and LLM safety.

Contact: `wzhrslh@gmail.com`

Google Scholar: [LvP_YfYAAAAJ](https://scholar.google.com/citations?user=LvP_YfYAAAAJ&hl=en)
<a href='https://scholar.google.com/citations?user=LvP_YfYAAAAJ&hl=en'><img src="https://img.shields.io/endpoint?url={{ scholarBadgeUrl | url_encode }}&logo=Google%20Scholar&labelColor=f6f6f6&color=9cf&style=flat&label=citations"></a>

# 🎓 Education
- *2024.09 - 2028.06*, Tianjin University, Ph.D. in Software Engineering
- *2021.09 - 2024.06*, Hangzhou Dianzi University, M.S. in Computer Technology
- *2016.09 - 2020.06*, Xidian University, B.Eng. in Communication Engineering

# 🔬 Research Interests & Skills
- Multi-agent systems: collaboration mechanisms, failure attribution, risk reasoning, and active defense
- Risk control and anomaly detection: graph anomaly detection (GNN), time-series anomaly detection, illicit-user behavior modeling
- LLM and AI safety: adversarial attack/defense, jailbreak analysis, and risk evaluation

# 📝 Selected Publications
- Zehao Wang, et al. *Pattern-aware Illicit Account Detection based on User Behavior Sequences*. WWW 2026 (CCF-A)
- Zehao Wang, et al. *NK-GAD: Neighbor Knowledge-Enhanced Unsupervised Graph Anomaly Detection*. DASFAA 2026 (CCF-B)
- Lanjun Wang, Zehao Wang, et al. *Bots Shield Fake News: Adversarial Attack on User Engagement-based Fake News Detection*. CIKM 2024 (CCF-B)
- Zehao Wang, et al. *Reasoning-targeted Jailbreak Attacks on Large Reasoning Models via Semantic Triggers and Psychological Framing*. Machine Intelligence Research 2026 (SCI Q1)
- Zehao Wang, et al. *Representing Multi-view Time-series Graph Structures for Multivariate Long-term Time-series Forecasting*. IEEE TAI 2024 (JCR Q1)
- Zehao Wang, et al. *A robust feature reinforcement framework for heterogeneous graphs neural networks*. FGCS 2023 (SCI Q1)
- Jin Fan, Zehao Wang, et al. *An Adversarial Time-Frequency Reconstruction Network for Unsupervised Anomaly Detection*. Neural Networks 2023 (CCF-B, SCI Q1)
- Jin Fan, Zehao Wang, et al. *Sepformer-based Models: More Efficient Models for Long Sequence Time-Series Forecasting*. IEEE TETC 2022 (SCI Q1)
</div>

<script>
function setAboutLang(lang) {
  var zh = document.getElementById('about-zh');
  var en = document.getElementById('about-en');
  var btnZh = document.getElementById('btn-zh');
  var btnEn = document.getElementById('btn-en');
  var showZh = lang !== 'en';

  zh.style.display = showZh ? 'block' : 'none';
  en.style.display = showZh ? 'none' : 'block';
  btnZh.style.fontWeight = showZh ? '700' : '400';
  btnEn.style.fontWeight = showZh ? '400' : '700';
}

setAboutLang('zh');
</script>
