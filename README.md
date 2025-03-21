# DeepBoil---Climate-Change-Project

📘 Project Overiview:
This repository contains the links notebooks for various models evaluated on bubble flow dynamics, developed as part of our project submission for the Climate Change module. Contributors: Marie-Ange Geagea, Yeji Kim, Zhuo Chen.

# Predicting Bubble Dynamics with Deep Learning

## Motivation: 
Boiling is a complex phase-change phenomenon essential for applications like electronics cooling, nuclear energy, and desalination. However,
modeling boiling bubbles is challenging due to multiphysics interactions, including phase transitions, fluid dynamics, and heat transfer.
Traditional CFD simulations are costly and hard to scale. BubbleML, a high-resolution dataset from Flash-X simulations, enables ML models to
efficiently learn and predict bubble dynamics. By leveraging data-driven approaches, we aim to bridge the gap between physical simulations and
forecasting, making bubble behavior prediction more accessible and cost-effective

## 📊 Dataset Description

- **Name**: BubbleML
- **Timesteps**: 500
- **Resolution**: 288×96 (half-bubble view, symmetric expansion to 192 for visualization)
- **Channels**: 2 (velocity_x, velocity_y)
- **Main GitHub Repository**: https://github.com/HPCForge/BubbleML/tree/main?tab=readme-ov-file 
- **Dataset Download Link:**: https://github.com/HPCForge/BubbleML/blob/main/bubbleml_data/README.md

## 📁 Repository Contents

This repository contains three different model implementations for predicting the velocity fields of boiling bubbles over time:

- **UNet**: A convolutional encoder-decoder model optimized for spatial pattern recognition. https://colab.research.google.com/drive/1Dr5Lm_bKwjoUFLLV3LnQ2IEeUKOyZeRn?usp=sharing
- **FNO (Fourier Neural Operator)**: A spectral model designed for learning spatiotemporal patterns, particularly suited for PDE-like problems. https://colab.research.google.com/drive/1ura3AK4RTJWFTvuAkxsUuAk5v5-BwN8D?usp=sharing
- **ConvLSTM**: A model combining convolutional layers and LSTM to capture both spatial and temporal dependencies. https://colab.research.google.com/drive/1NkVe6KD5u5eEqSqFTVdV_9zmaTC9ot7b?usp=sharing
- **Poster**: The DeepBoil_ClimateChangePoster_Final.pdf file is a summary of our work and findings. 

## 📌 Highlights from the Poster

You can view our project summary and results in the [poster](./poster/DeepBoil_ClimateChangePoster_Final.pdf). It includes:
- Model architectures
- One-step and rollout (multi-step) predictions
- Training and validation losses
- Visualizations of predicted velocity fields

## 👥 Team Members
Marie-Ange Geagea
Yeji Kim
Zhuo Chen
