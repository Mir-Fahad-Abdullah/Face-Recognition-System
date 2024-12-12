# Project Name: Face Recognition System
## Group Members :

| Name | ID | NSU Email |
| --- | --- | --- |
| Mir Fahad Abdullah | 2121572642 | fahad.abdullah@northsouth.edu |
| Sairat Jamin Shefa | 2122172042 | shirat.shefa@northsouth.edu |


## **Introduction:**
Emotion detection using facial recognition technology is a rapidly advancing field within computer vision and artificial intelligence. It aims to analyze facial expressions in real-time to determine the emotional state of an individual. This technology has a wide range of applications, including in human-computer interaction, security systems, personalized marketing, and mental health monitoring.

Facial emotion detection typically involves two main stages: face detection and emotion classification. Face detection identifies the presence of a face in an image, while emotion classification determines the emotion displayed based on predefined categories (e.g., happy, sad, angry, neutral, etc.). Machine learning algorithms, combined with powerful libraries like OpenCV, scikit-learn, and advanced techniques such as PCA (Principal Component Analysis) and HOG (Histogram of Oriented Gradients), are commonly used to build emotion detection systems.

### Methodologies for Building the Emotion Detection System

1. **Libraries and Tools:**
   - **OpenCV:** OpenCV (Open Source Computer Vision Library) is a powerful library used for real-time computer vision applications. It provides tools for image processing, such as face detection, feature extraction, and image transformations.
   - **Scikit-learn:** Scikit-learn (sklearn) is a widely used library for machine learning in Python. It provides tools for feature scaling, classification models (e.g., SVC), and dimensionality reduction techniques like PCA.
   - **Jupyter Notebook:** Jupyter Notebook is an interactive web-based environment for running and sharing Python code. It's ideal for prototyping, visualization, and iterative testing when building machine learning models.

2. **Feature Extraction:**
   - **Histogram of Oriented Gradients (HOG):** HOG is a feature descriptor used to capture the shape of objects, such as faces. It works by dividing an image into small cells, computing the gradient directions in each cell, and using the orientation histogram to capture structural information. This helps in recognizing various facial features and expressions.
  
   ![Face-detection-using-HoG-features-designed-by-Felzenszwalb-et-al-2010](https://github.com/user-attachments/assets/3ee7df5a-a3a5-4ccf-8232-4d3c1b5f0ae2)


   - **Principal Component Analysis (PCA):** PCA is a dimensionality reduction technique that transforms high-dimensional data into a smaller set of variables (principal components). In facial emotion detection, PCA can be used to reduce the complexity of face data by identifying the most important features, making the model more efficient.

3. **Data Preprocessing and Feature Scaling:**
   - **Feature Scaling:** This step involves normalizing or standardizing the feature values to ensure they are on a similar scale. This is important for models like SVC, where features on different scales can adversely affect the model's performance. Common techniques include Min-Max scaling and Standardization (z-score normalization).
   
   - **Face Detection:** OpenCV provides tools to detect faces in an image using methods like Haar cascades or deep learning-based detectors. Once the face is identified, the relevant features can be extracted.

4. **Model Training (Support Vector Classifier - SVC):**
   - **Support Vector Classifier (SVC):** SVC is a supervised machine learning algorithm that works by finding the optimal hyperplane that separates data points of different classes in a higher-dimensional space. For emotion detection, SVC can classify the extracted features (such as HOG and PCA) into different emotion categories. It is highly effective in scenarios where the classes are well-defined and the data is separable.


### Summary of Key Components:
- **OpenCV**: For face detection and image processing.
- **Scikit-learn (sklearn)**: For feature scaling, PCA, and training models like SVC.
- **Jupyter Notebook**: For developing and testing the model interactively.
- **HOG**: To capture facial features from images.
- **PCA**: For dimensionality reduction and feature selection.
- **SVC**: For classification of emotions based on the extracted features.
