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

## Survey

Federated Domain Generalization: A Survey (**arXiv 2024**)  [[paper](https://arxiv.org/abs/2306.01334)]
Federated Learning for Generalization, Robustness, Fairness: A Survey and Benchmark (**TPAMI 2024**) [[paper](https://arxiv.org/abs/2311.06750)]

## Papers

### 2024

PLAN: Federated Domain Generalization via Prompt Learning and Aggregation (**arXiv 2024**) [[paper](https://arxiv.org/pdf/2411.10063)] [[code](https://github.com/GongShuai8210/PLAN)]

DiPrompT: Disentangled Prompt Tuning for Multiple Latent Domain Generalization in Federated Learning (**CVPR 2024**) [[paper](https://openaccess.thecvf.com/content/CVPR2024/papers/Bai_DiPrompT_Disentangled_Prompt_Tuning_for_Multiple_Latent_Domain_Generalization_in_CVPR_2024_paper.pdf)]

Efficiently Assemble Normalization Layers and Regularization for Federated Domain Generalization (**CVPR 2024**) [[paper](https://openaccess.thecvf.com/content/CVPR2024/papers/Le_Efficiently_Assemble_Normalization_Layers_and_Regularization_for_Federated_Domain_Generalization_CVPR_2024_paper.pdf)] [[code](https://github.com/lhkhiem28/gPerXAN)]

Decentralized federated domain generalization with cluster alignment for fault diagnosis (**IFAC Control Engineering Practice 2024**) [[paper](https://www.sciencedirect.com/science/article/abs/pii/S0967066124001114)]

Overcoming Data and Model Heterogeneities in Decentralized Federated Learning via Synthetic Anchors (**arXiv 2024**) [[paper](https://arxiv.org/pdf/2405.11525)] [[code](https://github.com/ubc-tea/DESA)]

### 2023

Gradient Masked Averaging for Federated Learning (**TMLR 2023**) [[paper](https://openreview.net/forum?id=REAyrhRYAo)]

Federated Domain Generalization for Image Recognition via Cross-Client Style Transfer (**WACV 2023**) [[paper](https://openaccess.thecvf.com/content/WACV2023/papers/Chen_Federated_Domain_Generalization_for_Image_Recognition_via_Cross-Client_Style_Transfer_WACV_2023_paper.pdf)] [[code](https://github.com/JeremyCJM/CCST)]

FedCLIP: Fast generalization and personalization for clip in federated learning (**ICLR 2023**) [[paper](https://openreview.net/pdf?id=wgO-OK0_CQ)]

Out-of-Distribution Generalization of Federated Learning via Implicit Invariant Relationships (**PMLR 2023**) [[paper](https://proceedings.mlr.press/v202/guo23b/guo23b.pdf)] [[code](https://github.com/YamingGuo98/FedIIR)]

Federated Domain Generalization with Generalization Adjustment (**CVPR 2023**) [[paper](https://openaccess.thecvf.com/content/CVPR2023/papers/Zhang_Federated_Domain_Generalization_With_Generalization_Adjustment_CVPR_2023_paper.pdf)] [[code](https://github.com/MediaBrain-SJTU/FedDG-GA)]

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
