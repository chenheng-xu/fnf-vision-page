# Fourier Neural Filter as Generic Vision Backbone

[![Paper](https://img.shields.io/badge/Paper-arXiv-red)](https://arxiv.org/abs/XXXX.XXXXX)
[![Code](https://img.shields.io/badge/Code-GitHub-blue)](https://github.com/chenheng-xu/fnf-vision-code)
[![Project Page](https://img.shields.io/badge/Project-Page-green)](https://chenheng-xu.github.io/fnf-vision-page/)
[![ICLR 2026](https://img.shields.io/badge/ICLR-2026-blue)](https://iclr.cc/)

Official project page for **Fourier Neural Filter as Generic Vision Backbone** (ICLR 2026).

## 📌 TL;DR

We propose **Vision Filter (ViF)**, a novel generic backbone for Computer Vision that addresses the limitations of Fourier Neural Operator (FNO) by introducing:

- **Adaptive Modulation**: Enhances sensitivity to high-frequency components in the frequency domain
- **Selective Activation**: Balances local time-domain and global frequency-domain information flow

**Results**: ViF achieves state-of-the-art performance on ImageNet-1K (85.2%), COCO detection (50.1 Box mAP), and ADE20K segmentation (52.3 mIoU) with competitive computational efficiency.

## 🎯 Key Results

### Image Classification (ImageNet-1K)
- **ViF-Tiny**: 83.8% Top-1 accuracy (29M params, 5.1G FLOPs)
- **ViF-Small**: 84.5% Top-1 accuracy (45M params, 7.8G FLOPs)
- **ViF-Base**: 85.2% Top-1 accuracy (96M params, 16.7G FLOPs)

### Object Detection (COCO)
- **ViF-Tiny**: 47.7 Box mAP, 43.0 Mask mAP
- **ViF-Small**: 49.1 Box mAP, 44.0 Mask mAP
- **ViF-Base**: 50.1 Box mAP, 44.6 Mask mAP

### Semantic Segmentation (ADE20K)
- **ViF-Tiny**: 49.6 mIoU (multi-scale)
- **ViF-Small**: 51.3 mIoU (multi-scale)
- **ViF-Base**: 52.3 mIoU (multi-scale)

## 🔬 Key Contributions

1. **Fourier Neural Filter (FNF)**: The first unified backbone that couples time-domain and frequency-domain analysis, inherently preserving the spatial structure of 2D visual representation.

2. **Theoretical Analysis**: We theoretically and empirically demonstrate that our proposed FNF resolves the inherent over-smoothing effect and bandwidth bottleneck of the original FNO.

3. **State-of-the-Art Performance**: The proposed model ViF achieves superior performance on three mainstream visual tasks while maintaining competitive computational efficiency.

## 📚 Website Features

This project page includes:

- **Comprehensive Results**: Detailed performance metrics and comparisons with Transformer- and Mamba-based models
- **Theoretical Contributions**: Mathematical formulations, propositions, and proof sketches
- **Visualizations**: Architecture diagrams, ablation studies, task visualizations, and spatial/frequency analysis
- **Implementation Details**: Training configurations, data augmentation, and hardware specifications
- **Related Work**: Overview of Vision Transformer, Vision Mamba, and Fourier Transform for Vision
- **Datasets**: Information about ImageNet-1K, COCO, and ADE20K datasets
- **Quick Start Guide**: Installation and usage examples

## 🔗 Quick Links

- 📄 [Paper](https://arxiv.org/abs/XXXX.XXXXX) (Coming soon)
- 💻 [Code](https://github.com/chenheng-xu/fnf-vision-code)
- 🌐 [Project Page](https://chenheng-xu.github.io/fnf-vision-page/)

## 📖 Citation

If you find this work useful in your research, please cite:

```bibtex
@article{xu2025fourier,
  title={Fourier Neural Filter as Generic Vision Backbone},
  author={Xu, Chenheng and Ban, Yuanhao and Wu, Dan and Hsieh, Cho-Jui and Wu, Ying Nian and Zhu, Yixin},
  journal={arXiv preprint arXiv:XXXX.XXXXX},
  year={2025}
}
```

## 👥 Authors

- **Chenheng Xu**<sup>1,2,3,4</sup> (Peking University, UCLA)
- **Yuanhao Ban**<sup>2</sup> (UCLA)
- **Dan Wu**<sup>2</sup> (UCLA)
- **Cho-Jui Hsieh**<sup>2,✉</sup> (UCLA)
- **Ying Nian Wu**<sup>2,✉</sup> (UCLA)
- **Yixin Zhu**<sup>1,3,4,✉</sup> (Peking University)

<sup>1</sup>Peking University  
<sup>2</sup>University of California, Los Angeles  
<sup>3</sup>State Key Lab of General AI, Peking University  
<sup>4</sup>Beijing Key Laboratory of Behavior and Mental Health, Peking University

## 🏗️ Project Structure

```
fnf-vision-page/
├── index.html          # Main webpage
├── style.css           # Styling and layout
├── README.md           # This file
├── LICENSE             # MIT License
├── figures/            # All paper figures and visualizations
│   ├── *.png          # High-resolution PNG images (300 DPI)
│   └── *.pdf          # Original PDF figures
└── .github/
    └── workflows/
        └── deploy.yml  # GitHub Pages deployment workflow
```

## 🚀 Local Development

To view the website locally:

1. Clone the repository:
```bash
git clone https://github.com/chenheng-xu/fnf-vision-page.git
cd fnf-vision-page
```

2. Open `index.html` in your web browser, or use a local server:
```bash
# Using Python
python3 -m http.server 8000

# Using Node.js
npx http-server
```

3. Navigate to `http://localhost:8000` in your browser

## 📝 License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

## 🙏 Acknowledgments

This work is submitted to ICLR 2026. For questions and inquiries, please refer to the project page or open an issue on GitHub.
