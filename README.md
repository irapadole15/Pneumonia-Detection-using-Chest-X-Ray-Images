# Pneumonia Detection using Chest X-Ray Images

## Problem Statement

**Build a binary classifier to detect pneumonia using chest x-rays.**

### Pneumonia
> Pneumonia is an infection that inflames the air sacs in one or both lungs. The air sacs may fill with fluid or pus (purulent material), causing cough with phlegm or pus, fever, chills, and difficulty breathing. A variety of organisms, including bacteria, viruses and fungi, can cause pneumonia.  Chest X-ray, blood tests, and culture of the sputum may help confirm the diagnosis. The disease may be classified by where it was acquired, such as community- or hospital-acquired or healthcare-associated pneumonia.

## Dataset description

> The dataset is organized into 3 folders (train, test, val) and contains subfolders for each image category (Pneumonia/Normal). There are 5,863 X-Ray images (JPEG) and 2 categories (Pneumonia/Normal).
Chest X-ray images (anterior-posterior) were selected from retrospective cohorts of pediatric patients of one to five years old from Guangzhou Women and Children’s Medical Center, Guangzhou. All chest X-ray imaging was performed as part of patients’ routine clinical care. For the analysis of chest x-ray images, all chest radiographs were initially screened for quality control by removing all low quality or unreadable scans. The diagnoses for the images were then graded by two expert physicians before being cleared for training the AI system. In order to account for any grading errors, the evaluation set was also checked by a third expert.

<img width="700" height="350" alt="cor_pred" src="https://github.com/user-attachments/assets/e84e7a19-22fa-4152-b87f-5120cefd74d7" />


## Model used :
**Here is a small comparison of all the models tested in the project:**

<img width="700" height="350" alt="comparison" src="https://github.com/user-attachments/assets/99281116-2b72-40a0-82ca-a0fd2acb8303" />


- ### Convolutional Neural Network

<img width="700" height="350" alt="cnn" src="https://github.com/user-attachments/assets/30bea36f-77d3-4cd5-9965-d88356f59327" />


```
624/624 [==============================] - 11s 18ms/step
Loss of the model is -  0.30433156475042683
624/624 [==============================] - 10s 15ms/step
Accuracy of the model is -  91.98718070983887 %
```
<img width="700" height="350" alt="Screenshot 2026-01-04 192406" src="https://github.com/user-attachments/assets/40f33928-3b63-4d52-919a-9762c000d5e7" />


- ### Convolutional Neural Network(Different approach) :

<img width="700" height="350" alt="accuracy_cnn_2" src="https://github.com/user-attachments/assets/fb14ae4a-db4e-4545-8f9c-ecec7c1e1349" />


```
624/624 [==============================] - 30s 49ms/step
Test Accuracy: 68.91%
652/652 [==============================] - 338s 518ms/step
Train Accuracy: 66.33%
```

- ### DenseNet :

<img width="700" height="350" alt="densenet" src="https://github.com/user-attachments/assets/1e1bd69d-7753-4762-9c4e-f0f2ae500ada" />

<img width="700" height="350" alt="densenetperf" src="https://github.com/user-attachments/assets/2eeb1eec-b23e-4c0a-99cd-37214751776c" />


```
624/624 [==============================] - 132s 211ms/step
Test Accuracy: 87.18%
652/652 [==============================] - 622s 954ms/step
Train Accuracy: 86.22%
```

- ### VGG16 :

<img width="700" height="350" alt="Screenshot 2026-01-04 192723" src="https://github.com/user-attachments/assets/0088b544-a7ec-4c7f-b110-469b2c469fd9" />

<img width="700" height="350" alt="Screenshot 2026-01-04 192825" src="https://github.com/user-attachments/assets/c2dda4ee-a9c3-42fd-8588-c5f461eba8cb" />


```
624/624 [==============================] - 226s 363ms/step
Test Accuracy: 66.19%
652/652 [==============================] - 1608s 2s/step
Train Accuracy: 82.63%
```


- ### ResNet :
  
<img width="700" height="350" alt="Screenshot 2026-01-04 192912" src="https://github.com/user-attachments/assets/d28da2d7-75ca-4471-9a5b-e2909af474d9" />

```
624/624 [==============================] - 101s 162ms/step
Test Accuracy: 73.40%
652/652 [==============================] - 651s 999ms/step
Train Accuracy: 88.92%
```

- ### InceptionNet :

<img width="700" height="350" alt="Screenshot 2026-01-04 193017" src="https://github.com/user-attachments/assets/02854251-29ba-43e9-917f-a82e20d7a86d" />


```
624/624 [==============================] - 41s 66ms/step
Test Accuracy: 76.76%
652/652 [==============================] - 295s 453ms/step
Train Accuracy: 91.26%
```


