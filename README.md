
---

# Smart Waste Classification and Recycling Assistant

This project implements a **Smart Waste Classification and Recycling Assistant** using **deep learning and computer vision** techniques. It explores multiple approaches—ranging from **data preprocessing and augmentation** to **CNNs, transfer learning, object detection (YOLO), GAN-based augmentation, and autoencoders**—to build a robust waste classification system that supports **sustainability and recycling initiatives**.

---

## 📌 Project Description

Improper waste sorting is a global environmental challenge. Manual sorting is often **inefficient, error-prone, and labor-intensive**. This project leverages **AI-powered computer vision models** to automatically detect, classify, and denoise waste images, forming the foundation for **smart bins, recycling plants, and municipal services**.

The work is based on the **TrashNet dataset**, which contains images of six waste categories:

* **Cardboard**
* **Glass**
* **Metal**
* **Paper**
* **Plastic**
* **Trash**

---

## 🛠️ Project Pipeline

1. **Data Preprocessing & Augmentation**

   * Cleaning, resizing, normalization.
   * Classical augmentation (rotation, flips, brightness, contrast, cropping).

2. **CNNs & Transfer Learning**

   * Baseline CNN model as a starting point.
   * Transfer learning with **ResNet50, EfficientNetB1, MobileNetV3Small**.
   * Achieved best accuracy with **EfficientNetB1 (\~88% validation, \~85% test)**.

3. **YOLOv8 Object Detection**

   * Real-time waste localization with bounding boxes.
   * Precision: **0.919**, Recall: **0.926**, mAP: **>97%**.
   * Strongest results for **paper, cardboard, glass**.

4. **GANs for Data Augmentation**

   * Generated synthetic images for minority classes.
   * Faced challenges with instability and noisy outputs.
   * Highlighted trade-offs between **quality and diversity**.

5. **Autoencoder for Image Denoising**

   * Encoder–Decoder architecture for removing Gaussian noise.
   * Achieved **PSNR = 30.60 dB** and **SSIM = 0.8769**, producing cleaner reconstructions.

---

## 📊 Results Overview

* **Custom CNN:** 58% validation accuracy → limited baseline.
* **ResNet50 & VGG16:** Solid improvements, up to \~85%.
* **EfficientNetB1:** Best overall accuracy and efficiency.
* **MobileNetV3Small:** Good trade-off for mobile deployment.
* **YOLOv8:** High detection accuracy and real-time inference.
* **GANs:** Generated realistic but unstable synthetic samples.
* **Autoencoder:** Effective denoising with strong reconstruction metrics.

---

## 🌍 Ethical & Societal Impact

* **Supports UN SDGs:**

  * SDG 11: Sustainable Cities & Communities.
  * SDG 12: Responsible Consumption & Production.
  * SDG 13: Climate Action.
* **Benefits:** Improved recycling efficiency, cost savings, public awareness, cleaner environments.
* **Challenges:** Dataset bias (clean images vs real-world waste), energy cost of training models, global accessibility.
* **Applications:** Smart bins, recycling plants, municipal waste services, and corporate sustainability programs.

---

## 📑 Repository Structure

* `1_Data_Preprocessing_and_Augmentation.ipynb` → Cleaning, resizing, normalization, classical augmentation.
* `2_CNNs_and_TransferLearning.ipynb` → Baseline CNN + Transfer Learning with ResNet, EfficientNet, MobileNet, VGG16.
* `3_YOLO_ObjectDetection.ipynb` → YOLOv8 implementation for detection and localization.
* `4_GANs_for_DataAugmentation.ipynb` → GAN-based augmentation for underrepresented classes.
* `5_Autoencoder_Denoising.ipynb` → Autoencoder for denoising and feature representation.

---

## 🛠️ Tech Stack

* **Languages:** Python
* **Frameworks:** TensorFlow/Keras, PyTorch
* **Computer Vision:** OpenCV, Albumentations
* **Detection Models:** YOLOv5 / YOLOv8
* **Visualization:** Matplotlib, Seaborn

---

## 🚀 How to Use

```bash
# Clone the repository  
git clone https://github.com/habibahelal/Smart-Waste-Classification-and-Recycling-Assistant 
cd smart-waste-assistant  

# Install dependencies  
pip install -r requirements.txt  

# Run notebooks in order for preprocessing, training, and evaluation  
```

## 📑 Documentation & Presentation  

For full project documentation and visualization, the following files are included in this repository:  

- **Final Report (PDF):** Detailed explanation of methodology, experiments, results, ethical & societal impact.  
- **PowerPoint Presentation (PPTX):** Summarized slides with visualizations,GIFs, results, and key findings for presentation purposes.  

  


Would you like me to also create a **shorter presentation-style README (like a 1-page portfolio showcase)**, alongside this detailed one, so you can use one for GitHub and one for presenting to evaluators?
