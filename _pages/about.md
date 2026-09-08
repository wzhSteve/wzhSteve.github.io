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


<!-- ========================================================= -->
<!-- ======================== STYLE =========================== -->
<!-- ========================================================= -->

<style>

:root {
  --accent: #1769aa;
  --text: #222;
  --muted: #666;
  --light: #888;
  --border: #e8e8e8;
  --soft: #f7f9fb;
}

/* ---------- Language Switcher ---------- */

#lang-switcher {
  margin: 4px 0 34px 0;
  padding-bottom: 10px;
  border-bottom: 1px solid var(--border);
  font-size: 0.86rem;
  letter-spacing: 0.01em;
}

#lang-switcher button {
  border: none;
  background: transparent;
  padding: 0;
  margin-right: 18px;
  cursor: pointer;
  font-family: inherit;
  font-size: inherit;
  transition: all 0.2s ease;
}

#lang-switcher button:hover {
  color: var(--accent) !important;
}

/* ---------- Main Typography ---------- */

#about-en,
#about-zh {
  max-width: 900px;
  color: var(--text);
  line-height: 1.75;
}

#about-en h1,
#about-zh h1 {
  margin-top: 0;
  margin-bottom: 8px;
  font-size: 2.35rem;
  font-weight: 700;
  letter-spacing: -0.025em;
}

#about-en h2,
#about-zh h2 {
  margin-top: 48px;
  margin-bottom: 20px;
  padding-bottom: 9px;
  border-bottom: 1px solid var(--border);
  font-size: 1.38rem;
  font-weight: 650;
  letter-spacing: -0.01em;
}

#about-en h3,
#about-zh h3 {
  margin-top: 28px;
  margin-bottom: 8px;
  font-size: 1.05rem;
  font-weight: 650;
}

#about-en h4,
#about-zh h4 {
  margin-top: 22px;
  margin-bottom: 7px;
  font-size: 0.96rem;
  font-weight: 600;
  color: #444;
}

/* ---------- Links ---------- */

#about-en a,
#about-zh a {
  color: var(--accent);
  text-decoration: none;
}

#about-en a:hover,
#about-zh a:hover {
  text-decoration: underline;
}

/* ---------- Intro ---------- */

.profile-subtitle {
  margin: 0 0 20px 0;
  color: #555;
  font-size: 1.02rem;
}

.profile-description {
  max-width: 820px;
  margin-bottom: 18px;
}

.profile-links {
  margin: 18px 0 8px 0;
  font-size: 0.92rem;
}

.profile-links a {
  margin-right: 15px;
  white-space: nowrap;
}

/* ---------- Research Cards ---------- */

.research-grid {
  display: grid;
  grid-template-columns: repeat(3, 1fr);
  gap: 14px;
  margin: 8px 0 12px 0;
}

.research-card {
  padding: 17px 18px 15px 18px;
  background: var(--soft);
  border: 1px solid #edf0f2;
  border-radius: 6px;
}

.research-card h3 {
  margin: 0 0 8px 0 !important;
  font-size: 1rem !important;
  color: #222;
}

.research-card p {
  margin: 0;
  font-size: 0.88rem;
  line-height: 1.65;
  color: #555;
}

.research-card ul {
  margin: 9px 0 0 17px;
  padding: 0;
}

.research-card li {
  margin-bottom: 3px;
  font-size: 0.84rem;
}

/* ---------- Publications ---------- */

.pub-section {
  margin-top: 6px;
}

.pub-item {
  position: relative;
  margin: 0 0 20px 0;
  padding: 0 0 18px 15px;
  border-left: 2px solid #e5e9ed;
}

.pub-item:hover {
  border-left-color: var(--accent);
}

.pub-venue {
  display: inline-block;
  margin-bottom: 5px;
  padding: 2px 7px;
  border-radius: 3px;
  background: #f0f5f9;
  color: var(--accent);
  font-size: 0.76rem;
  font-weight: 700;
  letter-spacing: 0.02em;
}

