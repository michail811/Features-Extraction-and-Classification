Accelerometer Data Feature Extraction and Classification (X-Axis Only)

This Jupyter notebook focuses on feature extraction and classification using accelerometer data, specifically from the X-axis. The dataset includes readings from the X-axis for both training and testing sets, along with corresponding activity labels. The primary challenge lies in classifying activities based solely on X-axis data. Here's an enhanced overview:

Key Sections:
1. Data Loading:
Accelerometer data from the X-axis is loaded from files (total_acc_x_train.txt and total_acc_x_test.txt).

2. Preprocessing:
Two scaling techniques, Min-Max Scaler and Standard Scaler, are applied to normalize X-axis signals.

3. Feature Extraction:
Fast Fourier Transform (FFT) is utilized to extract frequency domain features from X-axis accelerometer data.
Extracted features include average, variance, standard deviation, median absolute deviation, maximum, minimum, signal magnitude area, and energy measure.

4. Feature Selection:
Various techniques, such as SelectKBest and SelectPercentile with chi-squared tests, are explored to optimize the dataset.

5. K-Nearest Neighbors (KNN) Classification:
The KNN algorithm is employed for activity classification based on features derived solely from the X-axis.
Visualizations illustrate accuracy scores for different parameter values.

Challenge:
The exclusive use of X-axis accelerometer data poses a unique challenge, requiring the model to accurately classify activities based on this limited information.
