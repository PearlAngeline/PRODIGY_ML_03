🐶🐱 Cats vs Dogs Classification using SVM
PRODIGY_ML_03 – Machine Learning Internship Task

This project implements a Support Vector Machine (SVM) classifier to distinguish between images of cats and dogs using the Kaggle “Dogs vs Cats” dataset.

Although SVMs are not typically used for high-resolution image classification, this task demonstrates how traditional ML models behave on visual data by converting images into feature vectors.

📌 Objective

To build an SVM model capable of classifying images of cats and dogs based on pixel features.

📂 Dataset

Kaggle Dataset:
🔗 https://www.kaggle.com/c/dogs-vs-cats/data

Contains 25,000 labeled images (cat & dog)

Only the train folder is needed

Images are resized to 128×128 and flattened into vectors for SVM

🧠 Steps Performed
✔ 1. Data Loading

Loaded image files from the Kaggle dataset.

✔ 2. Image Preprocessing

Converted images to RGB

Resized them to 128 × 128

Flattened them into 1D arrays (16384 features)

Assigned labels → Cat = 0, Dog = 1

✔ 3. Splitting the Dataset

80% Training

20% Testing

✔ 4. Model Training

Used SVM with Linear Kernel for binary classification.

✔ 5. Model Evaluation

Used:

Accuracy Score

Classification Report

Precision, Recall, F1-score

🛠 Technologies Used

Python

OpenCV

NumPy

Scikit-learn

🧪 Code Snippet (Training SVM)
model = SVC(kernel="linear")
model.fit(X_train, y_train)

y_pred = model.predict(X_test)

📊 Expected Accuracy

SVM on raw pixel features typically gives:

➡️ 60%–70% accuracy
(depending on hardware, image size, and preprocessing)

📁 Files in This Repository

svm_cats_dogs.ipynb – Full implementation

README.md – Project documentation

Sample images (optional)

👩‍💻 Author

Pearl Angeline
Machine Learning Intern – PRODIGY InfoTech
GitHub: https://github.com/PearlAngeline

🎯 Conclusion

This project demonstrates the challenges of applying traditional machine learning (SVM) to image classification tasks. It provides a strong understanding of:

Image preprocessing

Feature vector creation

Binary classification using SVM