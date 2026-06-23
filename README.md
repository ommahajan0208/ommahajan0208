<div align="center">

# Om Mahajan

**AI & Data Science · PICT, Pune**

[![Email](https://img.shields.io/badge/Email-ommahajan0208%40gmail.com-0a0a0a?style=flat-square&logo=gmail&logoColor=white)](mailto:ommahajan0208@gmail.com)
[![LinkedIn](https://img.shields.io/badge/LinkedIn-om--mahajan-0a0a0a?style=flat-square&logo=linkedin&logoColor=white)](https://www.linkedin.com/in/om-mahajan-1092b232a/)
[![LeetCode](https://img.shields.io/badge/LeetCode-ommahajan0208-0a0a0a?style=flat-square&logo=leetcode&logoColor=white)](https://leetcode.com/u/ommahajan0208/)
[![Kaggle](https://img.shields.io/badge/Kaggle-ommahajan0208-0a0a0a?style=flat-square&logo=kaggle&logoColor=white)](https://www.kaggle.com/ommahajan0208)

</div>

---

## About

I'm an AI & Data Science undergraduate at PICT, building systems that sit at the intersection of research and engineering. My work spans two axes - experimental ML research (cognitive memory architectures, biosignal classification, quantitative strategy modeling) and production-grade agentic systems (multi-agent orchestration, RAG pipelines, LLM workflows).

I design end-to-end, from hypothesis and experimentation to orchestration, deployment, and inference, with a strong emphasis on making things robust, traceable, and production-ready.

In practice, that means a biologically-inspired LLM agent memory system with multiplicative retrieval scoring and an online RL bandit, a multi-agent insurance claims processor with consensus-based fraud detection, a critical-level open-source contribution extending a physics-informed classifier to 6-class EEG sleep staging, and a boosting ensemble placing 3rd with macro-F1 0.9424. CGPA 9.35/10, top 10% of batch. Grades are the floor, not the ceiling.

---

## Projects

### Research

#### [Decay Lab: Biologically-Inspired LLM Agent Memory](https://github.com/ommahajan0208/Decay_Lab)
`Python` `Flask` `Sentence-BERT` `Cross-Encoder` `HLR` `Contextual Bandit` 

Experimental framework modeling AI agent memory as a time-decaying, reinforcement-learning-tuned retrieval system. Implements a weighted ensemble of three cognitive decay models (Half-Life Regression, Power-Law, Reinforcement) with **multiplicative relevance-strength scoring** that eliminates retrieval noise from stale-but-strong memories regardless of their age. 2-stage neural retrieval pipeline with Bi-Encoder candidate selection followed by Cross-Encoder re-ranking. Online Softmax Contextual Bandit adapts decay weights in real-time from user thumbs-up/thumbs-down feedback. Three Brain Profiles (Smart, Dumb, Adaptive) control retention behavior, with sleep consolidation and interference decay mechanics. Flask REST API, web dashboard with Chart.js decay curve visualization, Student spaced-repetition simulation, and a full evaluation harness (Precision, Recall, MRR, MAP).

---

#### [HRF Multi-Class EEG Sleep Staging](https://github.com/Devanik21/Harmonic-Resonance-Forest/pull/61)
`Python` `NumPy` `SciPy` `Scikit-learn` `MNE` `XGBoost` `imbalanced-learn` · *GSSoC 2026 · PR #61 · Level: Critical*

Extended Harmonic Resonance Forest (HRF) v15.0 from binary to 6-class polysomnography sleep staging (W, N1, N2, N3, N4, REM) on Sleep-EDF PhysioNet. Added `class_freq_map` anchoring each class to its dominant EEG rhythm (Delta->N3/N4, Theta->N1, Sigma->N2, Alpha->Wake/REM). Engineered 32 neurophysiological features (band powers, Hjorth parameters, spectral entropy, spindle density, slow-wave duration, theta/delta and alpha/theta ratios). Leakage-free two-stage class balancing (undersample Wake, SMOTE minorities). Benchmarked HRF 80.14% vs RF 92.12%, XGBoost 92.72%, SVM 88.29% with 5-fold stratified cross-validation and Cohen's kappa.

---

#### [Inferenc26: International AI Competition](https://github.com/ommahajan0208/Inferenc26)
`Python` `Scikit-learn` `NumPy` `Optimization` · *17th Place Globally · Score: 2202.96*

Ranked 17th globally in the Inferenc26 international AI competition. Built simulation engines and systematic optimization pipelines with robust strategy search under adversarial conditions. Applied quantitative reasoning techniques including Kelly criterion-based sizing and market-making strategy design under adverse selection, combining stochastic modeling with empirical hyperparameter optimization to maximize score across competition scenarios.

---

### Production Systems

#### [Claimiyo: Intelligent Insurance Claims Processing System](https://github.com/ommahajan0208/Claimiyo)
`LangGraph` `LangChain` `FastAPI` `YOLOv8` `HuggingFace` `Python`

Multi-stage agentic pipeline with 4 specialised nodes (Planner, Executor, Verifier, Output Validator). Consensus-based fraud detection via 3 parallel LLM reviewers and a verifier aggregation layer, delivering deterministic approval/rejection with confidence scoring and full reasoning transparency. YOLOv8 damage detection (Minor/Moderate/Severe), Tesseract OCR, AI-generated image fraud detection, ICD-10/CPT medical code validation, and a dual-versioned FastAPI backend with Pydantic validation.

---

#### [CortexReach: Offline LLM Cold Outreach Engine](https://github.com/ommahajan0208/CortexReach)
`Python` `Ollama` `LLaMA3` `Rich TUI` `Prompt Engineering`

Offline LLM-powered CLI engine generating hyper-personalized cold outreach across 5 channels (Email, WhatsApp, SMS, LinkedIn, Instagram) from multi-source prospect data. 8-layer modular architecture (input, analysis, context, generation, optimization, validation, storage, visualization) with persona analysis, hook extraction, and company context reuse across same-company prospects. Two-pass generation pipeline, channel-optimized generation followed by persona-typed critic optimization (4 styles - technical, executive, casual, formal). Anti-hallucination enforcement via prompt-level rules and regex post-processing prevents invented facts. Privacy and ethics validation layers screen all output. Zero cloud cost, fully offline via Ollama.

---

### Competition / Hackathon

#### [AIloyance: AI-Powered Life Cycle Assessment Platform](https://github.com/LCAlloyance/ml_Alloyance)
`XGBoost` `LangChain` `ChromaDB` `HuggingFace` `FastAPI` `Python` · *Qualified for Stage 2, Smart India Hackathon 2025*

5 specialised XGBoost regression models predicting circularity KPIs (Recycled Content, Resource Efficiency, Recovery Rate, Reuse Potential, Extended Product Life) across 40+ engineered features. MICE imputation with XGBoost and Random Forest estimators for robust missing-data handling. Multi-LLM RAG pipeline (Gemini 2.0 Flash / Mistral Nemo) generating 6-section evidence-based sustainability reports. 25,000-sample domain dataset with Scope 1-3 emissions modelling.

---

#### [DataQuest: Air Quality Index Prediction](https://github.com/ommahajan0208/DataQuest25)
`XGBoost` `LightGBM` `CatBoost` `Optuna` `Scikit-learn` · *3rd Place, DataQuest '25, Pulzion ACM PICT*

Macro-F1 of **0.9424** on a 3-class AQI classification (Good/Moderate/Poor) via Optuna-tuned weighted soft voting and OOF stacking, surpassing the competition baseline of 0.9260. 30+ engineered meteorological interaction features (temperature-dew point differentials, wind gust ratios, cyclic sine-cosine wind encoding) with systematic Optuna hyperparameter optimisation with early-stopping across all three boosting frameworks.

---

## Achievements

| Competition | Result |
|---|---|
| DataQuest '25, Pulzion ACM PICT | **3rd Place** · Macro-F1: 0.9424 |
| Inferenc26 International AI Competition | **17th Place** · Score: 2202.96 |
| Credenz 2026 Xodia Challenge (PISB) | **9th Place** · Deep Q-Network RL agents |
| TechRush '25, Solar Energy Prediction | **99.98% Accuracy** |
| GSSoC 2026, PR #61 | Critical-level merge · Praised by repo owner |

---

## Tech Stack

**Languages**
`Python` `Java` `C++` `C` `SQL`

**ML / DL**
`Scikit-learn` `PyTorch` `XGBoost` `LightGBM` `CatBoost` `Random Forest` `YOLOv8`

**LLM & Agentic AI**
`LangChain` `LangGraph` `Ollama` `OpenRouter` `HuggingFace Transformers` `Sentence Transformers` `ChromaDB`

**Data & Visualisation**
`Pandas` `NumPy` `Matplotlib` `Seaborn` `Optuna` `MICE Imputation`

**Backend & Deployment**
`FastAPI` `Flask` `Docker` `GitHub` `Pydantic`

---

## Beyond the Code

- **Advisory Team**, Google ELP Pune Community, contributing to developer community strategy and student engagement
- **ML Workshop Mentor**, designed and delivered 3 hands-on workshops for 50+ undergraduate students
- **AI Literacy Educator**, PICT Model School, 6 sessions on ML and AI fundamentals for 3rd-5th grade students
- **Core Member**, Computer Society of India (CSI), PICT

---

## Courses / Certifications

#### [Machine Learning Specialization](https://www.coursera.org/specializations/machine-learning-introduction) · *DeepLearning.AI, Coursera*
`Supervised Learning` `Unsupervised Learning` `Reinforcement Learning` `Neural Networks` `Decision Trees`

3-course series by Andrew Ng covering supervised learning (linear/logistic regression, SVMs, decision trees, ensemble methods), unsupervised learning (clustering, anomaly detection, recommender systems), and an introduction to reinforcement learning. Emphasis on practical implementation and intuition behind core ML algorithms.

[![Credential](https://img.shields.io/badge/Credential-View%20Certificate-0a0a0a?style=flat-square&logo=coursera&logoColor=white)](#)

---

#### [Deep Learning Specialization](https://www.coursera.org/specializations/deep-learning) · *DeepLearning.AI, Coursera*
`Neural Networks` `CNNs` `RNNs` `LSTMs` `Transformers` `Batch Normalization` `Dropout` `Adam`

5-course series by Andrew Ng covering the full deep learning stack, neural network foundations, hyperparameter tuning and regularization, structuring ML projects, convolutional networks (CNNs for image recognition and detection), and sequence models (RNNs, LSTMs, GRUs, attention mechanisms, Transformers). Applied across computer vision, NLP, and speech recognition tasks.

[![Credential](https://img.shields.io/badge/Credential-View%20Certificate-0a0a0a?style=flat-square&logo=coursera&logoColor=white)](#)

---

<div align="center">

*"Patience and persistence is the key to success."*

![Profile Views](https://komarev.com/ghpvc/?username=ommahajan0208&style=flat-square&color=555555)

</div>
