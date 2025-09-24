# AnimeGAN

This project implements a **Generative Adversarial Network (GAN)** trained on the [Anime Face Dataset](https://www.kaggle.com/datasets/splcher/animefacedataset) to generate realistic anime-style faces.  
Built with **PyTorch**, the model uses a **CNN-based discriminator** and a **deconvolution-based generator**, both optimized with **Adam**.

---

## 🚀 Features
- Trains a GAN from scratch on the AnimeFace dataset.
- Implements adversarial training with generator & discriminator losses.
- Generates novel anime faces that resemble real anime characters.
- Visualizes loss curves and generated samples at different epochs.

---

## 📂 Dataset
We use the [AnimeFaceDataset (Kaggle)](https://www.kaggle.com/datasets/splcher/animefacedataset).  
Each image is preprocessed:
- Resized to **64x64**
- Normalized to **[-1, 1]** range

---

## 🛠️ Requirements
Install the dependencies with:

```bash
pip install torch torchvision matplotlib opencv-python
