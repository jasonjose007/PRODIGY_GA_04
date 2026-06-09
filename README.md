# PRODIGY_GA_04: Image-to-Image Translation with Conditional GANs (Pix2Pix)

An end-to-end implementation of a **Conditional Generative Adversarial Network (cGAN)** built using TensorFlow/Keras to perform image-to-image mapping.

## 📌 Project Overview
This repository contains a Pix2Pix architecture trained on architectural facade datasets. The network takes a semantic segmentation layout map as an input constraint and reconstructs it into a realistic photorealistic building image. Detailed inline explanations of the adversarial game theory are documented within the code.

## 🚀 Key Features
* **Generator (U-Net):** Employs an encoder-decoder framework with skip connections to preserve localized spatial features.
* **Discriminator (PatchGAN):** Evaluates image validity at the patch level (NxN pixels) rather than the full frame, promoting sharp, high-frequency textures.
* **Adversarial Loss Mapping:** Combines standard Binary Cross-Entropy (adversarial loss) with an L1 regularization penalty ($\lambda = 100$) to force structural correctness.
* **Performance Acceleration:** Fully executed on a Google Colab T4 GPU platform.

## 🧠 Core Concepts Documented Inside
* **Conditional GAN Logic:** Understanding how the model conditions both the generator and discriminator on a source reference matrix.
* **Adversarial Optimization:** Tracking the training balance where the generator minimizes loss while the discriminator maximizes it.

---
*Internship project for the Prodigy InfoTech Generative AI Track.*
