# 📚 **Research Paper Library**

A curated library of papers structured around the **four leading pathways toward generalized humanoid robot control**, along with supporting domains such as perception, mechatronics, locomotion, and space robotics.

These categories reflect how top labs—**Sunday Robotics, Google DeepMind, MIT, CMU, Berkeley, TRI, FAIR, NVIDIA**—conceptualize the modern landscape of humanoid learning.

---

# 🧠 **Three Major Methods for General-Purpose Humanoid Controllers**

Current research in humanoid robot intelligence converges around four dominant paradigms. Each represents a different philosophy for scaling robot capabilities.

---

# 1️⃣ **UMI Imitation Learning (Large-Scale Action Foundations)**

UMI-style controllers learn **directly from large-scale human demonstrations**, providing expressive, high-frequency motor control.

### **Key ideas**

- Large, diverse human teleop datasets
- Low-level torque/velocity commands
- Diffusion or transformer policies
- No reward engineering — pure behavioral cloning
- Excellent contact-rich manipulation + loco-manipulation

### **Strengths**

- Extremely human-like
- Robust contact behavior
- Highly expressive actions
- Scales with data (like language models or vision models)

### **Limitations**

- Requires large amounts of high-quality demonstrations
- Does not inherently understand language unless paired with VLA models

<!--
# 2️⃣ **Vision-Language-Action (VLA) Generalist Models**

VLA models extend IL with **language-conditioned actions**, giving robots a semantic interface that makes their skills programmable through natural language.

### **Key ideas**

- Combine vision encoders + language models + action heads
- Uses robot datasets paired with language captions or task instructions
- Functions as high-level semantic planners or generalist policies

### **Strengths**

- Human-friendly interface (natural language)
- Zero-shot generalization via semantic grounding
- Embodiment-agnostic (same model can work across robots)

### **Limitations**

- Lower control frequency
- Needs a low-level reflex or IL/RL layer underneath for physical agility

VLA is now distinct enough from pure IL to be its own category. -->

---

# 2️⃣ **Sim-to-Real Reinforcement Learning**

RL learns policies through **optimization**, often in simulation, then transfers them to hardware using domain randomization or skill distillation.

### **Key ideas**

- Reward-driven policy search
- Domain randomization for robustness
- MoE multi-skill RL (locomotion, manipulation, exos)
- Privileged teacher → student distillation

### **Strengths**

- Best raw performance for locomotion
- Learns dynamic, agile behaviors
- Captures complex contact physics in simulation

### **Limitations**

- Reality gap
- Reward engineering
- Struggles with high-dimensional humanoid manipulation

This paradigm continues to dominate locomotion and dynamic manipulation.

---

# 3️⃣ **World Models for Embodied Control**

World models learn **latent dynamics** so the robot can “imagine” trajectories internally, then act using planning or model predictive control.

### **Key ideas**

- Latent video models
- Predictive dynamics
- Imagination rollouts
- Model-based RL (Dreamer family)

### **Strengths**

- Superior long-horizon reasoning
- Efficient learning
- Unifies perception + prediction + action in one model

### **Limitations**

- Hard to scale to high-contact manipulation
- Complex multi-component training

World models increasingly form the backbone of generalist robot architectures.

---

# 🌐 **Comparison of the 3 Methods**

| Method             | Core Advantage                     | Main Challenge               | Best Applications                         |
| ------------------ | ---------------------------------- | ---------------------------- | ----------------------------------------- |
| **UMI IL**         | Human-like expressive motor skills | Requires massive teleop data | Loco-manipulation, daily tasks            |
| **Sim-to-Real RL** | Raw performance & agility          | Reality gap                  | Locomotion, exoskeletons, dynamic control |
| **World Models**   | Long-horizon reasoning             | Training complexity          | Planning, tool use, generalization        |

---

# 📁 **Full Library (Structured Under the Framework)**

Below, your **original tables are preserved**, but placed into the new conceptual hierarchy.

---

# ⭐ **1. My Papers**

(unchanged — as requested)

