# Deepfake Detection Project
Welcome to the Deepfake Detection Project repository. This project focuses on the detection of deepfakes using multiple machine learning and deep learning models, which have been trained on different datasets. Additionally, a comparison of these models has been performed on a test dataset that combines both altered and real images to evaluate their accuracies.


# Mesonet for Deepfake Detection

Utilizes the Mesonet architecture for deepfake detection, a model known for its effectiveness in discerning manipulated content. The model has been meticulously trained on the Deepfakes dataset which combines 7104 images (you can download it from kaggle), a comprehensive dataset that encompasses a diverse array of altered and real images of individuals captured under varying conditions of illumination, sharpness, and other relevant factors.
Accuracy: 0.89 
This image fake labeled 0, was predicted as fake using Mesonet as it's shown with the predicted likelihood (0.0077) which is so near to 0 (the actual label). 
![image](https://github.com/nourhenehanana/deepfakes_detection_DL_ML/assets/93352403/136d7102-fd4c-467e-8d80-3d8c3ffb2b40)
![git9](https://github.com/nourhenehanana/deepfakes_detection_DL_ML/assets/93352403/a447f289-1ee2-4eec-a41d-0dc09d7051ae)

# Xception with Transfer Learning

Leverages the Xception model, augmented with transfer learning techniques, to facilitate the detection of deepfakes. This model has undergone rigorous training on the DeepFake Detection Challenge (DFDC) dataset, a compilation of 5,639 video sequences that were meticulously subdivided into individual frames for the purpose of modeling and analysis.
Accuracy: 0.85
![git10](https://github.com/nourhenehanana/deepfakes_detection_DL_ML/assets/93352403/1789218d-f4e8-459c-a325-2bcacf453499)


# Logistic Regression (LR) and Support Vector Machine (SVM)
Applies logistic regression and support vector machine (SVM) models as robust tools for the purpose of deepfake detection. These models have been rigorously trained on the Faces HQ dataset, an extensive compilation of 40,000 images sourced from a combination of four distinct datasets, namely CelebA, Flickr-Faces-HQ, 100K faces, and thispersondoesnotexist. This amalgamation of datasets ensures a comprehensive and diverse training set for the models.
Logistic Regression: 1.0
SVM: 1.0
![git11](https://github.com/nourhenehanana/deepfakes_detection_DL_ML/assets/93352403/010f9eb7-c390-4404-aad6-6421550f43fa)

# Test Dataset
A test dataset has been manually created, combining altered (deepfake) and real images. This dataset is designed to assess the performance and accuracy of the various models in detecting deepfakes and image manipulations. The dataset covers 2000 images that were labeled manually by their grounded truth 0 when the image is fake and 1 when the image is real.
![git12](https://github.com/nourhenehanana/deepfakes_detection_DL_ML/assets/93352403/aeb2ffa2-e4cd-4fb5-a303-8e0caf46b77c)
Then we test the previous models and calculate their accuracies as seen in the script deepfakes_detection_test. 

Getting Started
To get started with this project, follow these steps:

Install Dependencies: Ensure you have the required Python libraries and deep learning frameworks installed, such as TensorFlow, Keras, scikit-learn, pandas and matplotlib.
Extract the data from kaggle or github.
Train the Models: Train the deep learning models (Mesonet and Xception) using their respective datasets (Deepfakes and DFDC), and the machine learning models (LR and SVM) using the Faces HQ dataset.
Evaluate Model Performance: Run the evaluation scripts to assess the accuracy and performance of each model on the manually created test dataset that combines altered and real images.
Compare Results: Compare the accuracies and outcomes of the different models to understand their respective capabilities in detecting deepfakes and image manipulations.