.pub-authors {
  margin-bottom: 2px;
  font-size: 0.88rem;
  color: #555;
}

.pub-title {
  font-size: 0.94rem;
  line-height: 1.55;
}

.pub-journal {
  margin-top: 2px;
  color: #777;
  font-size: 0.82rem;
  font-style: italic;
}

/* ---------- Lists ---------- */

#about-en ul,
#about-zh ul {
  padding-left: 20px;
}

#about-en li,
#about-zh li {
  margin-bottom: 5px;
}

/* ---------- News ---------- */

.news-item {
  margin-bottom: 9px;
  font-size: 0.92rem;
}

.news-date {
  display: inline-block;
  min-width: 72px;
  color: var(--accent);
  font-weight: 650;
}

/* ---------- Experience / Education ---------- */

.timeline-item {
  margin: 0 0 25px 0;
  padding-left: 16px;
  border-left: 2px solid #e5e9ed;
}

.timeline-title {
  margin-bottom: 2px;
  font-size: 1rem;
  font-weight: 650;
}

.timeline-role {
  margin-bottom: 3px;
  color: #555;
  font-size: 0.9rem;
}

.timeline-date {
  margin-bottom: 8px;
  color: #888;
  font-size: 0.82rem;
  font-style: italic;
}

/* ---------- Collaboration ---------- */

.collaboration-box {
  margin-top: 8px;
  padding: 17px 20px;
  background: var(--soft);
  border-left: 3px solid var(--accent);
  border-radius: 3px;
}

/* ---------- Mobile ---------- */

@media (max-width: 700px) {

  #about-en,
  #about-zh {
    max-width: 100%;
  }

  #about-en h1,
  #about-zh h1 {
    font-size: 2rem;
  }

  .research-grid {
    grid-template-columns: 1fr;
  }

  .profile-links a {
    display: inline-block;
    margin-bottom: 6px;
  }

  .news-date {
    min-width: 62px;
  }
}

</style>


<!-- ========================================================= -->
<!-- ==================== LANGUAGE SWITCHER ================== -->
<!-- ========================================================= -->

<div id="lang-switcher">

  <button
    onclick="setAboutLang('en')"
    id="btn-en">
    English
  </button>

  <button
    onclick="setAboutLang('zh')"
    id="btn-zh">
    中文
  </button>

</div>


<!-- ========================================================= -->
<!-- ======================== ENGLISH ========================= -->
<!-- ========================================================= -->

<div id="about-en" markdown="1">

# Zehao Wang

<div class="profile-subtitle">
<strong>Third-year Ph.D. Student in Software Engineering, Tianjin University</strong>
</div>

<div class="profile-description">

I study **reliable and self-improving LLM agents and multi-agent systems**.  
My research focuses on how agents can **make reliable decisions, coordinate effectively, diagnose failures, and continuously improve from interaction and experience**.

My current interests lie at the intersection of **Multi-Agent Systems, Agent Reinforcement Learning, Epistemic Reasoning, and Trustworthy AI**, with an emphasis on building agent systems that can reason about their own decisions and learn better strategies over time.

</div>

<div class="profile-links">

