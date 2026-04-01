# HAFM: A Post-Fusion Gating Module for Haze-Aware RGB–Thermal Object Detection

[![CVPR Findings 2026](https://img.shields.io/badge/CVPR_Findings-2026-blue.svg)](#)

This is the official repository for the paper **"HAFM: A Post-Fusion Gating Module for Haze-Aware RGB–Thermal Object Detection"**, accepted at the **CVPR 2026 Findings Track**.

**Authors:** Juan M. Saeteros, Nick J. Arévalo, Boris X. Vintimilla (ESPOL Polytechnic University, Ecuador).

---

## 📢 Release Schedule (Coming Soon)

**The full source code, datasets, and pre-trained models will be publicly released in June 2026**, coinciding with the CVPR 2026 conference and the publication of the official proceedings. 

The upcoming release will include:
* **Synthetic Haze Generator:** Our depth-guided, non-homogeneous synthesis pipeline using FBM noise and depth-gated sprite compositing.
* **Degradation Mask Estimator:** Training scripts and pre-trained weights for the U-Net model.
* **HAFM Integration:** Plug-and-play implementation of the post-fusion gating module for standard object detection baselines (e.g., CFMW, TarDAL, SeAFusion).

---

## 📖 Abstract

Object detection in adverse weather remains challenging for visible (RGB) cameras, where atmospheric scattering and airlight reduce contrast and obscure fine structures. Thermal infrared (IR) sensing is resistant to illumination and haze but lacks rich textures and sharp boundaries. We address this complementary degradation with the **Haze-Aware Fusion Module (HAFM)**—a lightweight, detector-agnostic post-fusion gating block that re-weights RGB-IR features using a continuous haze mask inferred from RGB. 

Rather than restoring corrupted visible content through dehazing, HAFM explicitly suppresses hazy RGB regions and replaces them with co-located thermal responses, enhancing localization and classification under reduced visibility. Across multiple baselines, HAFM consistently improves mAP under haze (up to +20 mAP50 depending on the backbone) with minimal computational overhead.

---

## ✒️ Citation

If you find our work or the upcoming code useful for your research, please consider citing our paper:

```bibtex
@inproceedings{saeteros2026hafm,
  title={HAFM: A Post-Fusion Gating Module for Haze-Aware RGB-Thermal Object Detection},
  author={Saeteros, Juan M. and Ar{\'e}valo, Nick J. and Vintimilla, Boris X.},
  booktitle={Proceedings of the IEEE/CVF Conference on Computer Vision and Pattern Recognition (CVPR) Findings},
  year={2026}
}
```
*Note: The BibTeX entry will be updated with the exact page numbers once the IEEE proceedings are officially published.*
