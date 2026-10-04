# Galaxy Morphology Classification with DINOv2

A study comparing **self-supervised DINOv2 representations** with **supervised CNN models** for galaxy morphology classification.

## Overview

The project evaluates how well pretrained visual representations work when only a limited amount of labelled astronomical data is available.

### Models
- Frozen DINOv2 + Linear Probe
- Frozen DINOv2 + MLP Probe
- ResNet-18 trained from scratch
- ImageNet-pretrained ResNet-18
- Fine-tuned DINOv2

## Experiments

- Multi-seed and multi-label-fraction evaluation
- Label-efficiency analysis
- Accuracy and macro-F1
- 95% confidence intervals
- Statistical significance testing
- Per-class precision, recall and F1
- Confusion matrices and error analysis
- t-SNE visualization of DINOv2 embeddings
- DINOv2 attention visualization
- Computational efficiency comparison
- Ablation studies

## Notebooks

1. `Notebook_1_Data_and_DINOv2_Probes.ipynb` — Dataset preparation, morphology labels, DINOv2 embeddings and frozen probes.
2. `Notebook_2_ResNet18_From_Scratch.ipynb` — ResNet-18 baseline trained from scratch.
3. `Notebook_3_Transfer_Models_and_Analysis.ipynb` — Transfer-learning experiments and complete statistical/error analysis.

## Dataset

Galaxy Zoo 2 (GZ2) data with a scientifically defined 5-class galaxy morphology classification scheme.

## Tech Stack

Python · PyTorch · DINOv2 · torchvision · scikit-learn · NumPy · Pandas · Matplotlib · Seaborn

## References

- Oquab et al., *DINOv2: Learning Robust Visual Features without Supervision*, 2023.
- Willett et al., *Galaxy Zoo 2*, 2013.
- He et al., *Deep Residual Learning for Image Recognition*, 2016.
- Manwadkar & Kapare, *AstroDINO*, 2025.
