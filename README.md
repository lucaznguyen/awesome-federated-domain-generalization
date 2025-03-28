# Awesome Federated Domain Generalization (FedDG)

This repository is a collection of awesome things about federated domain generalization, including papers, code, etc.

## What is Federated Domain Generalization?

Federated Learning (FL) enables collaborative model training on decentralized data residing on client devices (e.g., hospitals, mobile phones) without sharing the raw data, thus preserving privacy. Domain Generalization (DG) focuses on training a model from multiple observed source domains such that it generalizes effectively to unseen target domains, addressing the challenge of domain shift. **Federated Domain Generalization (FedDG)** combines these paradigms. It tackles the problem of learning a *generalizable* model across decentralized clients, where each client (or group of clients) may represent a distinct *domain*. The goal is to train a model under federated constraints (privacy, communication bottlenecks, systems heterogeneity) that performs well not only on participating client domains but critically, on *new, unseen domains* (and potentially unseen clients) encountered after deployment.

**Key Challenges & Differences:**
* **Compared to Standard FL:** FedDG explicitly addresses the *domain shift* aspect present across clients and aims for generalization to *entirely unseen domains*, going beyond typical non-IID settings in FL that often focus on statistical heterogeneity within a common task space.
* **Compared to Standard DG:** FedDG operates under the constraints of FL – data is decentralized, cannot be pooled, and communication is often limited. Centralized DG algorithms are often not directly applicable.
* **Compared to Federated Domain Adaptation (FedDA):** FedDA usually assumes the target domain(s) are known during the adaptation phase, and sometimes unlabeled (or even limited labeled) target data is available. FDG aims for generalization *without* access to target domain data during training.

FedDG is crucial for applications where models are deployed in diverse environments unseen during training, such as medical diagnosis across different hospitals/scanners, autonomous driving in varying weather/locations, and financial modeling across disparate markets.

## Other Awesome Related Repos

