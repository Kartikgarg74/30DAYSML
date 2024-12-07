# Day 11: Machine Learning Feature Engineering

Welcome to Day 11 of the 30-Day Machine Learning series! In this session, we focus on **Feature Engineering**, an essential aspect of building efficient and accurate machine learning models. By the end of this day, you'll have a solid understanding of:

- Why feature engineering is crucial
- Types of feature transformations
- Common techniques for feature extraction and selection
- Hands-on examples using Python

---

## What is Feature Engineering?
Feature Engineering is the process of selecting, modifying, or creating new features from raw data to improve model performance. It bridges the gap between raw data and the most effective input representation for a machine learning algorithm.

---

## Key Concepts

### 1. Types of Features
- **Numerical Features**: Continuous or discrete numbers.
- **Categorical Features**: Fixed categories or labels.
- **Text Features**: Words, phrases, or sentences.
- **Temporal Features**: Time-related data like timestamps.
- **Geographical Features**: Spatial data like coordinates.

### 2. Common Feature Transformations
- **Scaling**: Adjusting feature values to a common scale (e.g., StandardScaler, MinMaxScaler).
- **Encoding**: Converting categorical variables into numerical format (e.g., One-Hot Encoding, Label Encoding).
- **Imputation**: Filling missing values using mean, median, or other techniques.
- **Polynomial Features**: Generating higher-order terms from numerical features.

---

## Techniques

### 1. Feature Selection
Reducing the number of features to eliminate redundancy and irrelevance:
- **Filter Methods**: Correlation, Chi-Square.
- **Wrapper Methods**: Recursive Feature Elimination (RFE).
- **Embedded Methods**: Feature importance from models like Random Forest.

### 2. Feature Extraction
Transforming raw data into informative features:
- **Principal Component Analysis (PCA)**
- **Latent Dirichlet Allocation (LDA)**
- **Word Embeddings**: Word2Vec, GloVe.

---

## Hands-On Example

### Import Libraries
```python
import pandas as pd
import numpy as np
from sklearn.preprocessing import StandardScaler, OneHotEncoder
from sklearn.impute import SimpleImputer
```

### Load Dataset
```python
data = pd.read_csv('sample_data.csv')
```

### Handling Missing Values
```python
imputer = SimpleImputer(strategy='mean')
data['column_name'] = imputer.fit_transform(data[['column_name']])
```

### Scaling Features
```python
scaler = StandardScaler()
data_scaled = scaler.fit_transform(data[['numerical_column']])
```

### Encoding Categorical Variables
```python
encoder = OneHotEncoder()
data_encoded = encoder.fit_transform(data[['categorical_column']])
```

---

## Best Practices
- **Understand Your Data**: Always explore your data before engineering features.
- **Avoid Data Leakage**: Ensure transformations are only based on training data.
- **Keep it Simple**: Start with straightforward transformations before moving to advanced techniques.

---

## Resources
- [Scikit-learn: Preprocessing Techniques](https://scikit-learn.org/stable/modules/preprocessing.html)
- [Kaggle Datasets for Practice](https://www.kaggle.com/datasets)

---

Stay tuned for Day 12, where we'll dive deeper into **Model Evaluation Techniques**!

Happy learning! 🚀
