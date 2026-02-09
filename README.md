# 🌧️ Multimodal Monsoon Indian Dataset (1 km)

This repository provides **code, metadata, and documentation** associated with the **Multimodal Monsoon Indian Dataset**, a high-resolution Earth-observation dataset curated for **monsoon precipitation classification and analysis across Indian states**.

> 🔗 **The full dataset is hosted on Hugging Face:**  
> 👉 https://huggingface.co/datasets/swaib/Multimodal_Monsoon_Indian_Dataset

---

## 📌 Why the Dataset Is Hosted on Hugging Face

Due to GitHub file size limitations and to ensure **reliable, long-term hosting**, all large geospatial files (GeoTIFFs, climate rasters, masks) are hosted on **Hugging Face Datasets**, which provides:

- Stable dataset URLs  
- Efficient large-file storage  
- Proper dataset cards and citation support  
- Better visibility and reuse within the research community  

This GitHub repository intentionally contains **no large data files**.

---

## 🌍 Dataset Overview

The **Multimodal Monsoon Indian Dataset** is a curated, high-resolution (~1 km) dataset designed for **Climate AI and geospatial machine learning** research. It integrates multiple Earth-observation modalities into a unified, state-wise structure.

**Key characteristics:**
- **Spatial resolution:** ~1 km × 1 km  
- **Geographic scope:** Indian states  
- **Focus:** Monsoon precipitation classification and analysis  
- **Data format:** Raw geospatial exports (GeoTIFF / CSV / masks)  

---

## 🗺️ Geographic Coverage

The dataset currently includes the following Indian states:

- **Assam**  
- **Bihar**  
- **Himachal Pradesh**  
- **Karnataka**  
- **Kerala**  

Each state was processed using the **same notebook-based pipeline**, ensuring methodological consistency across regions.

---

## 🧩 Modalities Included

Depending on state and data availability, the dataset includes:

### 🛰️ Satellite-Derived Features
- NDVI and vegetation indices  
- Land Surface Temperature (LST)  
- Spectral bands and derived indices  

### 🌦️ Climate & Reanalysis Variables
- ERA5 atmospheric variables  
- Aggregated precipitation and climate fields  

### 🗻 Static Geospatial Context
- Elevation / topography  
- Land-use / land-cover (LULC)  

### 🏷️ Labels
- Pixel-wise or region-wise precipitation classes  
- Label definitions documented in the `metadata/` directory  

---

## 📂 Repository Structure (GitHub)

This GitHub repository contains **supporting material only**

---

### 🧪 How the Data Was Generated

Each state dataset was generated using a dedicated Jupyter notebook (e.g., Assam.ipynb) following the same pipeline:

Define the state boundary and spatial grid

Query satellite and climate data (Google Earth Engine / ERA5)

Export aligned raster layers at ~1 km resolution

Generate precipitation labels

Save raw artifacts (GeoTIFF / CSV)

This ensures reproducibility and consistency across all states.

---

### 🧠 Intended Use

This dataset is designed for:

Climate AI research

Multimodal and geospatial deep learning

Precipitation classification and benchmarking

Regional monsoon analysis over India

---

⚠️ The dataset is provided as raw geospatial artifacts. Users are expected to perform task-specific preprocessing such as tiling, normalization, and temporal aggregation.



