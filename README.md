# Smart Waste Classification and Recycling Assistant

This repository contains the implementation of a **Smart Waste Classification and Recycling Assistant** using deep learning and computer vision techniques.  
The project explores **data preprocessing, augmentation, CNNs, transfer learning, object detection (YOLO), GAN-based augmentation, and Autoencoding for denoising**.

---

## 📂 Repository Structure

- `1_Data_Preprocessing_and_Augmentation.ipynb`  
  - Data cleaning, resizing, normalization.  
  - Classical augmentation (rotation, flips, brightness, etc.).  

- `2_CNNs_and_TransferLearning.ipynb`  
  - Custom CNN (baseline).  
  - Transfer Learning with **ResNet, EfficientNet, MobileNet**.  
  - Model comparison and evaluation.  

- `3_YOLO_ObjectDetection.ipynb`  
  - YOLO-based detection model for localizing waste in images.  
  - Bounding box predictions.  

- `4_GANs_for_DataAugmentation.ipynb`  
  - GAN-based data augmentation for minority waste classes.  
  - Challenges due to data variability.  

- `5_Autoencoder_Denoising.ipynb`  
  - Autoencoder for noise removal and feature learning.  
  - Reconstruction performance using PSNR & SSIM.  

---

## 🚀 Project Pipeline

1. **Data Preprocessing** → Cleaning, balancing, augmentation.  
2. **Classification Models** → Custom CNN, ResNet, EfficientNet, MobileNet.  
3. **Detection Model** → YOLO for waste localization.  
4. **Data Augmentation** → GANs to enrich dataset diversity.  
5. **Autoencoding** → Noise reduction, better feature representation.  

---

## 📊 Results Overview

- **Custom CNN**: baseline, lower accuracy.  
- **ResNet & EfficientNe# Smart Waste Classification and Recycling Assistant

This repository contains the implementation of a **Smart Waste Classification and Recycling Assistant** using deep learning and computer vision techniques.  
The project explores **data preprocessing, augmentation, CNNs, transfer learning, object detection (YOLO), GAN-based augmentation, and Autoencoding for denoising**.

---


## 🛠️ Tech Stack

- Python, PyTorch, TensorFlow/Keras  
- OpenCV, Albumentations  
- YOLOv5/YOLOv8  
- Matplotlib, Seaborn  

---

## 📑 How to Use

1. Clone the repo:
   ```bash
   git clone https://github.com/yourusername/smart-waste-assistant.git
   cd smart-waste-assistant
t**: best performing, strong generalization.  
- **MobileNet**: lightweight, good trade-off between speed and accuracy.  
- **YOLO**: effective detection with bounding boxes.  
- **GANs**: generated realistic but variable-quality images, highlighting augmentation challenges.  
- **Autoencoder**: achieved denoising with **PSNR = 30.60 dB, SSIM = 0.8769**.  

