# Brain Tumor Detection using Transfer Learning (VGG16)

## Project Overview
This project focuses on brain tumor detection from MRI images using deep learning. We applied transfer learning on top of the pretrained VGG16 model to classify MRI scans into tumor and non-tumor categories. The goal is to build an accurate, efficient, and interpretable model that can assist in early diagnosis. 

---
## Model Architecture 
- **Base Model:** VGG16 pretrained on ImageNet
- **Transfer Learning:** Convolutional layers frozen; custom dense layers added for classification
- **Input Size:** Images resized to 128×128 pixels
- **Output:** classification (Glioma, Meningioma, Pituitary tumor, No tumor)
- **Optimizer:** Adam with categorical cross-entropy loss

---
## Dataset
We used the **Brain Tumor MRI Dataset** from Kaggle, containing MRI images. [Link](https://www.kaggle.com/datasets/masoudnickparvar/brain-tumor-mri-dataset) <br>
The dataset contains 7,200 human brain MRI images categorized into four classes:
- Glioma
- Meningioma
- Pituitary tumor
- No tumor <br>
The dataset is structured into training and testing sets with balanced class distributions.

---
## Sample MRI images from the dataset
<img width="4658" height="3543" alt="mri_image_samples" src="https://github.com/user-attachments/assets/1aaacf2f-e11a-419e-b09f-ee19c4ab6e7c" />

---
## Results & Evaluation 
### Model Classification Report
<img width="578" height="264" alt="image" src="https://github.com/user-attachments/assets/29084550-8258-4e2f-b104-9713cb67275d" />

### Confusion Matrix 
We plotted a confusion matrix to evaluate classification performance. 
- Diagonal cells represent correct predictions
- Off-diagonal cells highlight misclassifications
<img width="2698" height="2347" alt="confusion_matrix" src="https://github.com/user-attachments/assets/71d56c74-c3f6-4cf7-a6f8-6900a38cf721" />

---
### Sample Predictions 
We visualized random test images with their **true labels vs. predicted labels** to qualitatively assess model performance.

<img width="5970" height="1411" alt="prediction" src="https://github.com/user-attachments/assets/bb991b73-e85b-4b97-87c7-352382f0cfd6" />

