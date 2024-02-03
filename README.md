Accelerometer Data Feature Extraction and Classification

This Jupyter notebook aims to leverage accelerometer data for activity classification, employing feature extraction techniques and the k-nearest neighbors (KNN) algorithm. The dataset contains accelerometer readings and corresponding activity labels. Here's a concise overview of the notebook's key sections:

Key Sections:
1. Data Loading:
Accelerometer data, both training, and testing sets are loaded from files (total_acc_x_train.txt, total_acc_x_test.txt, y_train.txt, and y_test.txt).

2. Preprocessing:
Two scaling techniques, Min-Max Scaler and Standard Scaler, are applied to normalize both time and frequency domain signals.

3. Feature Extraction:
Fast Fourier Transform (FFT) is utilized to extract frequency domain features from accelerometer data.
Features include average, variance, standard deviation, median absolute deviation, maximum, minimum, signal magnitude area, and energy measure.

4. Feature Selection:
Various techniques, such as SelectKBest and SelectPercentile with chi-squared tests, are explored for optimizing the dataset.

5. K-Nearest Neighbors (KNN) Classification:
The KNN algorithm is employed for activity classification based on the extracted features.
Visualizations depict accuracy scores for different parameter values.
