Handwritten Digit Recognition using KNN & PCA
📌 Overview

This project implements a handwritten digit recognition system using the MNIST Digit Recognizer dataset from Kaggle.
The model uses K-Nearest Neighbors (KNN) for classification and Principal Component Analysis (PCA) for dimensionality reduction and visualization.

📂 Dataset

Source: Kaggle – Digit Recognizer (MNIST)

Samples: 42,000

Features: 784 pixel values (28×28 images)

Target: Digit labels (0–9)

Files:

train.csv

test.csv

sample_submission.csv

🛠 Tech Stack

Python

NumPy

Pandas

Matplotlib

Plotly

Scikit-learn

⚙️ Project Workflow
1. Data Exploration

Loaded dataset using Pandas

Visualized handwritten digits using Matplotlib

Confirmed dataset shape (42000, 785)

2. Preprocessing

Feature–label separation

Train–test split (80:20)

Standardization using StandardScaler

3. KNN Classification

Applied KNN on original 784-dimensional data

Achieved ~96.48% accuracy

Observed high computation time

4. PCA + KNN

Reduced dimensions using PCA

Optimal performance around 200 components

Accuracy after PCA: ~95%

Faster predictions and reduced complexity

5. Visualization

2D PCA scatter plot for class separation

3D PCA visualization for better cluster understanding

Explained variance and cumulative variance plots

📊 Results
Model	Dimensions	Accuracy
KNN (No PCA)	784	96.48%
KNN + PCA	200	~95%
📈 Explained Variance

PCA eigenvalues analyzed

Cumulative variance used to determine optimal components

Demonstrates trade-off between accuracy and dimensionality

🚀 Future Enhancements

Implement CNN for higher accuracy

Hyperparameter tuning of KNN

Try t-SNE / UMAP for visualization

Deploy using Streamlit / Flask

▶️ How to Run
pip install numpy pandas matplotlib plotly scikit-learn

python main.py


(Or run the notebook in Kaggle/Jupyter)

👩‍💻 Author

Srishti Kumari
Third-Year Data Science Student
📍 India
