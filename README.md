# Diffusion Models for Calorimeter Shower Generation

A hands-on tutorial on **Diffusion Transformer (DiT)** for **High-Energy Physics (HEP)**, prepared for **[The First Training School on Machine Learning & Quantum Computing for Future Colliders](https://indico.cern.ch/event/1696287/overview)**.

---

## Overview

Diffusion models have recently emerged as one of the most powerful classes of generative models, achieving state-of-the-art performance in image synthesis and scientific machine learning.

In High-Energy Physics, diffusion models provide a promising approach for accelerating computationally expensive detector simulations by learning to generate realistic calorimeter showers from data.

This tutorial introduces the fundamental concepts behind diffusion models and demonstrates how to build and train a **conditional DiT** in PyTorch for calorimeter shower generation. Participants will learn both the theoretical foundations and the practical implementation of diffusion models, from the forward diffusion process to efficient sample generation using DDIM.

---

## Learning Objectives

By the end of this tutorial, participants will be able to:

- Understand the forward and reverse diffusion process.
- Explain how DDPMs are trained.
- Build a conditional diffusion model in PyTorch.
- Train a diffusion model on calorimeter shower data.
- Save and load model checkpoints.
- Resume training from a checkpoint.
- Generate new calorimeter showers using both DDPM and DDIM sampling.

---

## Repository Structure

```text
.
├── Tutorial_Surrogate_Model.ipynb            # Main tutorial notebook
├── Images/                                   # Figures used throughout the notebook
├── checkpoint/                               # Downloaded pretrained checkpoint
├── data/  
├── diffusion/                                # Diffusion process
└── README.md
```

---

## Dataset and Pretrained Model

The tutorial uses a small calorimeter shower dataset together with a pretrained diffusion model.

The following files are downloaded automatically from Zenodo when running the notebook:

**Dataset**

- `Tutorial_Surrogate_Model.ipynb`

**Checkpoint**

- `latest.pt`

No manual download is required.

---

## Requirements

The notebook can be executed either

- locally using Jupyter Notebook or JupyterLab, or
- directly in Google Colab.

Required Python packages include

- PyTorch
- torchvision
- NumPy
- Matplotlib
- h5py
- scikit-image

---

## Getting Started

Clone this repository

```bash
git clone https://github.com/X-T-Nguyen/Diffusion_Model_Tutorial_for_The_first_MLQC4FC_Training_School.git
cd Diffusion_Model_Tutorial_for_The_first_MLQC4FC_Training_School
```

Open

```text
Tutorial_Surrogate_Model.ipynb
```

using

- Jupyter Notebook
- JupyterLab
- Google Colab

The notebook automatically downloads the required dataset and pretrained checkpoint from Zenodo.

---

## Tutorial Contents

The notebook covers the following topics:

1. Introduction to diffusion models
2. Conditional diffusion models
3. Forward diffusion process
4. Noise prediction objective
5. Preparing the calorimeter shower dataset
6. Building the conditional U-Net architecture
7. Training the diffusion model
8. Saving and loading checkpoints
9. DDPM sampling
10. DDIM sampling
11. Generating calorimeter showers

---

## Related Resources

This tutorial presents a simplified implementation of diffusion models for educational purposes. It is based on the methodology developed in our research on differentiable detector simulation and design using diffusion models.

### Publication

**Differentiable surrogate for detector simulation and design with diffusion models**

Xuan Tung Nguyen et al.
Machine Learning: Science and Technology, 7(2), 025061 (2026)
DOI: https://doi.org/10.1088/2632-2153/ae5c56

### Source Code

The complete research implementation, including differentiable detector optimization and full-scale calorimeter shower generation, is available at:

https://github.com/X-T-Nguyen/Diffusion-Surrogate-Detector-Design

---

## Acknowledgements

This tutorial was prepared as part of **The First Training School on Machine Learning & Quantum Computing for Future Colliders** to introduce modern generative models for High-Energy Physics applications and promote hands-on training in scientific machine learning.
