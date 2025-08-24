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
- Federated Domain Generalization with Data-free On-server Matching Gradient (FedOMG) (**ICLR 2025**) [[paper](https://openreview.net/pdf?id=8TERgu1Lb2)]
- Enhancing Foundation Models with Federated Domain Knowledge Infusion (FedAG) (**ICML 2025**) [[paper](https://icml.cc/virtual/2025/poster/46374)]
- TTA-FedDG: Leveraging Test-Time Adaptation to Address Federated Domain Generalization (**AAAI 2025**) [[paper](https://ojs.aaai.org/index.php/AAAI/article/view/34053)]
- Federated Unsupervised Domain Generalization Using Global and Local Alignment of Gradients (FedGaLA) (**AAAI 2025**) [[paper](https://ojs.aaai.org/index.php/AAAI/article/view/34197)]
- Improving Federated Domain Generalization Through Dynamical Weights Calculated from Data Influences on Global Model Update (DI) (**AAAI 2025**) [[paper](https://ojs.aaai.org/index.php/AAAI/article/view/34468)]
- FedGOG: Federated Graph Out-of-Distribution Generalization (**AAAI 2025**) [[paper](https://ojs.aaai.org/index.php/AAAI/article/view/34459/36614)]
- Multi-Source Collaborative Style Augmentation and Domain-Invariant Learning for Federated Domain Generalization (MCSAD) (**IJCAI 2025**) [[paper](https://arxiv.org/abs/2505.10152)]
- Federated Learning with Domain Shift Eraser (FDSE) (**CVPR 2025**) \[[paper](https://openaccess.thecvf.com/content/CVPR2025/html/Wang_Federated_Learning_with_Domain_Shift_Eraser_CVPR_2025_paper.html)]
- BTFL: A Bayesian-based Test-Time Generalization Method for Internal and External Data Distributions in Federated Learning (**KDD 2025**) [[paper](https://dl.acm.org/doi/10.1145/3690624.3709309)]
- Vision enhancement and consistency assurance for multicenter fundus image segmentation (FedDG-VECA) (**Pattern Recognition 2025**) [[paper](https://doi.org/10.1016/j.patcog.2025.111324)]
- A Causal Unbiased Optimization Method for Federated Domain Generalization (**Knowledge-Based Systems 2025**) [[paper](https://doi.org/10.1016/j.knosys.2025.112220)]
- A unified Personalized Federated Learning framework ensuring Domain Generalization (**Expert Systems with Applications 2025**) [[paper](https://doi.org/10.1016/j.eswa.2024.125700)]
- FedTG: Text-guided Federated Domain Generalization (**ICASSP 2025**) [[paper](https://doi.org/10.1109/ICASSP49660.2025.10888120)]
- Federated Domain Generalization with Label Smoothing and Balanced Decentralized Training (**ICASSP 2025**) [[paper](https://doi.org/10.1109/ICASSP49660.2025.10888230)] [[code](https://github.com/AhmedMostafaSoliman/FedPartWhole)]
- Frequency-Based Federated Domain Generalization for Polyp Segmentation (**ICASSP 2025**) [[paper](https://doi.org/10.1109/ICASSP49660.2025.10889662)] [[code](https://github.com/nubagcilab/icassp2025-fdgpolyp)]
- Federated Domain Generalization for Fault Diagnosis: Cross-Client Style Integration and Dual Alignment Representation (**IEEE IoT-J 2025**) [[paper](https://doi.org/10.1109/JIOT.2025.3551339)]
- Heterogeneous Federated Learning: Client-Side Collaborative Update Interdomain Generalization Method for Intelligent Fault Diagnosis (**IEEE IoT-J 2025**) [[paper](https://doi.org/10.1109/JIOT.2024.3489617)]
- Fedpartwhole: federated domain generalization via consistent part-whole hierarchies (**PAA 2025**) [[paper](https://doi.org/10.1007/s10044-025-01439-4)] [[code](https://github.com/AhmedMostafaSoliman/FedPartWhole)]
### 2024
- Decentralized federated domain generalization with cluster alignment for fault diagnosis (**Control Engineering Practice 2024**) [[paper](https://doi.org/10.1016/j.conengprac.2024.105951)]
- DiPrompT: Disentangled Prompt Tuning for Multiple Latent Domain Generalization in Federated Learning (**CVPR 2024**) [[paper](https://openaccess.thecvf.com/content/CVPR2024/html/Bai_DiPrompT_Disentangled_Prompt_Tuning_for_Multiple_Latent_Domain_Generalization_in_CVPR_2024_paper.html)]
- Efficiently Assemble Normalization Layers and Regularization for Federated Domain Generalization (**CVPR 2024**) [[paper](https://openaccess.thecvf.com/content/CVPR2024/html/Le_Efficiently_Assemble_Normalization_Layers_and_Regularization_for_Federated_Domain_Generalization_CVPR_2024_paper.html)] [[code](https://github.com/lhkhiem28/gPerXAN)]
- A unified Personalized Federated Learning framework for improving performance on Non-IID data via domain generalization (**ESWA 2024**) [[paper](https://doi.org/10.1016/j.eswa.2024.125700)]
- Bilateral Proxy Federated Domain Generalization for Privacy-preserving Medical Image Diagnosis (**IEEE J-BHI 2024**) [[paper](https://doi.org/10.1109/JBHI.2024.3456440)]
- Federated Adversarial Domain Hallucination for Privacy-Preserving Domain Generalization (**IEEE TMM 2023**) [[paper](https://doi.org/10.1109/tmm.2023.3257566)]
### 2023
- Federated Domain Generalization With Generalization Adjustment (**CVPR 2023**) [[paper](https://openaccess.thecvf.com/content/CVPR2023/html/Zhang_Federated_Domain_Generalization_With_Generalization_Adjustment_CVPR_2023_paper.html)] [[code](https://github.com/MediaBrain-SJTU/FedDG-GA)]
- Federated Learning for IoT Devices With Domain Generalization (**IEEE Internet of Things Journal 2023**) [[paper](https://doi.org/10.1109/JIOT.2022.3173489)]
- Collaborative Semantic Aggregation and Calibration for Federated Domain Generalization (**IEEE TKDE 2023**) [[paper](https://doi.org/10.1109/TKDE.2023.3273882)]
- Domain Generalization for Foreground Segmentation Using Federated Learning (**ISVC 2023**) [[paper](https://doi.org/10.1007/978-3-031-47969-4_20)]
- Federated Condition Generalization on Low-dose CT Reconstruction via Cross-domain Learning (**MICCAI 2023**) [[paper](https://doi.org/10.1007/978-3-031-43898-1_5)]
- StableFDG: Style and Attention Based Learning for Federated Domain Generalization (**NeurIPS**) [[paper](https://proceedings.neurips.cc/paper_files/paper/2023/hash/dae8bdacd265399b193e6b43d44a80f0-Abstract-Conference.html)]
- Enhancing domain generalization in the AI-based analysis of chest radiographs with federated learning (**Sci Rep 2023**) [[paper](https://doi.org/10.1038/s41598-023-49956-8)] [[code](https://github.com/tayebiarasteh/fldomain)]
- Enhancing domain generalization in the AI-based analysis of chest radiographs with federated learning (**Scientific Reports 2023**) [[paper](https://doi.org/10.1038/s41598-023-49956-8)] [[code](https://github.com/tayebiarasteh/FLdomain)]
- Federated Domain Generalization for Image Recognition via Cross-Client Style Transfer (**WACV 2023**) [[paper](https://openaccess.thecvf.com/content/WACV2023/html/Chen_Federated_Domain_Generalization_for_Image_Recognition_via_Cross-Client_Style_Transfer_WACV_2023_paper.html)] [[code](https://github.com/JeremyCJM/CCST)]
### 2022
- Feature Distribution Matching for Federated Domain Generalization (**ACML 2022**) [[paper](https://proceedings.mlr.press/v189/sun23a/sun23a.pdf)] [[code](https://github.com/yuweisunn/federated-knowledge-alignment)]
- FedSR: A Simple and Effective Domain Generalization Method for Federated Learning (**NeurIPS 2022**) [[paper](https://proceedings.neurips.cc/paper_files/paper/2022/hash/fd946a6c99541fddc3d64a3ea39a1bc2-Abstract-Conference.html)] [[code](https://github.com/atuannguyen/FedSR)]
- FL Games: A federated learning framework for distribution shifts (**FL-NeurIPS 2022**) [[paper](https://arxiv.org/pdf/2205.11101)]
- Generalized Federated Learning via Sharpness Aware Minimization (**PMLR 2022**) [[paper](https://proceedings.mlr.press/v162/qu22a.html)] [[code](https://github.com/NAVER-INTEL-Co-Lab/gaudi-byzantine)]
- Improving Generalization in Federated Learning by Seeking Flat Minima (**ECCV 2022**) [[paper](https://doi.org/10.1007/978-3-031-20050-2_38)] [[code](https://github.com/debcaldarola/fedsam)]
### 2021
- Collaborative optimization and aggregation for decentralized domain generalization and adaptation (**ICCV 2021**) [[paper](https://openaccess.thecvf.com/content/ICCV2021/html/Wu_Collaborative_Optimization_and_Aggregation_for_Decentralized_Domain_Generalization_and_Adaptation_ICCV_2021_paper.html)]
- FedDG: Federated Domain Generalization on Medical Image Segmentation via Episodic Learning in Continuous Frequency Space (**CVPR 2021**) [[paper](https://openaccess.thecvf.com/content/CVPR2021/html/Liu_FedDG_Federated_Domain_Generalization_on_Medical_Image_Segmentation_via_Episodic_CVPR_2021_paper.html)] [[code](https://github.com/liuquande/FedDG-ELCFS)]
