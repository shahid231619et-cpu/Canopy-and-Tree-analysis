# 🌿 Canopy Analysis & 🗺️ Map Tiles

##  Live Demo
- **Canopy Analysis App** →  https://canopy-analysis.onrender.com/
- 
- **Map Tiles App** → https://map-tiles.onrender.com/


##  GitHub Repositories
- **Canopy Analysis Repository** → [View Code](https://github.com/Faraaz1806/canopy-analysis)
- **Map Tiles Repository** → [View Code](https://github.com/Faraaz1806/map-tiles-)


##  How to Use (Canopy Analysis)
1. Open the [Canopy Analysis App](https://canopy-analysis.onrender.com/).  
2. Choose a **sample image** from the gallery or **upload your own image**. (Threshold )  
3. Click **Analyze** (you may need to click twice:  
   - First click → uploads the image  
   - Second click → runs the analysis).  
4. View the results: canopy height map, tree detection, and summary stats.
---


# 🌲 Canopy Height Analysis Model Overview

## Model: PVTv2 (Primary)
- **Type:** Vision Transformer (PVTv2)  
- **Training Dataset:** LIDAR Canopy Height Dataset  
- **Epoch:** 22  
- **Training Accuracy:** 40%  
- **R² Score:** 35%  
- **RMSE:** 11.63m  

---

## Training Details
- **Dataset:**
  - Source: LIDAR Canopy Height Dataset  
  - Resolution: High-res aerial images  
  - Labels: Per-pixel canopy height (meters)  
- **Augmentation:** Random crop, flip, color jitter  
- **Validation:**
  - Split: 80% train / 20% val  
  - Metrics: RMSE, R²  

---

## ConvNeXt Model (In Training)
- **Type:** ConvNeXt V2  
- **Status:** Training in progress  
- **Dataset:** LIDAR Canopy Height Dataset  
- **Expected Improvements:** Better generalization, lower RMSE, higher accuracy on unseen regions  
- **Model File:** Will be added after training  

---

## Model Accuracy Visualization
![Canopy Height Model Accuracy](evaluation/error_histogram_pvtv2.png)

*Above: Error histogram for PVTv2 model on validation set (LIDAR dataset)*

---

## References
- [PVTv2 Paper](https://arxiv.org/abs/2106.13797)  
- [ConvNeXt Paper](https://arxiv.org/abs/2201.03545)  
- [LIDAR Canopy Dataset](https://example.com/lidar-dataset)


# 🗺️ Map View Module

This module provides the **interactive map visualization system** .

---## Features
-  Cesium 3D globe and 2D map view  
-  Satellite imagery overlays (multiple providers)  
-  Interactive polygon 
-  Custom map controls (zoom, fullscreen, layers)  
-  Python backend for advanced data APIs  
-  Secure credential management  
-  ###When user click on polygon -> show details of project####
---
