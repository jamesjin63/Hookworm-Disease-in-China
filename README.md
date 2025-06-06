# Spatial Distribution and Risk Factors of Hookworm Disease in China (2016–2021)

**Authors**: Huihui Zhu, Jilei Huang, Jinxin Zheng, Changhai Zhou, Tingjun Zhu, Mizhen Zhang, Luyuan Zhao, Xiaohong Wu, Jingbo Xue, Xiaonong Zhou, Shizhu Li, Menbao Qian  
**Affiliations**: National Institute of Parasitic Diseases, Chinese CDC; Shanghai Jiao Tong University School of Medicine  
**Corresponding Authors**: Xiaonong Zhou*, Shizhu Li*, Menbao Qian*

---

## 📌 Description

This repository contains the code and data processing pipeline for the spatial epidemiological analysis of hookworm infection across 31 provincial-level administrative divisions (PLADs) in China from 2016 to 2021. It integrates geostatistical methods and machine learning to identify spatial patterns and major risk factors influencing hookworm prevalence.

---

## 📊 Objectives

- Map spatial distribution of hookworm disease at township level.
- Detect geographic and spatiotemporal clustering using spatial autocorrelation and scan statistics.
- Identify key environmental and behavioral determinants using machine learning.
- Provide policy-relevant guidance for targeted hookworm control in endemic areas.

---

---

## 🧪 Methods Overview

### 1. **Spatial Analysis**
- **Global Moran's I** and **Local Indicators of Spatial Association (LISA)** to detect spatial autocorrelation.
- **Hotspot analysis (Getis-Ord Gi*)** for high-risk clustering.
- **Standard Deviation Ellipse (SDE)** for directional trend and geographic center estimation.

### 2. **Spatiotemporal Scan**
- Conducted using **SaTScan** software to identify clusters in space-time dimension.
- Poisson model used to detect significant risk areas from 2016–2021.

### 3. **Machine Learning Modeling**
- Gradient Boosting Trees (XGBoost) to determine key predictors among 40 variables.
- Top risk factors: 
  - Frequency of barefoot farming
  - Land use/land cover type
  - Q3 average relative humidity
  - Q3 average sunshine hours

---

## 🔑 Key Findings

- High hookworm prevalence in **southwestern China**; coldspots in **northeastern China**.
- Higher risk among **elderly (≥60 years)** and **females**.
- Climatic and behavioral factors interact significantly.
- **Barefoot farming** is the strongest modifiable risk factor.

---

## 📦 Installation

```bash
git clone https://github.com/yourusername/hookworm-risk-mapping.git
cd hookworm-risk-mapping
pip install -r requirements.txt
