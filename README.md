# Diabetic Retinopathy Detection using Machine Learning

## What is Diabetic Retinopathy?
Diabetic Retinopathy (DR) is a severe complication of diabetes that affects the retina, leading to vision impairment or even blindness if not diagnosed and treated promptly. This project focuses on the early detection of DR using Machine Learning techniques, providing a highly accurate diagnosis with a success rate of 94%.


## Dataset
The project utilizes a dataset consisting of retinal images captured from diabetic patients. These images are used to train and evaluate the effectiveness of our machine learning models.

----



## Key Techniques and Preprocessing Steps

### Grayscale Conversion
Retinal images are converted from RGB (3 colour channels) to grayscale by taking a weighted average of the colour channels. This reduces the dimensionality of the data, optimizing storage and preprocessing requirements while retaining essential features for analysis.

### Histogram Equalization
We apply cumulative histogram equalization to enhance contrast in the grayscale images. This technique adjusts pixel intensities to stretch the dynamic range, resulting in an equalized image that highlights important features effectively.

### Discrete Wavelet Transform (DWT)
Images are divided into smaller components using wavelets—mathematical functions that analyze localized image regions. The Haar wavelet, in particular, helps with edge detection and localized information extraction, crucial for identifying diabetic retinopathy features.

### Gaussian Matching Filter
This filter is designed to match the patterns we are searching for. It accentuates specific patterns and structures in the images, further aiding the feature extraction process.

---

## Machine Learning Models
Two primary machine learning algorithms were employed to classify retinal images based on their dataset sizes:

### Support Vector Machine (SVM)
- **Used For**: Small datasets.
- **Working**: Finds the hyperplane with the maximum margin separating different classes of data points, making it ideal for high-accuracy classifications.

### K-Nearest Neighbors (KNN)
- **Used For**: Large datasets.
- **Working**: Assigns labels to test samples based on the majority label among its k-nearest neighbours in the feature space, leveraging simplicity and effectiveness for larger datasets.

---

## Accuracy
The methods implemented in this project achieved an impressive accuracy of **94%**, demonstrating their effectiveness in detecting diabetic retinopathy reliably.

---

## Conclusion
This project combines advanced image preprocessing techniques with machine learning algorithms to detect diabetic retinopathy efficiently. With its high accuracy, it holds potential as an assistive diagnostic tool in healthcare, ensuring timely and reliable detection of this severe condition.

