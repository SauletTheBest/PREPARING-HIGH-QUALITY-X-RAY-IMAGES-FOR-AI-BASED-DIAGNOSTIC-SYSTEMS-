# Preparing High-Quality X-ray Images for AI-based Diagnostic System

**Course:** Research Methods and Tools (SE-2307)
**Team:** Saulet Kabdrakhmanov, Galymzhan Aliakbar, Aruzhan Atelova, Bekzhan Nurallin.

## 📌 Project Overview
This repository documents the entire research process for improving chest X-ray image quality to enhance AI diagnostic performance. We investigate how preprocessing techniques (CLAHE, Gaussian Blur, Normalization) affect image consistency and clarity.

## 🎯 Research Aim
To improve the quality and consistency of chest X-ray images used in AI-based diagnostic systems through the evaluation of preprocessing techniques and the development of a standardized image preparation pipeline.

## 📂 Repository Structure
* `docs/`: Contains all research reports, methodology chapters, and drafts.
* `instruments/`: Interview scripts, survey forms, and data collection tools.
* `notebooks/`: Python code (Jupyter/Colab) for the preprocessing pipeline.
* `process/`: Project grahps and feedback logs.
* `image/`: Sample images.
* `model`: Containts trained models(effientNetB0, mobileNetV2) that we are used.

## 🛠 Methodology & Tools
We utilize a Python-based pipeline involving:
1. **Resizing** (224x224)
2. **Grayscale Conversion**
3. **Noise Reduction** (Bilateral Filter)
4. **Contrast Enhancement** (CLAHE)
5. **Quality Verification** (SSIM, Brightness Mean)

**Libraries:** OpenCV, NumPy, Matplotlib, scikit-image.

## 🚀 How to Reproduce
1. Download mannually notebook.
2. Open `notebooks/xray.ipynb`. You might though Google Colab.
4. Download datasets ([LINK TAP TAP](https://www.kaggle.com/datasets/tawsifurrahman/covid19-radiography-database?)), upload to your google disk and upload to your RAM memory(google colab) update the path in the notebook.
5. Run all cells to see the transformation from Raw to Enhanced images.

## 📊 Key Results
Preliminary results show an improvement in visual clarity for lung structures.
* **Average SSIM:** ~0.87 (indicating structural integrity is preserved)
* **Brightness:** Normalized to range [100-160]

## 🖼️ Example of pictures of our pipline
![figure 1](image/results1.png)
![figure 2](image/results2.png)
![figure 3](image/results3.png)
![figure 4](image/results4.png)

## 🖌️ Graphs (example of mobileNETV2) 
![graph](progress/graph1.png)
you can also check other pictures!


---
*This project is part of the academic curriculum at Astana IT University.*
