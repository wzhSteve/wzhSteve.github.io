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


<!-- ==================== Language Switcher ==================== -->

<div id="lang-switcher" style="
  margin: 8px 0 28px 0;
  font-size: 0.9rem;
">
  <button
    onclick="setAboutLang('en')"
    id="btn-en"
    style="
      border: none;
      background: none;
      padding: 0;
      margin-right: 14px;
      cursor: pointer;
      color: #222;
    ">
    English
  </button>

  <button
    onclick="setAboutLang('zh')"
    id="btn-zh"
    style="
      border: none;
      background: none;
      padding: 0;
      cursor: pointer;
      color: #888;
    ">
    中文
  </button>
</div>


<!-- ========================================================= -->
<!-- ======================== ENGLISH ========================= -->
<!-- ========================================================= -->

<div id="about-en" markdown="1">

# Zehao Wang

**Third-year Ph.D. Student in Software Engineering, Tianjin University**

I study **reliable and self-improving LLM agents and multi-agent systems**. My research focuses on how agents can **make reliable decisions, coordinate effectively, diagnose failures, and continuously improve from interaction and experience**.

My current interests lie at the intersection of **Multi-Agent Systems, Agent Reinforcement Learning, Epistemic Reasoning, and Trustworthy AI**, with an emphasis on building agent systems that can reason about their own decisions and learn better strategies over time.