[Google Scholar](https://scholar.google.com/) ·
[GitHub](https://github.com/) ·
[Email](mailto:your-email@example.com) ·
[CV](/files/CV.pdf)

</div>


---

# News

<div class="news-item">
<span class="news-date">2026.08</span>
Our work on failure reasoning in LLM-based multi-agent systems was accepted to <strong>EMNLP 2026</strong>.
</div>

<div class="news-item">
<span class="news-date">2026.05</span>
Our work on epistemic calibration in LLM-based multi-agent planning was accepted to <strong>ICML 2026</strong>.
</div>

<div class="news-item">
<span class="news-date">2026.01</span>
Our work on illicit account detection based on user behavior sequences was accepted to <strong>WWW 2026</strong>.
</div>

<div class="news-item">
<span class="news-date">2026</span>
Continuing research on <strong>reliable and self-improving LLM agents</strong>.
</div>


---

# Publications

<div class="pub-section">

### LLM Agents & Multi-Agent Systems

<div class="pub-item">

<span class="pub-venue">EMNLP 2026</span>

<div class="pub-authors">
<strong>Zehao Wang</strong>, Lanjun Wang, Shilong Jin, Junjie Chen, Yanghua Xiao.
</div>

<div class="pub-title">
<em>DCFA: Dual-view Causal Attribution for Failure Reasoning in LLM-based Multi-agent Systems.</em>
</div>

</div>


<div class="pub-item">

<span class="pub-venue">ICML 2026</span>

<div class="pub-authors">
<strong>Zehao Wang</strong>, Shilong Jin, Zhao Cao, Lanjun Wang.
</div>

<div class="pub-title">
<em>When Planning Fails Despite Correct Execution: On Epistemic Calibration for LLM-Based Multi-Agent Systems.</em>
</div>

</div>


### Trustworthy AI & Risk Control

<div class="pub-item">

<span class="pub-venue">WWW 2026</span>

<div class="pub-authors">
<strong>Zehao Wang</strong>, Lanjun Wang, Fuxia Guo, Yanjie Dong.
</div>

<div class="pub-title">
<em>Pattern-aware Illicit Account Detection based on User Behavior Sequences.</em>
</div>

</div>


<div class="pub-item">

<span class="pub-venue">DASFAA 2026</span>

<div class="pub-authors">
<strong>Zehao Wang</strong>, Lanjun Wang.
</div>

<div class="pub-title">
<em>NK-GAD: Neighbor Knowledge-Enhanced Unsupervised Graph Anomaly Detection.</em>
</div>

</div>


<div class="pub-item">

<span class="pub-venue">MIR 2026</span>

<div class="pub-authors">
<strong>Zehao Wang</strong>, Lanjun Wang.
</div>

<div class="pub-title">
<em>Reasoning-targeted Jailbreak Attacks on Large Reasoning Models via Semantic Triggers and Psychological Framing.</em>
</div>

<div class="pub-journal">
Machine Intelligence Research.
</div>

</div>


<div class="pub-item">

<span class="pub-venue">TIFS 2025</span>

<div class="pub-authors">
Jin Fan, Zheyu Wang, <strong>Zehao Wang</strong>, Jiajun Yang, Huifeng Wu, Jia Wu.
</div>

<div class="pub-title">
<em>Enhancing GCN Robustness Against Structural Attacks via Adaptive Spectrum Filtering.</em>
</div>

<div class="pub-journal">
IEEE Transactions on Information Forensics and Security.
</div>

</div>


<div class="pub-item">

<span class="pub-venue">Neurocomputing 2025</span>

<div class="pub-authors">
Jin Fan, <strong>Zehao Wang</strong><sup>★</sup>, Feiwei Qin, Huifeng Wu, Danfeng Sun, Jia Wu.
</div>

<div class="pub-title">
<em>A distribution feature extracting network with dual correlation for long sequence time-series forecasting.</em>
</div>

<div class="pub-journal">
★ Corresponding Author
</div>

</div>


<div class="pub-item">

<span class="pub-venue">TAI 2024</span>

<div class="pub-authors">
<strong>Zehao Wang</strong>, Jin Fan, Huifeng Wu, Danfeng Sun, Jia Wu.
</div>

<div class="pub-title">
<em>Representing Multi-view Time-series Graph Structures for Multivariate Long-term Time-series Forecasting.</em>
</div>

<div class="pub-journal">
IEEE Transactions on Artificial Intelligence.
</div>

</div>


<div class="pub-item">

<span class="pub-venue">CIKM 2024</span>

<div class="pub-authors">
Lanjun Wang, <strong>Zehao Wang</strong>, Le Wu, An-An Liu.
</div>

<div class="pub-title">
<em>Bots Shield Fake News: Adversarial Attack on User Engagement-based Fake News Detection.</em>
</div>

</div>


<div class="pub-item">

<span class="pub-venue">FGCS 2023</span>

<div class="pub-authors">
<strong>Zehao Wang</strong>, Huifeng Wu, Jin Fan, Danfeng Sun, Jia Wu.
</div>

<div class="pub-title">
<em>A robust feature reinforcement framework for heterogeneous graphs neural networks.</em>
</div>

<div class="pub-journal">
Future Generation Computer Systems.
</div>

</div>


<div class="pub-item">

<span class="pub-venue">Neural Networks 2023</span>

<div class="pub-authors">
Jin Fan, <strong>Zehao Wang</strong>, Huifeng Wu, Danfeng Sun, Jia Wu, Xin Lu.
</div>

<div class="pub-title">
<em>An Adversarial Time-Frequency Reconstruction Network for Unsupervised Anomaly Detection.</em>
</div>

</div>


<div class="pub-item">

<span class="pub-venue">TETC 2022</span>

<div class="pub-authors">
Jin Fan, <strong>Zehao Wang</strong>, Danfeng Sun, Huifeng Wu.
</div>

<div class="pub-title">
<em>Sepformer-based Models: More Efficient Models for Long Sequence Time-Series Forecasting.</em>
</div>

<div class="pub-journal">
IEEE Transactions on Emerging Topics in Computing.
</div>

</div>

</div>


---

# Research

My research is organized around a central question:

> **How can LLM agents become more reliable and continuously improve from their own experience?**

<div class="research-grid">

<div class="research-card">

### Reliable LLM Agents

I study agent reliability from a **decision-centric and epistemic perspective**, focusing on whether agents possess and appropriately use the knowledge required for reliable decisions.

<ul>
<li>Epistemic calibration</li>
<li>Decision reliability</li>
<li>Reliable planning & execution</li>
<li>Failure diagnosis & attribution</li>
</ul>

</div>


<div class="research-card">

### Self-Improving Agents

I investigate how agents can **learn from interaction, experience, and failures** rather than relying solely on static prompts or external supervision.

<ul>
<li>Agent reinforcement learning</li>
<li>Long-horizon trajectories</li>
<li>Credit assignment</li>
<li>Self-evolving agents</li>
</ul>

</div>


<div class="research-card">

### Trustworthy AI

I work on trustworthy AI and intelligent risk-control systems, where **behavioral modeling, reasoning, and anomaly detection** intersect.

<ul>
<li>Risk reasoning & intervention</li>
<li>LLM safety & robustness</li>
<li>Graph & temporal anomaly detection</li>
<li>Illicit-account detection</li>
</ul>

</div>

</div>


---

# Research Projects

### Reliable Multi-Agent Systems

Developing methods to improve the reliability of LLM-based multi-agent systems through **epistemic calibration, failure attribution, hierarchical intervention, and structured reasoning**.

### Self-Evolving Agent Systems

Exploring **online knowledge evolution and agent reinforcement learning** to enable agents to learn useful decision knowledge from interaction and continuously improve their behavior.

### AI Risk Control

Applying **LLM reasoning, behavioral modeling, graph learning, and anomaly detection** to intelligent risk detection and intervention in real-world systems.


---

# Honors & Awards

- **National Scholarship**, Ministry of Education of China, **2023**
- **Huawei Scholarship**, **2023**
- **Silver Award**, China International College Students' Innovation and Entrepreneurship Competition, **International Track, 2024**


---

# Research Grants & Leadership

- **Principal Investigator**, General Research Project, Zhejiang Provincial Department of Education, **2022–2023**
- **Principal Investigator**, Zhejiang Province Xinmiao Talent Program, **2023–2024**
- **Student Lead**, Tencent Rhino-Bird Research Program, **2024–2025**
  - Led the overall research and technical development.
  - Responsible for core technical development, experiments, and project delivery.
  - Project received **Excellent Project Completion (Top 25%)**.


---

# Research & Industry Experience

<div class="timeline-item">

<div class="timeline-title">
Huawei / FusionServer Research Institute
</div>

<div class="timeline-role">
<strong>Research / System Architect</strong>
</div>

<div class="timeline-date">
2025.11 – Present
</div>

<ul>
<li>Research on reliable LLM-based multi-agent systems.</li>
<li>Agent failure diagnosis, attribution, and system-level reliability.</li>
<li>Multi-agent workflow design and evaluation.</li>
<li>Research translation toward large-scale enterprise AI systems.</li>
</ul>

</div>


<div class="timeline-item">

<div class="timeline-title">
Tencent WeChat / Tencent Rhino-Bird Research Program
</div>

<div class="timeline-role">
<strong>Student Lead — Intelligent Risk Control Research Project</strong>
</div>

<div class="timeline-date">
2024.11 – 2025.08
</div>

<ul>
<li>Led the overall research and technical development.</li>
<li>User behavior modeling and illicit-account detection.</li>
<li>Behavioral sequence analysis and anomaly detection.</li>
<li>Core technical development, experimental evaluation, and project delivery.</li>
<li>Project received <strong>Excellent Project Completion (Top 25%)</strong>.</li>
</ul>

</div>


---

# Education

<div class="timeline-item">

<div class="timeline-title">
Tianjin University
</div>

<div class="timeline-role">
<strong>Ph.D. Student in Software Engineering</strong>
</div>

<div class="timeline-date">
2024.09 – 2028.06
</div>

</div>


<div class="timeline-item">

<div class="timeline-title">
Hangzhou Dianzi University
</div>

<div class="timeline-role">
<strong>M.S. in Computer Technology</strong>
</div>

<div class="timeline-date">
2021.09 – 2024.06
</div>

</div>


<div class="timeline-item">

<div class="timeline-title">
Xidian University
</div>

<div class="timeline-role">
<strong>B.Eng. in Communication Engineering</strong>
</div>

<div class="timeline-date">
2016.09 – 2020.06
</div>

</div>


---

# Research Collaboration

<div class="collaboration-box">

I am interested in research collaborations on:

- LLM agents and multi-agent systems
- Agent reinforcement learning
- Reliable and trustworthy AI
- Agent reasoning and decision making
- Self-improving and self-evolving agents

If you are interested in discussing research ideas or potential collaboration, feel free to reach out.

</div>


</div>


<!-- ========================================================= -->
<!-- ========================== 中文 ========================== -->
<!-- ========================================================= -->

<div id="about-zh" markdown="1" style="display:none;">

# 王则昊

<div class="profile-subtitle">
<strong>天津大学软件工程博士三年级研究生</strong>
</div>

<div class="profile-description">

我的研究主要聚焦于**可靠且能够持续自我改进的大语言模型智能体（LLM Agents）与多智能体系统（Multi-Agent Systems）**。

我关注智能体如何**做出可靠决策、进行有效协作、理解和诊断自身失败，并从交互经验中持续学习和改进**。

目前的研究主要位于 **Multi-Agent Systems、Agent Reinforcement Learning、Epistemic Reasoning 与 Trustworthy AI** 的交叉领域，重点探索如何让智能体具备更加可靠的决策能力，以及如何通过经验和强化学习实现持续自我改进。

</div>

<div class="profile-links">

[Google Scholar](https://scholar.google.com/) ·
[GitHub](https://github.com/) ·
[Email](mailto:your-email@example.com) ·
[CV](/files/CV.pdf)

</div>


---

# 最新动态

<div class="news-item">
<span class="news-date">2026.08</span>
关于 LLM-based Multi-Agent Systems 失败推理的工作被 <strong>EMNLP 2026</strong> 接收。
</div>

<div class="news-item">
<span class="news-date">2026.05</span>
关于 LLM-based Multi-Agent Systems 认知校准的工作被 <strong>ICML 2026</strong> 接收。
</div>

<div class="news-item">
<span class="news-date">2026.01</span>
关于用户行为序列与黑产账户检测的工作被 <strong>WWW 2026</strong> 接收。
</div>

<div class="news-item">
<span class="news-date">2026</span>
持续开展<strong>可靠、自我改进型 LLM Agent</strong>相关研究。
</div>


---

# 论文发表

<div class="pub-section">

### LLM Agents & Multi-Agent Systems

<div class="pub-item">

<span class="pub-venue">EMNLP 2026</span>

<div class="pub-authors">
<strong>Zehao Wang</strong>, Lanjun Wang, Shilong Jin, Junjie Chen, Yanghua Xiao.
</div>

<div class="pub-title">
<em>DCFA: Dual-view Causal Attribution for Failure Reasoning in LLM-based Multi-agent Systems.</em>
</div>

</div>


<div class="pub-item">

<span class="pub-venue">ICML 2026</span>

<div class="pub-authors">
<strong>Zehao Wang</strong>, Shilong Jin, Zhao Cao, Lanjun Wang.
</div>

<div class="pub-title">
<em>When Planning Fails Despite Correct Execution: On Epistemic Calibration for LLM-Based Multi-Agent Systems.</em>
</div>

</div>


### Trustworthy AI & Risk Control

<div class="pub-item">

<span class="pub-venue">WWW 2026</span>

<div class="pub-authors">
<strong>Zehao Wang</strong>, Lanjun Wang, Fuxia Guo, Yanjie Dong.
</div>

<div class="pub-title">
<em>Pattern-aware Illicit Account Detection based on User Behavior Sequences.</em>
</div>

</div>


<div class="pub-item">

<span class="pub-venue">DASFAA 2026</span>

<div class="pub-authors">
<strong>Zehao Wang</strong>, Lanjun Wang.
</div>

<div class="pub-title">
<em>NK-GAD: Neighbor Knowledge-Enhanced Unsupervised Graph Anomaly Detection.</em>
</div>

</div>


<div class="pub-item">

<span class="pub-venue">MIR 2026</span>

<div class="pub-authors">
<strong>Zehao Wang</strong>, Lanjun Wang.
</div>

<div class="pub-title">
<em>Reasoning-targeted Jailbreak Attacks on Large Reasoning Models via Semantic Triggers and Psychological Framing.</em>
</div>

<div class="pub-journal">
Machine Intelligence Research.
</div>

</div>


<div class="pub-item">

<span class="pub-venue">TIFS 2025</span>

<div class="pub-authors">
Jin Fan, Zheyu Wang, <strong>Zehao Wang</strong>, Jiajun Yang, Huifeng Wu, Jia Wu.
</div>

<div class="pub-title">
<em>Enhancing GCN Robustness Against Structural Attacks via Adaptive Spectrum Filtering.</em>
</div>

<div class="pub-journal">
IEEE Transactions on Information Forensics and Security.
</div>

</div>


<div class="pub-item">

<span class="pub-venue">Neurocomputing 2025</span>

<div class="pub-authors">
Jin Fan, <strong>Zehao Wang</strong><sup>★</sup>, Feiwei Qin, Huifeng Wu, Danfeng Sun, Jia Wu.
</div>

<div class="pub-title">
<em>A distribution feature extracting network with dual correlation for long sequence time-series forecasting.</em>
</div>

<div class="pub-journal">
★ Corresponding Author
</div>

</div>


<div class="pub-item">

<span class="pub-venue">TAI 2024</span>

<div class="pub-authors">
<strong>Zehao Wang</strong>, Jin Fan, Huifeng Wu, Danfeng Sun, Jia Wu.
</div>

<div class="pub-title">
<em>Representing Multi-view Time-series Graph Structures for Multivariate Long-term Time-series Forecasting.</em>
</div>

<div class="pub-journal">
IEEE Transactions on Artificial Intelligence.
</div>

</div>


<div class="pub-item">

<span class="pub-venue">CIKM 2024</span>

<div class="pub-authors">
Lanjun Wang, <strong>Zehao Wang</strong>, Le Wu, An-An Liu.
</div>

<div class="pub-title">
<em>Bots Shield Fake News: Adversarial Attack on User Engagement-based Fake News Detection.</em>
</div>

</div>


<div class="pub-item">

<span class="pub-venue">FGCS 2023</span>

<div class="pub-authors">
<strong>Zehao Wang</strong>, Huifeng Wu, Jin Fan, Danfeng Sun, Jia Wu.
</div>

<div class="pub-title">
<em>A robust feature reinforcement framework for heterogeneous graphs neural networks.</em>
</div>

<div class="pub-journal">
Future Generation Computer Systems.
</div>

</div>


<div class="pub-item">

<span class="pub-venue">Neural Networks 2023</span>

<div class="pub-authors">
Jin Fan, <strong>Zehao Wang</strong>, Huifeng Wu, Danfeng Sun, Jia Wu, Xin Lu.
</div>

<div class="pub-title">
<em>An Adversarial Time-Frequency Reconstruction Network for Unsupervised Anomaly Detection.</em>
</div>

</div>


<div class="pub-item">

<span class="pub-venue">TETC 2022</span>

<div class="pub-authors">
Jin Fan, <strong>Zehao Wang</strong>, Danfeng Sun, Huifeng Wu.
</div>

<div class="pub-title">
<em>Sepformer-based Models: More Efficient Models for Long Sequence Time-Series Forecasting.</em>
</div>

<div class="pub-journal">
IEEE Transactions on Emerging Topics in Computing.
</div>

</div>

</div>


---

# 研究方向

我的研究围绕一个核心问题展开：

> **如何让 LLM Agent 做出更加可靠的决策，并能够从自身经验中持续学习和改进？**

<div class="research-grid">

<div class="research-card">

### Reliable LLM Agents

从**决策与认知（epistemic）视角**研究 LLM Agent 的可靠性，重点关注智能体是否拥有并能够正确使用支撑可靠决策所需的知识。

<ul>
<li>认知校准与决策可靠性</li>
<li>Agent Planning 与 Execution 可靠性</li>
<li>Agent Failure Diagnosis 与 Attribution</li>
</ul>

</div>


<div class="research-card">

### Self-Improving Agents

研究智能体如何从**交互、经验和失败中学习**，而不是完全依赖静态 Prompt 或外部监督。

<ul>
<li>Agent Reinforcement Learning</li>
<li>长程 Agent Trajectory 探索</li>
<li>Credit Assignment 与策略学习</li>
<li>Self-improving / Self-evolving Agents</li>
</ul>

</div>


<div class="research-card">

### Trustworthy AI & 风险控制

研究可信人工智能与智能风险控制，重点关注**行为建模、推理与异常检测**的结合。

<ul>
<li>风险推理与智能干预</li>
<li>LLM 安全与对抗鲁棒性</li>
<li>图与时序异常检测</li>
<li>黑产账户与恶意用户检测</li>
</ul>

</div>

</div>


---

# 研究项目

### Reliable Multi-Agent Systems

研究通过**认知校准、失败归因、分级干预与结构化推理**提升 LLM-based Multi-Agent Systems 可靠性的方法。

### Self-Evolving Agent Systems

研究 **Online Knowledge Evolution 与 Agent Reinforcement Learning**，使智能体能够从交互过程中积累有效的决策知识，并持续改进自身行为。

### AI Risk Control

结合 **LLM 推理、用户行为建模、图学习与异常检测**，研究面向真实场景的智能风险识别与干预。


---

# 荣誉与奖励

- **国家奖学金**，教育部，**2023**
- **华为奖学金**，**2023**
- **中国国际大学生创新大赛（原“互联网+”）国际赛道银奖**，**2024**


---

# 科研项目与科研领导力

- **项目主持人（Principal Investigator）**，浙江省教育厅一般科研项目，**2022–2023**
- **项目主持人（Principal Investigator）**，浙江省新苗人才计划，**2023–2024**
- **学生负责人（Student Lead）**，腾讯犀牛鸟科研项目，**2024–2025**
  - 负责项目整体科研工作与技术方案设计。
  - 负责核心技术开发、实验验证与项目成果交付。
  - 项目获腾讯犀牛鸟**优秀结项，位列前 25%**。


---

# 科研与产业经历

<div class="timeline-item">

<div class="timeline-title">
华为 / 超聚变中央研究院
</div>

<div class="timeline-role">
<strong>Research / System Architect</strong>
</div>

<div class="timeline-date">
2025.11 – Present
</div>

<ul>
<li>可靠 LLM-based Multi-Agent Systems 研究。</li>
<li>Agent Failure Diagnosis、Attribution 与系统可靠性研究。</li>
<li>Multi-Agent Workflow 设计与系统评估。</li>
<li>面向企业级 AI 系统的研究成果转化。</li>
</ul>

</div>


<div class="timeline-item">

<div class="timeline-title">
腾讯微信 / 腾讯犀牛鸟科研项目
</div>

<div class="timeline-role">
<strong>学生负责人（Student Lead）— 智能风控研究项目</strong>
</div>

<div class="timeline-date">
2024.11 – 2025.08
</div>

<ul>
<li>负责项目整体科研工作与技术方案设计。</li>
<li>开展黑产账户检测与用户行为建模研究。</li>
<li>设计并实现用户行为序列分析与异常检测方法。</li>
<li>负责核心技术开发、实验验证与项目成果交付。</li>
<li>项目获腾讯犀牛鸟<strong>优秀结项，位列前 25%</strong>。</li>
</ul>

</div>


---

# 教育经历

<div class="timeline-item">

<div class="timeline-title">
天津大学
</div>

<div class="timeline-role">
<strong>软件工程博士</strong>
</div>

<div class="timeline-date">
2024.09 – 2028.06
</div>

</div>


<div class="timeline-item">

<div class="timeline-title">
杭州电子科技大学
</div>

<div class="timeline-role">
<strong>计算机技术硕士</strong>
</div>

<div class="timeline-date">
2021.09 – 2024.06
</div>

</div>


<div class="timeline-item">

<div class="timeline-title">
西安电子科技大学
</div>

<div class="timeline-role">
<strong>通信工程学士</strong>
</div>

<div class="timeline-date">
2016.09 – 2020.06
</div>

</div>


---

# 学术合作

<div class="collaboration-box">

欢迎围绕以下方向进行学术交流与合作：

- LLM Agents 与 Multi-Agent Systems
- Agent Reinforcement Learning
- Reliable & Trustworthy AI
- Agent Reasoning 与 Decision Making
- Self-Improving / Self-Evolving Agents

如果你对相关研究方向感兴趣，欢迎通过 Email 与我联系。

</div>


</div>


<!-- ========================================================= -->
<!-- ======================== SCRIPT ========================== -->
<!-- ========================================================= -->

<script>

function setAboutLang(lang) {

  var en = document.getElementById('about-en');
  var zh = document.getElementById('about-zh');

  var btnZh = document.getElementById('btn-zh');
  var btnEn = document.getElementById('btn-en');

  var showEn = lang !== 'zh';

  zh.style.display = showEn ? 'none' : 'block';
  en.style.display = showEn ? 'block' : 'none';

  btnZh.style.fontWeight = showEn ? '400' : '600';
  btnEn.style.fontWeight = showEn ? '600' : '400';

  btnZh.style.color = showEn ? '#888' : '#222';
  btnEn.style.color = showEn ? '#222' : '#888';

  try {
    localStorage.setItem('aboutLang', lang);
  } catch (e) {}

}

(function() {

  var lang = 'en';

  try {

    var savedLang = localStorage.getItem('aboutLang');

    if (savedLang === 'zh' || savedLang === 'en') {
      lang = savedLang;
    }

  } catch (e) {}

  setAboutLang(lang);

})();

</script>
