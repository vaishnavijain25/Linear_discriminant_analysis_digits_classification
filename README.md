# Dimensionality Reduction and Classification using LDA on Digits Dataset

## Overview  
This project uses **Linear Discriminant Analysis (LDA)** to reduce the number of features in the handwritten digits dataset. The original 64 features are reduced to 9 while preserving important class information. Then, a **Random Forest Classifier** is trained on these reduced features to identify digits from 0 to 9.

## Dataset  
- The digits dataset from scikit-learn  
- 1797 samples of handwritten digits  
- Each sample has 64 features (8x8 pixel images)  
- 10 classes (digits 0 through 9)

## Approach  
- Features are scaled with **StandardScaler**  
- LDA reduces features to 9 components (number of classes minus one)  
- Random Forest model is trained on the LDA-transformed data  
- Model tested on unseen data to check accuracy

## Results  
- The model achieved about **95.5% accuracy** even after feature reduction  
- The 9 LDA components explain almost all the differences between classes  
- 2D and 3D plots show clear separation of digit classes

## Conclusion  
Using LDA helps simplify the data while retaining important class differences. This makes the Random Forest classifier faster and still very accurate.