[Google Scholar](https://scholar.google.com/) · [GitHub](https://github.com/) · [Email](mailto:your-email@example.com) · [CV](/files/CV.pdf)


---

# 📰 News

- **2026.08** — Our work on failure reasoning in LLM-based multi-agent systems was accepted to **EMNLP 2026**.
- **2026.05** — Our work on epistemic calibration in LLM-based multi-agent planning was accepted to **ICML 2026**.
- **2026.01** — Our work on illicit account detection based on user behavior sequences was accepted to **WWW 2026**.
- **2026** — Continuing research on **reliable and self-improving LLM agents**.


---

# 🔬 Research

My research is organized around a central question:

> **How can LLM agents become more reliable and continuously improve from their own experience?**

### Reliable LLM Agents

I study the reliability of LLM-based agents from a **decision-centric and epistemic perspective**, focusing on whether agents possess and appropriately use the knowledge required for reliable decisions.

- Epistemic calibration and decision reliability
- Reliable planning and execution
- Failure diagnosis and attribution
- Causal-inspired reasoning for agent decisions
- Hierarchical intervention and decision correction

### Self-Improving Agents

I investigate how agents can **learn from interaction, experience, and failures** rather than relying solely on static prompts or external supervision.

- Agent reinforcement learning
- Long-horizon trajectory exploration
- Credit assignment and strategy learning
- Online knowledge evolution
- Self-improving and self-evolving agents

### Trustworthy AI & Risk Control

I also work on trustworthy AI and intelligent risk-control systems, particularly where **behavioral modeling, reasoning, and anomaly detection** intersect.

- Risk reasoning and intelligent intervention
- LLM safety and adversarial robustness
- User behavior modeling
- Graph and temporal anomaly detection
- Illicit-account and malicious-user detection


---

# 📝 Publications

### LLM Agents & Multi-Agent Systems

- **[EMNLP 2026]**  
  **Zehao Wang**, Lanjun Wang, Shilong Jin, Junjie Chen, Yanghua Xiao.  
  *DCFA: Dual-view Causal Attribution for Failure Reasoning in LLM-based Multi-agent Systems.*

- **[ICML 2026]**  
  **Zehao Wang**, Shilong Jin, Zhao Cao, Lanjun Wang.  
  *When Planning Fails Despite Correct Execution: On Epistemic Calibration for LLM-Based Multi-Agent Systems.*

### Trustworthy AI & Risk Control

- **[WWW 2026]**  
  **Zehao Wang**, Lanjun Wang, Fuxia Guo, Yanjie Dong.  
  *Pattern-aware Illicit Account Detection based on User Behavior Sequences.*

- **[MIR 2026]**  
  **Zehao Wang**, Lanjun Wang.  
  *Reasoning-targeted Jailbreak Attacks on Large Reasoning Models via Semantic Triggers and Psychological Framing.*  
  *Machine Intelligence Research.*

- **[DASFAA 2026]**  
  **Zehao Wang**, Lanjun Wang.  
  *NK-GAD: Neighbor Knowledge-Enhanced Unsupervised Graph Anomaly Detection.*

- **[TIFS 2025]**  
  Jin Fan, Zheyu Wang, **Zehao Wang**, Jiajun Yang, Huifeng Wu, Jia Wu.  
  *Enhancing GCN Robustness Against Structural Attacks via Adaptive Spectrum Filtering.*  
  *IEEE Transactions on Information Forensics and Security.*

- **[Neurocomputing 2025]**  
  Jin Fan, **Zehao Wang**$^{\star}$ *(Corresponding Author)*, Feiwei Qin, Huifeng Wu, Danfeng Sun, Jia Wu.  
  *A distribution feature extracting network with dual correlation for long sequence time-series forecasting.*

- **[TAI 2024]**  
  **Zehao Wang**, Jin Fan, Huifeng Wu, Danfeng Sun, Jia Wu.  
  *Representing Multi-view Time-series Graph Structures for Multivariate Long-term Time-series Forecasting.*  
  *IEEE Transactions on Artificial Intelligence.*

- **[CIKM 2024]**  
  Lanjun Wang, **Zehao Wang**, Le Wu, An-An Liu.  
  *Bots Shield Fake News: Adversarial Attack on User Engagement-based Fake News Detection.*

- **[Neural Networks 2023]**  
  Jin Fan, **Zehao Wang**, Huifeng Wu, Danfeng Sun, Jia Wu, Xin Lu.  
  *An Adversarial Time-Frequency Reconstruction Network for Unsupervised Anomaly Detection.*

- **[FGCS 2023]**  
  **Zehao Wang**, Huifeng Wu, Jin Fan, Danfeng Sun, Jia Wu.  
  *A robust feature reinforcement framework for heterogeneous graphs neural networks.*

- **[TETC 2022]**  
  Jin Fan, **Zehao Wang**, Danfeng Sun, Huifeng Wu.  
  *Sepformer-based Models: More Efficient Models for Long Sequence Time-Series Forecasting.*
  *IEEE Transactions on Emerging Topics in Computing.*


---

# 🚀 Research Projects

### Reliable Multi-Agent Systems

Developing methods to improve the reliability of LLM-based multi-agent systems through **epistemic calibration, failure attribution, hierarchical intervention, and structured reasoning**.

### Self-Evolving Agent Systems

Exploring **online knowledge evolution and agent reinforcement learning** to enable agents to learn useful decision knowledge from interaction and continuously improve their behavior.

### AI Risk Control

Applying **LLM reasoning, behavioral modeling, graph learning, and anomaly detection** to intelligent risk detection and intervention in real-world systems.


---

# 🏆 Honors & Awards

- **National Scholarship**, Ministry of Education of China, **2023**
- **Huawei Scholarship**, **2023**
- **Silver Award**, China International College Students' Innovation and Entrepreneurship Competition, **International Track, 2024**


---

# 🔬 Research Grants & Leadership

- **Principal Investigator**, General Research Project, Zhejiang Provincial Department of Education, **2022**
- **Principal Investigator**, Zhejiang Province Xinmiao Talent Program, **2023**
- **Student Lead**, Tencent Rhino-Bird Research Program, **2024–2025**
  - Led the overall research and technical development of the project.
  - Responsible for core technical development, experiments, and project delivery.
  - The project received **Excellent Project Completion (Top 25%)**.


---

# 💼 Research & Industry Experience

### Huawei / FusionServer Research Institute

**Research / System Architect**  
*2025.11 – Present*

- Research on reliable LLM-based multi-agent systems.
- Agent failure diagnosis, attribution, and system-level reliability.
- Multi-agent workflow design and evaluation.
- Research translation toward large-scale enterprise AI systems.


### Tencent WeChat / Tencent Rhino-Bird Research Program

**Student Lead — Intelligent Risk Control Research Project**  
*2024.11 – 2025.08*

- Led the overall research and technical development of the project.
- Conducted research on user behavior modeling and illicit-account detection.
- Designed and implemented behavioral sequence analysis and anomaly detection methods.
- Responsible for core technical development, experimental evaluation, and project delivery.
- The project received **Excellent Project Completion (Top 25%)** in the Tencent Rhino-Bird Research Program.


---

# 🎓 Education

### Tianjin University

**Ph.D. Student in Software Engineering**  
*2024.09 – 2028.06*

### Hangzhou Dianzi University

**M.S. in Computer Technology**  
*2021.09 – 2024.06*

### Xidian University

**B.Eng. in Communication Engineering**  
*2016.09 – 2020.06*


---

# 🤝 Research Collaboration

I am interested in research collaborations on:

- LLM agents and multi-agent systems
- Agent reinforcement learning
- Reliable and trustworthy AI
- Agent reasoning and decision making
- Self-improving and self-evolving agents

If you are interested in discussing research ideas or potential collaboration, feel free to reach out.


</div>


<!-- ========================================================= -->
<!-- ========================== 中文 ========================== -->
<!-- ========================================================= -->

<div id="about-zh" markdown="1" style="display:none;">

# 王则昊

**天津大学软件工程博士三年级研究生**

我的研究主要聚焦于**可靠且能够持续自我改进的大语言模型智能体（LLM Agents）与多智能体系统（Multi-Agent Systems）**。

我关注智能体如何**做出可靠决策、进行有效协作、理解和诊断自身失败，并从交互经验中持续学习和改进**。

目前的研究主要位于 **Multi-Agent Systems、Agent Reinforcement Learning、Epistemic Reasoning 与 Trustworthy AI** 的交叉领域，重点探索如何让智能体具备更加可靠的决策能力，以及如何通过经验和强化学习实现持续自我改进。

[Google Scholar](https://scholar.google.com/) · [GitHub](https://github.com/) · [Email](mailto:your-email@example.com) · [CV](/files/CV.pdf)


---

# 📰 最新动态

- **2026.08** — 关于 LLM-based Multi-Agent Systems 失败推理的工作被 **EMNLP 2026** 接收。
- **2026.05** — 关于 LLM-based Multi-Agent Systems 认知校准的工作被 **ICML 2026** 接收。
- **2026.01** — 关于用户行为序列与黑产账户检测的工作被 **WWW 2026** 接收。
- **2026** — 持续开展**可靠、自我改进型 LLM Agent**相关研究。


---

# 🔬 研究方向

我的研究围绕一个核心问题展开：

> **如何让 LLM Agent 做出更加可靠的决策，并能够从自身经验中持续学习和改进？**

### Reliable LLM Agents

从**决策与认知（epistemic）视角**研究 LLM Agent 的可靠性，重点关注智能体是否拥有并能够正确使用支撑可靠决策所需的知识。

- 认知校准与决策可靠性
- Agent Planning 与 Execution 可靠性
- Agent Failure Diagnosis 与 Attribution
- 面向 Agent 决策的因果启发式推理
- 分级干预与决策纠正

### Self-Improving Agents

研究智能体如何从**交互、经验和失败中学习**，而不是完全依赖静态 Prompt 或外部监督。

- Agent Reinforcement Learning
- 长程 Agent Trajectory 探索
- Credit Assignment 与策略学习
- Online Knowledge Evolution
- Self-improving / Self-evolving Agents

### Trustworthy AI & 风险控制

研究可信人工智能与智能风险控制，重点关注**行为建模、推理与异常检测**的结合。

- 风险推理与智能干预
- LLM 安全与对抗鲁棒性
- 用户行为建模
- 图与时序异常检测
- 黑产账户与恶意用户检测


---

# 📝 论文发表

### LLM Agents & Multi-Agent Systems

- **[EMNLP 2026]**  
  **Zehao Wang**, Lanjun Wang, Shilong Jin, Junjie Chen, Yanghua Xiao.  
  *DCFA: Dual-view Causal Attribution for Failure Reasoning in LLM-based Multi-agent Systems.*

- **[ICML 2026]**  
  **Zehao Wang**, Shilong Jin, Zhao Cao, Lanjun Wang.  
  *When Planning Fails Despite Correct Execution: On Epistemic Calibration for LLM-Based Multi-Agent Systems.*

### Trustworthy AI & Risk Control

- **[WWW 2026]**  
  **Zehao Wang**, Lanjun Wang, Fuxia Guo, Yanjie Dong.  
  *Pattern-aware Illicit Account Detection based on User Behavior Sequences.*

- **[MIR 2026]**  
  **Zehao Wang**, Lanjun Wang.  
  *Reasoning-targeted Jailbreak Attacks on Large Reasoning Models via Semantic Triggers and Psychological Framing.*  
  *Machine Intelligence Research.*

- **[DASFAA 2026]**  
  **Zehao Wang**, Lanjun Wang.  
  *NK-GAD: Neighbor Knowledge-Enhanced Unsupervised Graph Anomaly Detection.*

- **[TIFS 2025]**  
  Jin Fan, Zheyu Wang, **Zehao Wang**, Jiajun Yang, Huifeng Wu, Jia Wu.  
  *Enhancing GCN Robustness Against Structural Attacks via Adaptive Spectrum Filtering.*  
  *IEEE Transactions on Information Forensics and Security.*

- **[Neurocomputing 2025]**  
  Jin Fan, **Zehao Wang**$^{\star}$ *(Corresponding Author)*, Feiwei Qin, Huifeng Wu, Danfeng Sun, Jia Wu.  
  *A distribution feature extracting network with dual correlation for long sequence time-series forecasting.*

- **[TAI 2024]**  
  **Zehao Wang**, Jin Fan, Huifeng Wu, Danfeng Sun, Jia Wu.  
  *Representing Multi-view Time-series Graph Structures for Multivariate Long-term Time-series Forecasting.*  
  *IEEE Transactions on Artificial Intelligence.*

- **[CIKM 2024]**  
  Lanjun Wang, **Zehao Wang**, Le Wu, An-An Liu.  
  *Bots Shield Fake News: Adversarial Attack on User Engagement-based Fake News Detection.*

- **[Neural Networks 2023]**  
  Jin Fan, **Zehao Wang**, Huifeng Wu, Danfeng Sun, Jia Wu, Xin Lu.  
  *An Adversarial Time-Frequency Reconstruction Network for Unsupervised Anomaly Detection.*

- **[FGCS 2023]**  
  **Zehao Wang**, Huifeng Wu, Jin Fan, Danfeng Sun, Jia Wu.  
  *A robust feature reinforcement framework for heterogeneous graphs neural networks.*

- **[TETC 2022]**  
  Jin Fan, **Zehao Wang**, Danfeng Sun, Huifeng Wu.  
  *Sepformer-based Models: More Efficient Models for Long Sequence Time-Series Forecasting.*
  *IEEE Transactions on Emerging Topics in Computing.*


---

# 🚀 研究项目

### Reliable Multi-Agent Systems

研究通过**认知校准、失败归因、分级干预与结构化推理**提升 LLM-based Multi-Agent Systems 可靠性的方法。

### Self-Evolving Agent Systems

研究 **Online Knowledge Evolution 与 Agent Reinforcement Learning**，使智能体能够从交互过程中积累有效的决策知识，并持续改进自身行为。

### AI Risk Control

结合 **LLM 推理、用户行为建模、图学习与异常检测**，研究面向真实场景的智能风险识别与干预。


---

# 🏆 荣誉与奖励

- **国家奖学金**，教育部，**2023**
- **华为奖学金**，**2023**
- **中国国际大学生创新大赛（原“互联网+”）国际赛道银奖**，**2024**


---

# 🔬 科研项目与科研领导力

- **项目主持人（Principal Investigator）**，浙江省教育厅一般科研项目，**2022-2023**
- **项目主持人（Principal Investigator）**，浙江省新苗人才计划，**2023-2024**
- **学生负责人（Student Lead）**，腾讯犀牛鸟科研项目，**2024–2025**
  - 负责项目整体科研工作与技术方案设计。
  - 负责核心技术开发、实验验证与项目成果交付。
  - 项目获腾讯犀牛鸟**优秀结项，位列前 25%**。


---

# 💼 科研与产业经历

### 华为 / 超聚变中央研究院

**Research / System Architect**  
*2025.11 – Present*

- 可靠 LLM-based Multi-Agent Systems 研究。
- Agent Failure Diagnosis、Attribution 与系统可靠性研究。
- Multi-Agent Workflow 设计与系统评估。
- 面向企业级 AI 系统的研究成果转化。


### 腾讯微信 / 腾讯犀牛鸟科研项目

**学生负责人（Student Lead）— 智能风控研究项目**  
*2024.11 – 2025.08*

- 负责项目整体科研工作与技术方案设计。
- 开展黑产账户检测与用户行为建模研究。
- 设计并实现用户行为序列分析与异常检测方法。
- 负责核心技术开发、实验验证与项目成果交付。
- 项目获腾讯犀牛鸟**优秀结项，位列前 25%**。


---

# 🎓 教育经历

### 天津大学

**软件工程博士**  
*2024.09 – 2028.06*

### 杭州电子科技大学

**计算机技术硕士**  
*2021.09 – 2024.06*

### 西安电子科技大学

**通信工程学士**  
*2016.09 – 2020.06*


---

# 🤝 学术合作

欢迎围绕以下方向进行学术交流与合作：

- LLM Agents 与 Multi-Agent Systems
- Agent Reinforcement Learning
- Reliable & Trustworthy AI
- Agent Reasoning 与 Decision Making
- Self-Improving / Self-Evolving Agents

如果你对相关研究方向感兴趣，欢迎通过 Email 与我联系。


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