Awesome Federated Machine Learning [[github](https://github.com/innovation-cat/Awesome-Federated-Machine-Learning)]

Awesome Domain Generalization [[github](https://github.com/junkunyuan/Awesome-Domain-Generalization)]

OOD Machine Learning: Detection, Robustness, and Generalization [[github](https://github.com/huytransformer/Awesome-Out-Of-Distribution-Detection)]

## Benchmarks

DomainBed [[github](https://github.com/facebookresearch/DomainBed)]

Federated Domain Generalization Benchmark [[paper](https://openreview.net/forum?id=wprSv7ichW)][[github](https://github.com/inouye-lab/FedDG_Benchmark)]

## Survey

Federated Domain Generalization: A Survey (**arXiv 2024**)  [[paper](https://arxiv.org/abs/2306.01334)]

Federated Learning for Generalization, Robustness, Fairness: A Survey and Benchmark (**TPAMI 2024**) [[paper](https://arxiv.org/abs/2311.06750)]

## Papers

### 2025
FedDAG: Federated Domain Adversarial Generation Towards Generalizable Medical Image Analysis (**arXiv 2025**) [[paper](https://arxiv.org/abs/2501.13967)]

FedTG: Text-guided Federated Domain Generalization (**ICASSP 2025**) [[paper](https://doi.org/10.1109/ICASSP49660.2025.10888120)]

Frequency-Based Federated Domain Generalization for Polyp Segmentation (**ICASSP 2025**) [[paper](https://doi.org/10.1109/ICASSP49660.2025.10889662)] [[code](https://github.com/nubagcilab/icassp2025-fdgpolyp)]

Federated Domain Generalization with Label Smoothing and Balanced Decentralized Training (**ICASSP 2025**) [[paper](https://doi.org/10.1109/ICASSP49660.2025.10888230)] [[code](https://github.com/AhmedMostafaSoliman/FedPartWhole)]

Fedpartwhole: federated domain generalization via consistent part-whole hierarchies (**PAA 2025**) [[paper](https://doi.org/10.1007/s10044-025-01439-4)] [[code](https://github.com/AhmedMostafaSoliman/FedPartWhole)]

Federated Domain Generalization for Fault Diagnosis: Cross-Client Style Integration and Dual Alignment Representation (**IEEE IoT-J 2025**) [[paper](https://doi.org/10.1109/JIOT.2025.3551339)]

Federated Self-supervised Domain Generalization for Label-efficient Polyp Segmentation (**arXiv 2025**) [[paper](https://arxiv.org/abs/2502.07951)]

FedAlign: Federated Domain Generalization with Cross-Client Feature Alignment (**arXiv 2025**) [[paper](https://arxiv.org/abs/2501.15486)]

Federated Domain Generalization with Data-free On-server Gradient Matching (**arXiv 2025**) [[paper](https://arxiv.org/abs/2501.14653)] [[code](https://github.com/skydvn/FedOMG)]

Heterogeneous Federated Learning: Client-Side Collaborative Update Interdomain Generalization Method for Intelligent Fault Diagnosis (**IEEE IoT-J 2025**) [[paper](https://doi.org/10.1109/JIOT.2024.3489617)]

A unified Personalized Federated Learning framework ensuring Domain Generalization (**Expert Systems with Applications 2025**) [[paper](https://doi.org/10.1016/j.eswa.2024.125700)]

### 2024

Decentralized federated domain generalization with cluster alignment for fault diagnosis (**Control Engineering Practice 2024**) [[paper](https://doi.org/10.1016/j.conengprac.2024.105951)]

A unified Personalized Federated Learning framework for improving performance on Non-IID data via domain generalization (**ESWA 2024**) [[paper](https://doi.org/10.1016/j.eswa.2024.125700)]

Federated Domain Generalization via Prompt Learning and Aggregation (**arXiv 2024**) [[paper](https://arxiv.org/pdf/2411.10063)] [[code](https://github.com/GongShuai8210/PLAN)]

FISC: Federated Domain Generalization via Interpolative Style Transfer and Contrastive Learning (**arXiv 2024**) [[paper](https://arxiv.org/abs/2410.22622)]

FedCCRL: Federated Domain Generalization with Cross-Client Representation Learning (**arXiv 2024**) [[paper](https://arxiv.org/abs/2410.11267)] [[code](https://github.com/sanphouwang/fedccrl)]

FedGCA: Global Consistent Augmentation Based Single-Source Federated Domain Generalization (**arXiv 2024**) [[paper](https://arxiv.org/abs/2409.14671)]

Boosting Federated Domain Generalization: Understanding the Role of Advanced Pre-Trained Architectures (**arXiv 2024**) [[paper](https://arxiv.org/abs/2409.13527)]

Reducing Spurious Correlation for Federated Domain Generalization (**arXiv 2024**) [[paper](https://arxiv.org/abs/2407.19174)]

Feature Diversification and Adaptation for Federated Domain Generalization (**arXiv 2024**) [[paper](https://arxiv.org/abs/2407.08245)]

Federated Unsupervised Domain Generalization using Global and Local Alignment of Gradients (**arXiv 2024**) [[paper](https://arxiv.org/abs/2405.16304)] [[code](https://github.com/mahdiyarmm/fedgala)]

Efficiently Assemble Normalization Layers and Regularization for Federated Domain Generalization (**CVPR 2024**) [[paper](https://openaccess.thecvf.com/content/CVPR2024/html/Le_Efficiently_Assemble_Normalization_Layers_and_Regularization_for_Federated_Domain_Generalization_CVPR_2024_paper.html)] [[code](https://github.com/lhkhiem28/gPerXAN)]

DiPrompT: Disentangled Prompt Tuning for Multiple Latent Domain Generalization in Federated Learning (**CVPR 2024**) [[paper](https://openaccess.thecvf.com/content/CVPR2024/html/Bai_DiPrompT_Disentangled_Prompt_Tuning_for_Multiple_Latent_Domain_Generalization_in_CVPR_2024_paper.html)]

Hypernetwork-Driven Model Fusion for Federated Domain Generalization (**arXiv 2024**) [[paper](https://arxiv.org/abs/2402.06974)]

Multi-Source Collaborative Gradient Discrepancy Minimization for Federated Domain Generalization (**AIII 2024**) [[paper](https://doi.org/10.1609/aaai.v38i14.29510)]

Bilateral Proxy Federated Domain Generalization for Privacy-preserving Medical Image Diagnosis (**IEEE J-BHI 2024**) [[paper](https://doi.org/10.1109/JBHI.2024.3456440)]

Federated Adversarial Domain Hallucination for Privacy-Preserving Domain Generalization (**IEEE TMM 2023**) [[paper](https://doi.org/10.1109/tmm.2023.3257566)]

Federated Analytics With Data Augmentation in Domain Generalization Toward Future Networks (**IEEE TMLCN 2024**) [[paper](https://doi.org/10.1109/TMLCN.2024.3393892)]

Federated learning via reweighting information bottleneck with domain generalization (**Information Sciences 2024**) [[paper](https://doi.org/10.1016/j.ins.2024.120825)]

Heterogeneous Federated Domain Generalization Network With Common Representation Learning for Cross-Load Machinery Fault Diagnosis (**IEEE TSMCS 2024**) [[paper](https://doi.org/10.1109/TSMC.2024.3408058)]

Non-linear Fusion in Federated Learning: A Hypernetwork Approach to Federated Domain Generalization (**arXiv 2024**) [[paper](https://arxiv.org/abs/2402.06974)]

### 2023

Enhancing domain generalization in the AI-based analysis of chest radiographs with federated learning (**Scientific Reports 2023**) [[paper](https://doi.org/10.1038/s41598-023-49956-8)]

StableFDG: Style and Attention Based Learning for Federated Domain Generalization (**NeurIPS/arXiv 2023**) [[paper](https://proceedings.neurips.cc/paper_files/paper/2023/file/dae8bdacd265399b193e6b43d44a80f0-Paper-Conference.pdf)]

Mind the Gap: Federated Learning Broadens Domain Generalization in Diagnostic AI Models (**Sci Rep/arXiv 2023**) [[paper](https://doi.org/10.1038/s41598-023-49956-8)]

Benchmarking Algorithms for Federated Domain Generalization (**arXiv/ICLR Submission 2023**) [[paper](https://arxiv.org/abs/2307.05238)]

MLA-BIN: Model-level Attention and Batch-instance Style Normalization for Domain Generalization of Federated Learning on Medical Image Segmentation (**arXiv 2023**) [[paper](https://arxiv.org/abs/2306.16747)]

Federated Domain Generalization: A Survey (**arXiv 2023**) [[paper](https://arxiv.org/abs/2306.01334)]

Collaborative Semantic Aggregation and Calibration for Federated Domain Generalization (**IEEE TKDE 2023**) [[paper](https://doi.org/10.1109/TKDE.2023.3273882)]

Domain Generalization for Foreground Segmentation Using Federated Learning (**ISVC 2023**) [[paper](https://doi.org/10.1007/978-3-031-47969-4_20)]

Federated Condition Generalization on Low-dose CT Reconstruction via Cross-domain Learning (**MICCAI 2023**) [[paper](https://doi.org/10.1007/978-3-031-43898-1_5)]

Federated Learning for IoT Devices With Domain Generalization (**IEEE Internet of Things Journal 2023**) [[paper](https://doi.org/10.1109/JIOT.2022.3173489)]

### 2022

FedSR: A Simple and Effective Domain GeneralizationMethod for Federated Learning (**NeurIPS 2022**) [[paper](https://proceedings.neurips.cc/paper_files/paper/2022/file/fd946a6c99541fddc3d64a3ea39a1bc2-Paper-Conference.pdf)] [[code](https://github.com/atuannguyen/FedSR)]

FL Games: A federated learning framework for distribution shifts (**FL-NeurIPS 2022**) [[paper](https://arxiv.org/pdf/2205.11101)] 

Feature Distribution Matching for Federated DomainGeneralization (**ACML 2022**) [[paper](https://proceedings.mlr.press/v189/sun23a/sun23a.pdf)] [[code](https://github.com/yuweisunn/federated-knowledge-alignment)]

Generalized Federated Learning via Sharpness Aware Minimization (**PMLR 2022**) [[paper](https://proceedings.mlr.press/v162/qu22a/qu22a.pdf)]

Improving Generalization in Federated Learning by Seeking Flat Minima (**ECCV 2022**) [[paper](https://www.ecva.net/papers/eccv_2022/papers_ECCV/papers/136830636.pdf)] [[code](https://github.com/debcaldarola/fedsam)]

### 2021

FedDG: Federated Domain Generalization on Medical Image Segmentation via Episodic Learning in Continuous Frequency Space (**CVPR 2021**) [[paper](https://openaccess.thecvf.com/content/CVPR2021/papers/Liu_FedDG_Federated_Domain_Generalization_on_Medical_Image_Segmentation_via_Episodic_CVPR_2021_paper.pdf)] [[code](https://github.com/liuquande/FedDG-ELCFS)]

Collaborative optimization and aggregation for decentralized domain generalization and adaptation (**ICCV 2021**) [[paper](https://openaccess.thecvf.com/content/ICCV2021/papers/Wu_Collaborative_Optimization_and_Aggregation_for_Decentralized_Domain_Generalization_and_Adaptation_ICCV_2021_paper.pdf)]

Federated learning with domain generalization (**arXiv 2021**) [[paper](https://arxiv.org/pdf/2111.10487)] [[code](https://github.com/Haoxiang-Wang/FedADG)]
