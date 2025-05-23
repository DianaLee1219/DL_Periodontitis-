# Deep Learning Model for Periodontitis Stage Classification

A deep learning framework for classifying **periodontitis stages** from **dental panoramic radiographs**, based on the study:  
**"Deep Learning Model for Classifying Periodontitis Stages on Dental Panoramic Radiography"**

> 📌 **Performance**:  
> - Accuracy: **92.9%**  
> - Average Recall: **80.7%**  
> - Average Precision: **72.4%**

## 📄 Abstract

This repository replicates and builds upon a deep learning framework that classifies the **stage of periodontitis** for each individual tooth using dental panoramic radiographs. The model integrates:

- **Radiographic Bone Loss Detection**  
- **Cementoenamel Junction (CEJ) Identification**  
- **Tooth Numbering and Length Estimation**

The classification is based on the **2017 international criteria** for radiographic bone levels. The dataset used includes real patient images and annotations provided by **AIHub**, an open data platform in Korea.

## 📁 Dataset

The dataset used in this project comes from [AIHub](https://aihub.or.kr/) and includes:

- Dental panoramic X-ray images  
- Tooth annotations (numbering, length)  
- Bone loss and CEJ markers

> 📌 **Note**: You need to register on AIHub and agree to their terms of use to access the dataset.

## 🧠 Model Architecture

The system integrates multiple components:

- **Segmentation Model** (e.g., U-Net or YOLO-based) for detecting CEJ and bone loss  
- **Tooth Localization Module** for identifying individual teeth  
- **Classification Network** for predicting the stage (Stage I to IV)

## 🛠️ Installation

```bash
git clone https://github.com/DianaLee1219/periodontitis-AI.git
cd periodontitis-AI
pip install -r requirements.txt
