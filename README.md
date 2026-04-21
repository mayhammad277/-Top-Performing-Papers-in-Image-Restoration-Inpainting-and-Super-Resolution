
# 🖼️ Top Performing Papers in Image Restoration, Inpainting, and Super‑Resolution

This repository serves as a curated, up‑to‑date summary of the **top‑performing papers** in three closely related computer vision fields:

- **Image Restoration** – recovering clean images from degraded inputs (noise, blur, rain, low‑light, etc.)
- **Image Inpainting** – filling missing or masked regions with semantically plausible content
- **Super‑Resolution (SR)** – reconstructing high‑resolution details from low‑resolution inputs

The content is continuously updated with the latest **state‑of‑the‑art (SOTA)** papers, benchmark results, and open‑source implementations.

---

## 📋 Table of Contents

- [Image Restoration](#image-restoration)
- [Image Inpainting](#image-inpainting)
- [Super‑Resolution](#super-resolution)
- [Benchmarks & Evaluation Metrics](#benchmarks--evaluation-metrics)
- [Open‑Source Tools & Datasets](#open-source-tools--datasets)
- [Contributing](#contributing)
- [License](#license)

---

## 🛠️ Image Restoration

> **Definition**: Image restoration aims to reconstruct a clean, high‑fidelity image from a degraded observation (noise, blur, low‑light, compression artefacts, etc.).

### 🏆 Top Papers (2022–2026)

| Paper | Venue | Year | Key Contribution | Code |
|-------|-------|------|------------------|------|
| **From Zero to Detail: A Progressive Spectral Decoupling Paradigm for UHD Image Restoration with New Benchmark** | TPAMI | 2026 | ERR framework with 3‑stage spectral decomposition for ultra‑high‑definition restoration; introduces 82k‑image **LSUHDIR** benchmark. | [GitHub](https://github.com/NJU-PCALab/ERR) |
| **Locally‑Supervised Global Image Restoration** | arXiv | 2026 | Reconstructs images from fixed, incomplete measurements using distribution invariances; applied to photoacoustic microscopy. | [arXiv](https://arxiv.org/abs/2511.01998) |
| **MIRAGE: Efficient Degradation‑agnostic Image Restoration via Channel‑Wise Functional Decomposition and Manifold Regularization** | ICLR | 2026 | All‑in‑one restoration; combines CNN, attention & MLP branches for degradation‑agnostic learning; **SOTA** in efficiency‑performance trade‑off. | [arXiv](https://arxiv.org/abs/2505.18679) |
| **HAT: Hybrid Attention Transformer for Image Restoration** | arXiv | 2026 | Combines channel attention + window‑based self‑attention to activate more pixels; strong results on SR and denoising. | [HuggingFace](https://huggingface.co/Acly/hat) |
| **M2Restore: Mixture‑of‑Experts‑based Mamba‑CNN Fusion Framework for All‑in‑One Image Restoration** | arXiv | 2025 | Fuses Mamba (SSM) and CNN via MoE; **SOTA** on multiple benchmarks with low latency. | [GitHub](https://github.com/fub-hagen/M2Restore) |
| **DiffBIR: Towards Blind Image Restoration with Generative Diffusion Prior** | ECCV | 2024 | Two‑stage diffusion pipeline: degradation removal → information regeneration; unified for blind tasks. | [GitHub](https://github.com/XPixelGroup/DiffBIR) |
| **SeedVR2: One‑Step Video Restoration via Diffusion Adversarial Post‑Training** | ICLR | 2026 | Single‑step video restoration with **DiT**; matches multi‑step diffusion methods at high resolution. | [GitHub](https://github.com/IceClear/SeedVR2) |
| **Restormer: Efficient Transformer for High‑Resolution Image Restoration** | CVPR (Oral) | 2022 | **Transformer backbone** for high‑res restoration; **SOTA** on deraining, deblurring, denoising. | [GitHub](https://github.com/swz30/Restormer) |
| **MAXIM: Multi‑Axis MLP for Image Processing** | CVPR (Oral) | 2022 | **MLP‑only** backbone; **SOTA** on >10 benchmarks across denoising, deblurring, deraining, dehazing, enhancement. | [GitHub](https://github.com/google-research/maxim) |

**✨ Honorable Mentions**:  
- **LucidFlux‑14B** (2025) – a **Diffusion Transformer**‑based universal restoration model that surpasses commercial alternatives without relying on captions.  
- **NTIRE 2025 RAIM Challenge** – the leading real‑world restoration benchmark with 600+ submissions.

---

## 🎨 Image Inpainting

> **Definition**: Image inpainting fills missing regions (masks) with content that is both visually plausible and semantically consistent.

### 🏆 Top Papers (2019–2026)

| Paper | Venue | Year | Key Contribution | Code |
|-------|-------|------|------------------|------|
| **SEM‑Net: Efficient Pixel Modelling for Image Inpainting with Spatially Enhanced SSM** | WACV (Oral) | 2025 | **State Space Model (SSM)** for inpainting; linear complexity, **SOTA** on long‑range dependencies. | [Project Page](https://www.hubertshum.com/pbl_wacv2025inpainting.htm) |
| **CSF‑Net: Context‑Semantic Fusion Network for Large Mask Inpainting** | WACV | 2026 | Semantic‑guided inpainting; fuses context with amodal completion priors; reduces hallucination on large masks. | [GitHub](https://github.com/chaeyeonheo/CSF-Net) |
| **BrushNet: A Plug‑and‑Play Image Inpainting Model with Decomposed Dual‑Branch Diffusion** | ECCV | 2024 | **Plug‑and‑play** diffusion‑based inpainting; embeds masked features into any pretrained diffusion model. | [GitHub](https://github.com/TencentARC/BrushNet) |
| **PowerPaint: A Task Is Worth One Word** | ECCV | 2024 | **Versatile** inpainting with learnable task prompts; supports text‑guided insertion, removal, outpainting, shape‑guided inpainting. | [GitHub](https://github.com/open-mmlab/PowerPaint) |
| **AOT‑GAN for High‑Resolution Image Inpainting** | TVCG | 2023 | High‑resolution inpainting via **aggregated contextual transformations**. | [GitHub](https://github.com/researchmm/AOT-GAN-for-Inpainting) |
| **MI‑GAN: A Simple Baseline for Image Inpainting on Mobile Devices** | ICCV | 2023 | Lightweight GAN designed for **mobile inference**; competitive quality with minimal resources. | [GitHub](https://github.com/Picsart-AI-Research/MI-GAN) |
| **LaMa: Large Mask Inpainting** | WACV | 2022 | **Fast Fourier convolutions** for large‑area inpainting; widely adopted as a strong baseline. | [GitHub](https://github.com/advimman/lama) |
| **DeepFill v1/v2** | CVPR/ICCV | 2018/19 | **Gated convolution** and **contextual attention**; seminal works that popularized GAN‑based inpainting. | [GitHub](https://github.com/JiahuiYu/generative_inpainting) |

**🔍 Emerging Trends**:  
- **SSM‑based models** (e.g., SEM‑Net) are challenging CNNs and Transformers with linear complexity.  
- **Diffusion‑based inpainting** (BrushNet, PowerPaint) offers **plug‑and‑play** compatibility with pre‑trained text‑to‑image models.

---

## 🔬 Super‑Resolution (SR)

> **Definition**: Super‑resolution reconstructs high‑resolution images from low‑resolution inputs, either by **upsampling** or **blind real‑world SR**.

### 🏆 Top Papers (2021–2026)

| Paper | Venue | Year | Key Contribution | Code |
|-------|-------|------|------------------|------|
| **CASR: A Robust Cyclic Framework for Arbitrary Large‑Scale Super‑Resolution** | arXiv | 2026 | **Cyclic SR**; reformulates large‑scale SR as a sequence of in‑distribution scale transitions; **single model for arbitrary scales**. | [arXiv](https://arxiv.org/abs/2602.22159) |
| **RCOD: Realism Control One‑step Diffusion for Real‑world Image Super Resolution** | AAAI | 2026 | **One‑step diffusion** for real‑world SR; explicit **fidelity‑realism trade‑off control**; SOTA efficiency. | [AAAI](https://ojs.aaai.org/index.php/AAAI/article/view/38067) |
| **SUPIR: Scaling‑UP Image Restoration** | CVPR | 2024 | **Large‑scale model** with generative prior; text‑guided restoration; **SOTA** on real‑world low‑quality images. | [GitHub](https://github.com/Septivi10/SUPIR) |
| **AESRGAN** | – | 2024‑2025 | **Attention‑enhanced** ESRGAN; improves detail preservation and visual appeal; **outperforms Real‑ESRGAN**. | [GitHub](https://github.com/idealvin/AESRGAN) |
| **CodeFormer: Towards Robust Blind Face Restoration with Codebook Lookup Transformer** | NeurIPS | 2022 | **Discrete codebook prior** + transformer; **SOTA** for blind face restoration. | [GitHub](https://github.com/sczhou/CodeFormer) |
| **SwinIR: Image Restoration Using Swin Transformer** | ICCV (Oral) | 2021 | **Swin Transformer** for image restoration; strong SR baseline with efficient local attention. | [GitHub](https://github.com/JingyunLiang/SwinIR) |
| **Real‑ESRGAN: Practical Algorithms for General Image/Video Restoration** | ICCV (Oral) | 2021 | **Real‑world SR** with high‑order degradation pipeline; widely used for practical upscaling. | [GitHub](https://github.com/xinntao/Real-ESRGAN) |
| **GFPGAN: Practical Algorithms for Real‑world Face Restoration** | – | 2021 | **Face‑specific SR** with generative prior; restores old/blurry faces. | [GitHub](https://github.com/TencentARC/GFPGAN) |

**📊 Benchmark Highlights**:
- **NTIRE 2025 Efficient Super‑Resolution Challenge** – focuses on **PSNR ≥ 26.90** while minimising FLOPs and parameters.
- **AIM 2025 Efficient Perceptual SR Benchmark** – **VPEG** achieves highest perceptual quality with only **~19%** of Real‑ESRGAN’s parameters.

---

## 📊 Benchmarks & Evaluation Metrics

### 🔬 Common Datasets

| Dataset | Domain | Use |
|---------|--------|-----|
| **LSUHDIR** | UHD natural images | Ultra‑high‑definition restoration |
| **Places365** | Scene images | Inpainting, restoration |
| **COCOA** | Common objects with amodal annotations | Large‑mask inpainting |
| **Set5 / Set14 / BSD100 / Urban100** | Classic SR benchmarks | Bicubic SR evaluation |
| **RealSR / DRealSR** | Real‑world low‑high pairs | Real‑world SR |
| **GoPro / HIDE / RealBlur** | Motion blur | Deblurring |

### 📈 Evaluation Metrics

| Metric | Full Name | Use Case |
|--------|-----------|----------|
| **PSNR** | Peak Signal‑to‑Noise Ratio | Pixel‑wise fidelity (higher is better) |
| **SSIM** | Structural Similarity Index | Perceived structural similarity (0–1, higher better) |
| **LPIPS** | Learned Perceptual Image Patch Similarity | Perceptual quality (lower is better) |
| **FID** | Fréchet Inception Distance | Distributional similarity (lower better) |
| **NIQE** | Naturalness Image Quality Evaluator | No‑reference perceptual quality (lower better) |

---

## 🧰 Open‑Source Tools & Datasets

### 🔗 Popular Repositories

| Repository | Description | Stars |
|------------|-------------|-------|
| [Real‑ESRGAN](https://github.com/xinntao/Real-ESRGAN) | Practical blind SR for real‑world images/video | 35k+ |
| [GFPGAN](https://github.com/TencentARC/GFPGAN) | Real‑world face restoration | 37k+ |
| [BasicSR](https://github.com/XPixelGroup/BasicSR) | PyTorch toolbox for image/video restoration | 7k+ |
| [OpenMMLab MMagic](https://github.com/open-mmlab/MMagic) | Unified AIGC toolbox for restoration, editing, generation | 7k+ |
| [Image Inpainting Papers](https://github.com/1900zyh/Awesome-Image-Inpainting) | Curated list of inpainting papers | 1k+ |
| [Super‑Resolution Survey](https://github.com/Kokeip/Super-resolution-survey) | Benchmarking SR models under a unified framework | 500+ |

### 🗂️ Datasets

- [LSUHDIR](https://github.com/NJU-PCALab/ERR) – 82k UHD images for restoration.
- [NTIRE 2025 RAIM datasets](https://drive.google.com/drive/folders/1Mgqve-yNcE26IIieI8lMIf-25VvZRs_J) – Real‑world low‑light and detail enhancement.
- [COCO‑Inpaint](https://arxiv.org/abs/2504.11076) – Benchmark for inpainting detection and manipulation localisation.

---

## 🤝 Contributing

Contributions are welcome! If you want to add a new paper, fix an error, or improve the organisation, please:

1. Fork this repository.
2. Create a feature branch (`git checkout -b feature/amazing-paper`).
3. Commit your changes (`git commit -m 'Add some amazing paper'`).
4. Push to the branch (`git push origin feature/amazing-paper`).
5. Open a Pull Request.

Please ensure that any new papers are **peer‑reviewed** and include a **code link** (if available).

---

## 📄 License

This curated list is provided under the [MIT License](LICENSE). All referenced papers, code, and datasets remain the property of their respective authors.

---

*Last updated: **April 2026** – for the latest papers, watch this repository or check the [releases](https://github.com/your-repo/releases) page.*
