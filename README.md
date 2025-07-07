# Skin_Cancer_Lesion_Classification

📁 Dataset
Source: Kaggle dataset fanconic/skin-cancer-malignant-vs-benign

Structure:

/data/train/malignant/

/data/train/benign/

📌 Notebook Overview
1. Data Import
Downloads and unpacks dataset using kagglehub.

2. Preprocessing
Image segmentation techniques applied:

Otsu thresholding

Histogram equalization

Mean filter

Hole filling

Includes helper functions for visualization and manipulation of RGB layers.

3. Segmentation & Clustering
Applies K-Means clustering to segment skin lesions from background.

Uses elbow method to determine the optimal number of clusters.

4. Region of Interest (ROI) Extraction
Masks and merges segmented images to isolate relevant lesion areas.

🛠 Technologies Used
Python (NumPy, Matplotlib, SciPy, Scikit-learn)

Image processing: skimage, scipy.ndimage

Clustering: KMeans from sklearn.cluster

📊 Notes
The notebook focuses more on segmentation and visualization than on full CNN-based classification.

No deep learning model (e.g., CNN) is trained; the approach is mostly unsupervised and exploratory.


Open the notebook on Colab and run.