| Paper                                                                                                            | Link                                                                                             |
| ---------------------------------------------------------------------------------------------------------------- | ------------------------------------------------------------------------------------------------ |
| **Evolution of Humanoid Locomotion Control** (Science Robotics, Under Review 2025)                               | _(Not publicly released)_                                                                        |
| **A Certifiably Correct Algorithm for Generalized Robot–World & Hand–Eye Calibration** (IJRR, Under Review 2025) | [https://arxiv.org/abs/2507.23045](https://arxiv.org/abs/2507.23045)                             |
| **VibraForge** (CHI 2024)                                                                                        | [https://arxiv.org/abs/2402.16846](https://arxiv.org/abs/2402.16846)                             |
| **AeroHaptix** (RA-L 2024)                                                                                       | [https://arxiv.org/abs/2409.18009](https://arxiv.org/abs/2409.18009)                             |
| **Extrinsic Calibration of 2D mmWave Radar Pairs** (AIM 2023)                                                    | [https://doi.org/10.1109/AIM54679.2023.10196175](https://doi.org/10.1109/AIM54679.2023.10196175) |
| **Radar–Camera Spatiotemporal Calibration** (TRO 2022)                                                           | [https://arxiv.org/abs/2203.00768](https://arxiv.org/abs/2203.00768)                             |
| **Semantic + Attentive Data Mixing** (IEEE Access 2022)                                                          | [https://doi.org/10.1109/ACCESS.2022.3146381](https://doi.org/10.1109/ACCESS.2022.3146381)       |
| **Generative Design for Self-Balancing Unicycle Robot** (ACAIB 2022)                                             | [https://doi.org/10.1145/3542954.3543225](https://doi.org/10.1145/3542954.3543225)               |

---

# ⭐ **2. UMI Imitation Learning**

(Your IL/diffusion/BC-style papers go here)
→ Currently empty — you may add VideoMimic, VisualMimic, MaskedMimic, Multi-Loco IL, etc.

---

# ⭐ **3. Vision-Language-Action (VLA)**

→ Add RT-1, RT-2, PaLM-E, SayCan, OpenVLA, OmniH2O, etc.
→ (Your RL table below includes OmniH2O — but we keep it there to avoid modifying your tables.)

---

# ⭐ **4. Sim-to-Real Reinforcement Learning**

(your RL table preserved exactly)

| Paper                              | Link                                                                                                                                   |
| ---------------------------------- | -------------------------------------------------------------------------------------------------------------------------------------- |
| ADD                                | 🔗 _Unknown title_                                                                                                                     |
| ASAP                               | 🔗 _Unknown title_                                                                                                                     |
| Attention-Based Map (2025, Hutter) | 🔗 _Need full title_                                                                                                                   |
| Booster Robot RL                   | 🔗 _Need title_                                                                                                                        |
| Catch-It                           | [https://arxiv.org/abs/2302.00741](https://arxiv.org/abs/2302.00741)                                                                   |
| CORL Final                         | 🔗 _Need title_                                                                                                                        |
| DeepMimic                          | [https://arxiv.org/abs/1804.02717](https://arxiv.org/abs/1804.02717)                                                                   |
| DreamerV4                          | [https://arxiv.org/abs/2301.04104](https://arxiv.org/abs/2301.04104)                                                                   |
| DayDreamer                         | [https://arxiv.org/abs/2212.04586](https://arxiv.org/abs/2212.04586)                                                                   |
| Falcon                             | [https://arxiv.org/abs/2402.17961](https://arxiv.org/abs/2402.17961)                                                                   |
| Hover                              | [https://arxiv.org/abs/2306.14872](https://arxiv.org/abs/2306.14872)                                                                   |
| MaskedMimic                        | [https://arxiv.org/abs/2402.14289](https://arxiv.org/abs/2402.14289)                                                                   |
| Multi-Loco (Chen 2025)             | 🔗 _Need exact title_                                                                                                                  |
| OmniH2O                            | [https://arxiv.org/abs/2403.06952](https://arxiv.org/abs/2403.06952)                                                                   |
| Visual RL                          | 🔗 _Need exact title_                                                                                                                  |
| VisualMimic                        | 🔗 _Need exact title_                                                                                                                  |
| VideoMimic                         | 🔗 _Need exact title_                                                                                                                  |
| DRL Textbook                       | [https://www.andrew.cmu.edu/course/10-703/textbook/BartoSutton.pdf](https://www.andrew.cmu.edu/course/10-703/textbook/BartoSutton.pdf) |
| World Model (Ha & Schmidhuber)     | [https://arxiv.org/abs/1803.10122](https://arxiv.org/abs/1803.10122)                                                                   |

---

# ⭐ **5. World Models**

(your table preserved)

| Paper                      | Link                                                                 |
| -------------------------- | -------------------------------------------------------------------- |
| 2501.10100v4               | [https://arxiv.org/abs/2501.10100](https://arxiv.org/abs/2501.10100) |
| Science Robotics — ADT1497 | 🔗 _Link not available_                                              |

---

# ⭐ **6. Dexterous Manipulation Sim-to-Real**

(your table preserved)

| Paper   | Link                                                                 |
| ------- | -------------------------------------------------------------------- |
| DexCap  | [https://arxiv.org/abs/2309.02433](https://arxiv.org/abs/2309.02433) |
| DEX-NDM | 🔗 _Link not available_                                              |

---

# ⭐ **7. Locomotion Survey**

(your table preserved)

| Paper                                | Link                                                                 |
| ------------------------------------ | -------------------------------------------------------------------- |
| Quadrupedal & Bipedal Control Review | [https://arxiv.org/abs/2309.10072](https://arxiv.org/abs/2309.10072) |
| Sehoon Ha (2017)                     | [https://arxiv.org/abs/1707.02241](https://arxiv.org/abs/1707.02241) |
| ICRA Sim-to-Real Workshop            | 🔗 _Link not available_                                              |
| Brain Models                         | _(Not papers)_                                                       |

---

# ⭐ **8. Mixture-of-Experts (MoE)**

(your table preserved)

| Paper        | Link                                                                 |
| ------------ | -------------------------------------------------------------------- |
| Yang (2020)  | [https://arxiv.org/abs/1912.02246](https://arxiv.org/abs/1912.02246) |
| Celik (2022) | 🔗 _Link not available_                                              |
| Celik (2024) | 🔗 _Link not available_                                              |
| Huang (2025) | 🔗 _Link not available_                                              |
| Hou (2026)   | 🔗 _Link not available_                                              |

---

# ⭐ **9. Bionic Hand & Motor Control**

(your table preserved)

| Paper                 | Link                    |
| --------------------- | ----------------------- |
| Fang — eyeslight hand | 🔗 _Link not available_ |
| Peticco — DexWrist    | 🔗 _Link not available_ |
| Zhu — AIM 2019        | 🔗 _Link not available_ |

---

# ⭐ **10. Perception & State Estimation**

(your table preserved)

| Paper                   | Link                                                                 |
| ----------------------- | -------------------------------------------------------------------- |
| Stable Object Placement | [https://arxiv.org/abs/2008.07842](https://arxiv.org/abs/2008.07842) |

---

# ⭐ **11. Space Robotics**

(your table preserved)

| Paper                               | Link                                                                       |
| ----------------------------------- | -------------------------------------------------------------------------- |
| Convex Programming for Mars Landing | [https://arxiv.org/abs/2009.00950](https://arxiv.org/abs/2009.00950)       |
| 1810.08719v1                        | [https://arxiv.org/abs/1810.08719](https://arxiv.org/abs/1810.08719)       |
| SciTech 2020                        | 🔗 _Need title_                                                            |
| BMRI 2014                           | [https://doi.org/10.1155/2014/547242](https://doi.org/10.1155/2014/547242) |

---

# ⭐ **12. Survey & Overview Papers**

(your table preserved)

| Paper                                   | Link                                                                 |
| --------------------------------------- | -------------------------------------------------------------------- |
| Continuous-Time State Estimation Survey | [https://arxiv.org/abs/2302.05390](https://arxiv.org/abs/2302.05390) |

