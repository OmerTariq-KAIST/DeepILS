 ## DeepILS: Towards Accurate Domain Invariant AIoT-enabled Inertial Localization System (IEEE Internet of Things Journal 2025)

Abstract
----------
Accurate indoor localization and navigation enable real-time, ubiquitous, location-based services. Over the past decade, data-driven approaches for inertial odometry have shown the potential to enhance indoor positioning accuracy. However, low-cost inertial measurement units (IMUs), commonly used in smartphones and IoT devices, are prone to significant noise, leading to drift and degraded performance in navigation algorithms. This paper presents a novel, lightweight, and real-time end-to-end framework, DeepILS, designed to process raw inertial data for precise pedestrian localization in indoor environments. DeepILS utilizes a residual network enhanced with channel-wise and spatial attention mechanisms, enabling accurate velocity and position estimation across diverse motion dynamics. The framework’s effectiveness is validated using four benchmarks and two newly introduced datasets in real-time edge scenarios. These datasets were collected across diverse indoor environments at the KAIST campus and Incheon National Airport, using multiple hardware platforms, including the KAIST IoT positioning module and Android smartphones. Experimental results, including tests on unseen data and comprehensive ablation studies, demonstrate that DeepILS improves localization accuracy by 70% compared to state-of-the-art methods while effectively mitigating sensor noise and enhancing robustness in real-world environments. Specifically, DeepILS exhibits excellent edge performance on IoT devices, making it highly suitable for real-time applications.

[[Paper JIOT](https://ieeexplore.ieee.org/document/10873819)]

# Architectures
DeepILS with other lightweight S.O.T.A. model architectures are presented for comparative analysis. IMUNet, MobileNet, MobileNetV2, MnasNet, and EfficientNetB0 models have been re-implemented to work with one-dimensional Inertial data.

DeepILS (state-of-the-art Inertial Navigation Performance!)
----------
* Network architecture

![image](https://github.com/user-attachments/assets/fe621df9-0ea6-4eff-bcbb-d98ca081884c)


# Dataset
1. DeepILS is evaluated on six inertial odometry datssets.
2. You can download the proposed datasets from [KIOD, INAIOD](https://drive.google.com/file/d/1qtACj3BOiiOi0pgD0BrE8zD5OmH-Xi1A/view?usp=sharing)
3. IMUNet dataset can be downloaded from [IMUNet](https://www.dropbox.com/scl/fi/7o6qr0vexylxhec2u4xoi/IMUNet_dataset.zip?rlkey=h8u5374ow5djg2ybul74q2e5q&dl=0https://www.dropbox.com/scl/fi/7o6qr0vexylxhec2u4xoi/IMUNet_dataset.zip?rlkey=h8u5374ow5djg2ybul74q2e5q&dl=0)
4. OxIOD dataset can be downloaded from [OxIOD](https://drive.google.com/open?id=1UCHY3ENCybcBNyiC2wx1gQEWSLqzJag0)
5. RoNIN dataset can be downloaded from [RoNIN](https://ronin.cs.sfu.ca/#dataset)
6. RIDI dataset can be downloaded from [RIDI](https://www.kaggle.com/code/kmader/ridi-data-overview/data)

# Results
The inertial trajectories and checkpoints for 6 datasets evaluated on DeepILS are available in the folder /results

# Android
The DeepILS Mobile application is available at [DeepILS-Mobile](https://drive.google.com/file/d/15T4dHczYPHEoxazvyNO9vQIJLl1GPZLZ/view?usp=sharing). 


# Requirements

Dependencies can be installed using the following command:
```bash
conda env create -f DeepILS.yml
```

Citation
----------
```BibTex
@ARTICLE{10873819,
  author={Tariq, Omer and Dastagir, Bilal and Bilal, Muhammad and Han, Dongsoo},
  journal={IEEE Internet of Things Journal}, 
  title={DeepILS: Towards Accurate Domain Invariant AIoT-enabled Inertial Localization System}, 
  year={2025},
  volume={},
  number={},
  pages={1-1},
  keywords={Location awareness;Internet of Things;Computational modeling;Real-time systems;Data models;Accuracy;Smart phones;Pedestrians;Odometry;Performance evaluation;Pedestrian Localization;Indoor Navigation;Deep Neural Networks (DNN);Convolution;State Estimation;Quantization;ONNX;ZUPT;Deep Inertial Odometry;Artificial Intelligence of Things (AIoT)},
  doi={10.1109/JIOT.2025.3538938}}
```

