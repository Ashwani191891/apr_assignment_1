# apr_assignment_1


1. Introduction
The Iris dataset is one of the most widely used datasets in machine learning and pattern recognition. It contains measurements of iris flowers belonging to three species: Setosa, Versicolor, and Virginica.
The goal of this assignment is to build a classification model to predict the species of an iris flower based on its features.
In this assignment, I used Linear Discriminant Analysis (LDA) for dimensionality reduction and Gaussian Naïve Bayes for classification. The motivation for using this combination is:
• LDA reduces feature dimensions while maximizing class separability.
• Naïve Bayes is simple, efficient, and effective for classification tasks.
• Together, they provide a robust pipeline for multi-class classification.


2. Dataset Description
The Iris dataset has the following properties:
• Total samples: 150
• Features: 4 (Sepal Length, Sepal Width, Petal Length, Petal Width)
• Classes: 3 (Setosa, Versicolor, Virginica)
• Samples per class: 50 (balanced dataset)
• Data type: Continuous numerical features


3. Methodology
   
3.1 Preprocessing
• Standardized features using StandardScaler.
• Train-test split performed (80% training, 20% testing).
• No missing values or categorical encoding required as dataset is clean.

3.2 Dimensionality Reduction (LDA)
• LDA finds linear combinations of features that best separate classes.
• Reduces data from 4D to 2D for better visualization and reduced complexity.
• Maintains maximum class separability.
• Helps avoid overfitting and improves interpretability.

3.3 Classification (Naïve Bayes)
• Gaussian Naïve Bayes is used as the classifier.
• Works well with continuous data assuming Gaussian distribution.
• Provides class probabilities, making it useful for probabilistic interpretation.
• Fast and computationally efficient.


4. Implementation and Results

Install numpy, matplotlib, seaborn, sklearn modules in python and then run the given code.

The evaluation of the Naïve Bayes classifier on LDA-transformed features gives the following results:
• Accuracy: 98%
• Precision, Recall, and F1-Score are close to 1.0 for Setosa.
• A few misclassifications occur between Versicolor and Virginica.
• Confusion Matrix indicates strong performance overall.


6. Conclusions
• The combination of LDA and Naïve Bayes is highly effective for the Iris dataset.
• LDA helped in reducing dimensions while preserving class separability.
• Naïve Bayes performed well despite its strong independence assumptions.
• Misclassifications are due to overlapping features of Versicolor and Virginica.
• The model is lightweight and efficient, making it suitable for real-time applications.
