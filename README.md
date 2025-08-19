This repository contains a Python pipeline for analyzing time–density curves (TDCs) in aneurysm imaging using **circulant matrix–based singular value decomposition (SVD)**.  
It computes standard perfusion and angiographic parameters and performs deconvolution to extract the **impulse response function (IRF)**, Residue Blood Flow (RBF), Residue Blood Volume (RBV), and Mean Transit Time (MTT).

---

## 🔑 Features
- **API_parameters**: Extracts BAT, PH, TTP, AUC, MTT, and maximum derivative.
- **API_SVD**: Performs circulant-SVD based deconvolution with truncation.
- **Data handling**: Reads `.raw` projection images and `.tif` masks for aneurysm and inlet regions.
- **Signal processing**:
  - Median filtering
  - Cross-correlation between inlet and aneurysm TDCs
  - FFT-based convolution for forward validation
- **Metrics**: RMS error between reconstructed and measured aneurysm TDC.
- **Visualization**: 
  - TDCs (aneurysm vs inlet)
  - Reconstructed vs measured TDC
  - Impulse Response Function (IRF)
  - Overlay of ROI masks on projection images

---
