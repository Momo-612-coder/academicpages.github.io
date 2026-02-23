---
title: "大三（上）——工效学"
collection: publications
category: conferences
permalink: /publication/2025-10-ergonomics
excerpt: "本研究面向 **甲/乙类仓储火灾** 高危环境，基于 **人机工效学（Ergonomics）** 和 **Wickens 多资源理论**，设计并验证了一套 **异构人机协同智能救援系统**，融合 **Gemini 多模态大模型** 与 **AR 导航 UI**，显著优化了救援认知负荷和行动绩效。
"
date: 2025-10-17
#venue: 'GitHub Journal of Bugs'
#paperurl: 'http://academicpages.github.io/files/paper3.pdf'
#citation: 'Your Name, You. (2024). &quot;Paper Title Number 3.&quot; <i>GitHub Journal of Bugs</i>. 1(3).'
---

## Abstract
You can get more information just clicking here：[工效学遥操UI系统设计报告]({{ site.baseurl }}/files/ergonomics(5).pdf). 

<img src="{{ site.baseurl }}/images/ergonomics(5).jpg" alt="ergonomics(5)" style="display:block; margin:0 auto 1rem auto; max-width:100%; width:560px; height:auto;" />

**Background and Objective:**  
Warehouse fires of **Class A/B** present highly hazardous conditions. Dense smoke and complex structures often result in **spatial disorientation** and **cognitive overload** for rescue personnel. To overcome limitations of traditional “perception‑decision” models in rescue operations, this study develops a **heterogeneous human-robot teaming** system grounded in **human factors engineering** and **Wickens' Multiple Resource Theory**.

**Methods:**  
The system innovatively integrates the **Gemini Large Multi-modal Model (LMM)**.  
- **Front-end:** Sensor-equipped robots generate **dynamic environment maps**, capturing temperature fields, structural stress, and toxic gas concentrations.  
- **Back-end:** The **A.I.V.A. (Artificial Intelligence Visual Assistant)** uses the Gemini API to convert complex heterogeneous sensor data into **intuitive semantic tactical recommendations** (e.g., “Explosive detected, avoid this zone”) displayed via **AR head-mounted displays** for low cognitive-load visualization.  
- **Simulation:** High-fidelity fire environments were constructed in **Unity 3D**, employing a **Within‑Subjects Crossover Design** to compare rescue performance **with** and **without system assistance**.

**Results:**  
The collaborative system significantly improved overall rescue efficiency:  
1. **Cognitive Load Reduction:** NASA-TLX scores decreased by **57% (p < 0.01)**, demonstrating that semantic-level data abstraction by the LMM effectively frees human cognitive resources.  
2. **Operational Performance:** Action efficiency improved by **23.02%**, path decision pauses decreased by **52.7%**, and time spent in dangerous areas was significantly reduced.  
3. **UI‑AI Boundary Condition:** While AR navigation alone greatly aided decision-making, the AI assistant (A.I.V.A.) did not significantly improve performance under low task entropy conditions, highlighting **situational dependency** of LMM benefits.

**Conclusions:**  
The study confirms the feasibility of integrating **large-model intelligence** with **AR visualization** for single-rescuer decision support in extreme environments. The findings provide **empirical support** for developing next-generation **smart firefighting equipment** emphasizing a unified “perception‑computation‑execution” framework, and highlight conditions under which AI enhances human cognitive offloading and operational efficiency.

------