# Research Paper Library

A curated collection of seminal and recent papers in trustworthy machine learning. Papers are organized by topic and include our commentary on significance and practical implications.

!!! tip "Search & Filter"
    Use `Ctrl+F` to search for specific topics, authors, or venues. Papers are tagged with key concepts for easy discovery.

## Foundational Papers

### Fairness & Bias

**Seminal Works**

- **[Fairness Through Awareness](https://arxiv.org/abs/1104.3913)** (Dwork et al., 2012)  
  *ITCS 2012* | `individual-fairness` `awareness`  
  Introduces the concept of individual fairness and awareness in algorithmic decision-making.

- **[Equality of Opportunity in Supervised Learning](https://arxiv.org/abs/1610.02413)** (Hardt et al., 2016)  
  *NIPS 2016* | `group-fairness` `equalized-odds`  
  Defines equalized odds and equality of opportunity for binary classification.

- **[Fairness Definitions Explained](https://arxiv.org/abs/1710.03184)** (Verma & Rubin, 2018)  
  *IEEE FATES 2018* | `survey` `fairness-metrics`  
  Comprehensive survey of 20+ fairness definitions with mathematical formulations.

**Recent Advances**

- **[Fairness-Aware Machine Learning: Practical Challenges and Lessons Learned](https://dl.acm.org/doi/10.1145/3336191.3371878)** (Bellamy et al., 2019)  
  *WSDM 2019* | `aif360` `toolkit` `industry`  
  Practical insights from deploying fairness-aware ML in enterprise settings.

- **[Intersectional Fairness: A Fractal Approach](https://arxiv.org/abs/2206.03881)** (Foulds et al., 2020)  
  *FAccT 2020* | `intersectionality` `subgroup-fairness`  
  Novel approach to handling fairness across intersecting protected attributes.

### Robustness & Adversarial ML

**Foundational**

- **[Intriguing Properties of Neural Networks](https://arxiv.org/abs/1312.6199)** (Szegedy et al., 2013)  
  *ICLR 2014* | `adversarial-examples` `discovery`  
  First systematic study of adversarial examples in deep neural networks.

- **[Explaining and Harnessing Adversarial Examples](https://arxiv.org/abs/1412.6572)** (Goodfellow et al., 2014)  
  *ICLR 2015* | `fgsm` `linear-hypothesis`  
  Introduces FGSM attack and linear hypothesis for adversarial vulnerability.

- **[Towards Deep Learning Models Resistant to Adversarial Attacks](https://arxiv.org/abs/1706.06083)** (Madry et al., 2017)  
  *ICLR 2018* | `pgd` `adversarial-training`  
  Establishes PGD as the gold standard for adversarial training evaluation.

**Certified Defenses**

- **[Certified Adversarial Robustness via Randomized Smoothing](https://arxiv.org/abs/1902.02918)** (Cohen et al., 2019)  
  *ICML 2019* | `certified-defense` `randomized-smoothing`  
  Scalable approach to obtaining robustness certificates using Gaussian noise.

- **[Provably Robust Deep Learning via Adversarially Trained Smoothed Classifiers](https://arxiv.org/abs/1906.04584)** (Salman et al., 2019)  
  *NeurIPS 2019* | `certified-training` `smoothing`  
  Combines adversarial training with randomized smoothing for stronger guarantees.

### Interpretability & Explainability

**Core Methods**

- **["Why Should I Trust You?": Explaining the Predictions of Any Classifier](https://arxiv.org/abs/1602.04938)** (Ribeiro et al., 2016)  
  *KDD 2016* | `lime` `local-explanations`  
  Introduces LIME for locally interpretable model-agnostic explanations.

- **[A Unified Approach to Interpreting Model Predictions](https://arxiv.org/abs/1705.07874)** (Lundberg & Lee, 2017)  
  *NIPS 2017* | `shap` `shapley-values`  
  SHAP: Unified framework based on cooperative game theory.

- **[Attention is All You Need](https://arxiv.org/abs/1706.03762)** (Vaswani et al., 2017)  
  *NIPS 2017* | `attention` `transformers` `interpretability`  
  While primarily an architecture paper, attention mechanisms provide built-in interpretability.

**Evaluation & Benchmarking**

- **[Evaluating the Visualization of What a Deep Neural Network Has Learned](https://arxiv.org/abs/1509.06321)** (Simonyan et al., 2013)  
  *ICLR 2014* | `saliency-maps` `evaluation`  
  Early work on evaluating explanation quality through perturbation analysis.

- **[Sanity Checks for Saliency Maps](https://arxiv.org/abs/1810.03292)** (Adebayo et al., 2018)  
  *NeurIPS 2018* | `sanity-checks` `saliency-evaluation`  
  Demonstrates that many explanation methods fail basic sanity checks.

### Privacy-Preserving ML

**Differential Privacy**

- **[Deep Learning with Differential Privacy](https://arxiv.org/abs/1607.00133)** (Abadi et al., 2016)  
  *CCS 2016* | `differential-privacy` `sgd` `deep-learning`  
  First practical application of differential privacy to deep learning training.

- **[The Algorithmic Foundations of Differential Privacy](https://www.cis.upenn.edu/~aaroth/Papers/privacybook.pdf)** (Dwork & Roth, 2014)  
  *Foundations and Trends* | `dp-foundations` `survey`  
  Comprehensive theoretical foundation of differential privacy.

**Federated Learning**

- **[Communication-Efficient Learning of Deep Networks from Decentralized Data](https://arxiv.org/abs/1602.05629)** (McMahan et al., 2017)  
  *AISTATS 2017* | `federated-learning` `fedavg`  
  Introduces federated learning and the FedAvg algorithm.

- **[Towards Federated Learning at Scale: System Design](https://arxiv.org/abs/1902.01046)** (Bonawitz et al., 2019)  
  *MLSys 2019* | `federated-systems` `scale`  
  System design considerations for large-scale federated learning deployment.

## Recent Research (2023-2024)

### Emerging Topics

- **[Constitutional AI: Harmlessness from AI Feedback](https://arxiv.org/abs/2212.08073)** (Bai et al., 2022)  
  *Anthropic* | `constitutional-ai` `alignment` `safety`  
  Novel approach to AI alignment using constitutional principles and AI feedback.

- **[Red Teaming Language Models with Language Models](https://arxiv.org/abs/2202.03286)** (Perez et al., 2022)  
  *EMNLP 2022* | `red-teaming` `llm-safety` `automated-testing`  
  Automated red teaming approach for identifying harmful LLM behaviors.

- **[Training a Helpful and Harmless Assistant with Reinforcement Learning from Human Feedback](https://arxiv.org/abs/2204.05862)** (Bai et al., 2022)  
  *Anthropic* | `rlhf` `helpfulness` `harmlessness`  
  Balancing helpfulness and harmlessness in conversational AI systems.

### Benchmark Papers

- **[BOLD: Dataset and Metrics for Measuring Biases in Open-Ended Language Generation](https://arxiv.org/abs/2101.11718)** (Dhamala et al., 2021)  
  *FAccT 2021* | `bias-benchmarks` `language-generation`  
  Comprehensive benchmark for measuring bias in text generation models.

- **[RobustBench: a Standardized Adversarial Robustness Benchmark](https://arxiv.org/abs/2010.09670)** (Croce et al., 2020)  
  *NeurIPS 2021* | `robustness-benchmark` `evaluation`  
  Standardized benchmark and leaderboard for adversarial robustness evaluation.

## Paper Collections by Venue

### Top-Tier Conferences

=== "FAccT (Fairness, Accountability, Transparency)"
    - [FAccT 2024](https://facctconference.org/2024/) - Latest fairness and accountability research
    - [FAccT 2023](https://facctconference.org/2023/) - Includes algorithmic auditing advances
    - [FAccT 2022](https://facctconference.org/2022/) - Focus on intersectionality and bias

=== "ICML/NeurIPS"
    - Focus on theoretical foundations and scalable algorithms
    - Strong representation in robustness and privacy research
    - Recent emphasis on LLM safety and alignment

=== "ICLR"
    - Cutting-edge deep learning approaches to trustworthy ML
    - Novel architectures for interpretable models
    - Adversarial robustness innovations

### Specialized Venues

- **AIES** (AI, Ethics, and Society): Interdisciplinary perspectives
- **S&P, CCS, USENIX Security**: Security and privacy focus  
- **CHI, CSCW**: Human-computer interaction and social impacts
- **AAAI**: Broad AI applications and theoretical work

## Reading Lists by Course Module

### For Assignment 1: Bias Detection
1. Verma & Rubin (2018) - Fairness definitions overview
2. Bellamy et al. (2019) - Practical fairness toolkit usage
3. Choose one: Group fairness vs. individual fairness comparison

### For Assignment 2: Adversarial Robustness  
1. Goodfellow et al. (2014) - FGSM and basic concepts
2. Madry et al. (2017) - PGD and evaluation methodology
3. Cohen et al. (2019) - Certified defenses introduction

### For Midterm Preparation
Core papers from each topic area marked with ⭐ in the full bibliography.

---

!!! note "Contributing"
    Found an important paper we missed? [Submit a suggestion](https://github.com/trustworthyml-ai/trustworthyml-ai/issues) to help keep this library comprehensive and current.

*Last updated: {{ git_revision_date }}*