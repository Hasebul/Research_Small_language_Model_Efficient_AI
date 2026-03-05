# Research_Small_language_Model_Efficient_AI

Welcome to the **Research Small Language Model & Efficient AI** repository. This space is dedicated to tracking, studying, and implementing the latest advancements in Small Language Models (SLMs) and computationally efficient Artificial Intelligence. 

As the AI industry shifts toward running powerful models on edge devices with lower energy and memory constraints, SLMs (typically models under 7 billion parameters) and efficient training/inference techniques (like quantization, pruning, and distillation) have become critical areas of research.

---

## 📄 Essential Reading: Recent Papers (2024–2025)

Below is a curated reading list of recent surveys, technical reports, and breakthroughs in the realm of SLMs and efficient AI.

Paper Title | Overview | Link |
| :--- | :--- | :--- |
| **HYMBA: A Hybrid-Head Architecture for Small Language Models** | A family of small language models featuring a hybrid-head parallel architecture that integrates attention mechanisms and state space models (SSMs) within the same layer, offering parallel and complementary processing of the same inputs. | [Read Paper](https://openreview.net/pdf?id=A1ztozypga) |
| **Mamba: Linear-Time Sequence Modeling with Selective State Spaces** | Introduces a hardware-aware state space model (SSM) architecture with input-dependent gating. It achieves 5× higher inference throughput than Transformers and scales linearly with sequence length. | [Read Paper](https://arxiv.org/abs/2312.00752) |
| **Transformers are SSMs: Generalized Models and Efficient Algorithms (Mamba-2)** | Connects SSMs and attention through a State Space Duality (SSD) framework. The resulting Mamba-2 architecture is 2-8× faster than the original Mamba while remaining highly competitive on language modeling. | [Read Paper](https://arxiv.org/abs/2405.21060) |
| **FlashAttention: Fast and Memory-Efficient Exact Attention
with IO-Awareness** | FlashAttention,
an IO-aware exact attention algorithm that uses tiling to reduce the number of memory reads/writes
between GPU high bandwidth memory (HBM) and GPU on-chip SRAM. | [Read Paper](https://arxiv.org/pdf/2205.14135) |
| **FlashAttention-2: Faster Attention with Better Parallelism and Work Partitioning** | An IO-aware, exact attention algorithm that dramatically speeds up training and inference by reducing memory reads/writes between GPU HBM and SRAM. Crucial for understanding modern AI hardware efficiency. | [Read Paper](https://arxiv.org/abs/2307.08691) |
| **DeepSeek-R1: Incentivizing Reasoning Capability in LLMs via Reinforcement Learning** | While R1 itself is massive, the researchers open-sourced six highly efficient dense models (1.5B to 32B parameters) distilled from it. Essential for understanding how complex reasoning is distilled into small, efficient footprints. | [Read Paper](https://arxiv.org/abs/2501.12948) |
| **Qwen2.5-VL Technical Report** | Details the architecture of the Qwen vision-language series. Highly relevant for efficient AI because it addresses diverse use cases from edge AI to high-performance computing, bringing native dynamic-resolution processing to smaller scales. | [Read Paper](https://arxiv.org/abs/2502.13923) |


### 1. Foundational Surveys and Reviews
* **State of the Art and Future Directions of Small Language Models: A Systematic Review (2025)**
    * *Overview:* A comprehensive analysis of SLM developments from 2023 to 2025, focusing on models with up to 7 billion parameters. It provides a great structural overview of current methodologies, parameter distribution, and the bimodal focus on <1B and 4B-7B models.
* **Small Language Models: Survey, Measurements, and Insights (2024)**
    * *Overview:* Surveys 70 state-of-the-art open-source SLMs (100M–5B parameters), analyzing their technical innovations across architectures, training datasets, and algorithms.

### 2. Model Architecture & Distillation
* **DeepSeek-R1: Incentivizing Reasoning Capability in LLMs via Reinforcement Learning (2025)**
    * *Overview:* While R1 itself is a massive model, the researchers open-sourced six highly efficient dense models (ranging from 1.5B to 32B parameters) distilled from DeepSeek-R1. Reading this paper is crucial for understanding how complex reasoning capabilities from massive models are successfully distilled into small, efficient footprints.
* **Qwen2.5-VL Technical Report (2025)**
    * *Overview:* Details the architecture of the Qwen vision-language series. It is highly relevant for efficient AI because it addresses diverse use cases from edge AI to high-performance computing, bringing native dynamic-resolution processing to smaller scales.

### 3. Application & Task-Specific Efficiency

* **Small Language Models for Efficient Agentic Tool Calling: Outperforming Large Models with Targeted Fine-tuning (2025)**
    * *Overview:* Investigates replacing LLM-driven workflows with optimized SLMs. Demonstrates how a domain-adapted SLM with just 350M parameters can achieve exceptional performance on tool-calling evaluations, significantly lowering infrastructure overhead.
* **Evaluating Small Language Models for News Summarization: Implications and Factors Influencing Performance (2025)**
    * *Overview:* Explores the capability of SLMs for real-time edge-device summarization. It highlights how instruction-tuning impacts SLMs compared to their larger counterparts in resource-constrained environments.

---

## 🔬 Prominent Research Groups in Efficient AI

If you are looking for labs to follow, collaborate with, or draw inspiration from, these groups are currently at the forefront of Efficient AI and SLM research:

| Affiliation | PI / Lab | Link |
| :--- | :--- | :--- |
| **Princeton University** | Tri Dao | [https://tridao.me/](https://tridao.me/) |
| **MIT & NVIDIA** | Song Han *(Han Lab)* | [https://hanlab.mit.edu/](https://hanlab.mit.edu/) |
| **Yale University / USC** | Priyadarshini Panda *(Intelligent Computing Lab)* | [https://intelligentcomputinglab.yale.edu/](https://intelligentcomputinglab.yale.edu/) |
| **Georgia Tech** | Yingyan (Celine) Lin *(EIC Lab)* | [https://eiclab.net/](https://eiclab.net/) |
| **Microsoft Research** | Efficient AI Group | [https://www.microsoft.com/en-us/research/](https://www.microsoft.com/en-us/research/) |

* **Efficient AI Team (NVIDIA & MIT)**
    * *Focus:* A collaboration dedicated to GPU-accelerated efficient AI computing. They focus on hardware-aware optimization, quantization-enhanced reinforcement learning (QeRL), and long-video generation with real-time autoregressive frameworks. 
* **Efficient AI Group (Microsoft Research)**
    * *Focus:* Reimagining AI efficiency from GPU kernels to context engineering. They work on making AI smarter and leaner by engineering "context paths" that minimize redundancy, and designing GPU kernels to maximize throughput for LLM workloads.
* **Intelligent Computing Lab (Yale University / USC)**
    * *Led by:* Prof. Priyadarshini Panda
    * *Focus:* Biologically inspired algorithm and hardware co-design. They are responsible for breakthroughs in neuromorphic computing, algorithm-hardware co-design, and extreme quantization methods (like GPTAQ for asymmetric calibration).
* **Trusted and Efficient AI (TEA) Lab (University of British Columbia)**
    * *Focus:* Improving the explainability, fairness, privacy, and efficiency of AI models. They actively research collaborative learning via textual gradients on LLMs and federated learning paradigms.
* **EIC Lab (Georgia Tech)**
    * *Focus:* Developing efficient machine learning techniques via cross-layer innovations. Their work spans from AI algorithms down to AI hardware accelerators and chip design, fostering "green AI."
* **Catalyst Group (Carnegie Mellon University)**
    * *Focus:* An interdisciplinary machine learning and systems research group exploring the frontiers of specialized LLMs, edge computing, and AI-driven automated learning systems to dramatically reduce the energy needs of AI models.

---

## 🤝 Contributing

Contributions are welcome! If you know of a recent paper (2024 or newer) or a research lab doing incredible work in the Efficient AI space, please open a pull request or submit an issue to have it added to this repository.
