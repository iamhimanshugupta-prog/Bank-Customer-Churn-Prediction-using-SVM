# 🏦 Bank Customer Churn Prediction Using Support Vector Machine (SVM)

## 📌 About the Project

Customer churn is one of the important challenges faced by banks and other financial institutions. It refers to customers leaving a bank or stopping the use of its services.

The objective of this project is to develop a Machine Learning model that can predict whether a bank customer is likely to leave the bank based on their personal and banking-related information.

This project uses **Support Vector Machine (SVM)**, a supervised Machine Learning algorithm, to perform binary classification.

But this project is not only about predicting customer churn. It is also a practical learning project designed to understand important Machine Learning concepts, especially how SVM works, how different kernels behave, how hyperparameters affect model performance, and how to evaluate a classification model.

## 🎯 Project Objectives

- Predict whether a bank customer will churn or stay.
- Explore customer data using Exploratory Data Analysis (EDA).
- Understand the importance of data preprocessing in Machine Learning.
- Learn how Support Vector Machine works in a real-world classification problem.
- Compare different SVM kernels: Linear, RBF, Polynomial, and Sigmoid.
- Understand how hyperparameters such as C and Gamma affect model performance.
- Evaluate the model using different classification metrics.

## 🧠 What I Learned from This Project

One of the main goals of this project was to understand Machine Learning concepts practically rather than only learning their theoretical definitions.

### 1. Understanding Support Vector Machine (SVM)

Through this project, I explored how SVM works as a supervised classification algorithm.

Some important concepts I learned:

- **Hyperplane:** The decision boundary that separates different classes.
- **Margin:** The distance between the decision boundary and the closest data points.
- **Support Vectors:** The data points closest to the decision boundary that influence its position.
- **Kernel Trick:** A technique that helps SVM handle non-linear relationships between data points.

### 2. Understanding Different SVM Kernels

I experimented with four different kernels to understand how SVM handles different types of relationships in data.

| Kernel | What I Learned |
|---|---|
| Linear | Works with linear decision boundaries. |
| RBF | Can capture complex non-linear patterns. |
| Polynomial | Captures relationships using polynomial transformations. |
| Sigmoid | Uses a sigmoid-based kernel function. |

Comparing these kernels helped me understand why selecting the right kernel matters for a classification problem.

### 3. Understanding Hyperparameters

I also explored how hyperparameters influence the performance of an SVM model.

**C Parameter**
- Controls the penalty for classification errors.
- A smaller C allows more errors and generally favours a wider margin.
- A larger C penalizes errors more strongly.

**Gamma Parameter**
- Controls the influence of individual training points in the RBF kernel.
- Lower gamma generally produces smoother decision boundaries.
- Higher gamma can create more complex decision boundaries.

I tested different combinations of C and Gamma to identify a suitable configuration.

### 4. Other Machine Learning Concepts

During this project, I also practised:

- Exploratory Data Analysis (EDA)
- Handling numerical and categorical features
- One-Hot Encoding
- Feature Scaling using StandardScaler
- Training, validation, and testing datasets
- Avoiding data leakage during preprocessing
- Model comparison and hyperparameter tuning
- Confusion Matrix
- Precision, Recall, F1 Score, and Accuracy
- ROC Curve and ROC-AUC Score
- Precision-Recall Curve and Average Precision

## ⚙️ Project Workflow

The project follows these major steps:

1. **Data Loading and Inspection:** Load the dataset and understand its structure, features, data types, and missing values.
2. **Exploratory Data Analysis:** Explore customer behaviour using count plots, histograms, boxplots, and a correlation heatmap.
3. **Feature Selection:** Separate input features from the target variable and remove the customer ID because it is only an identifier.
4. **Data Splitting:** Divide the dataset into training (60%), validation (20%), and testing (20%) sets.
5. **Data Preprocessing:** Apply One-Hot Encoding to categorical features and StandardScaler to numerical features.
6. **Kernel Comparison:** Train and compare Linear, RBF, Polynomial, and Sigmoid SVM kernels.
7. **Hyperparameter Tuning:** Experiment with different C and Gamma combinations for the RBF kernel.
8. **Final Model Evaluation:** Evaluate the selected model on the unseen test dataset.
9. **Performance Visualization:** Use a Confusion Matrix, ROC Curve, and Precision-Recall Curve to understand model performance.

## 📊 Model Performance

After comparing four SVM kernels and experimenting with different hyperparameter combinations, the selected configuration was:

| Parameter | Selected Value |
|---|---|
| Algorithm | Support Vector Machine |
| Kernel | RBF |
| C | 1.0 |
| Gamma | auto |
| Class Weight | balanced |

### Final Test Results

The final model was evaluated on the unseen test dataset.

| Evaluation Metric | Score |
|---|---:|
| Accuracy | 79.30% |
| Precision (Churn) | 50% |
| Recall (Churn) | 78% |
| F1 Score (Churn) | 61% |
| ROC-AUC Score | 0.8619 |
| Average Precision | 0.6872 |

### What Do These Results Tell Us?

- **Accuracy (79.30%):** The model correctly classified approximately 79% of the test customers.
- **Precision (50%):** Approximately half of the customers predicted as churn customers actually churned.
- **Recall (78%):** The model identified approximately 78% of the customers who actually churned.
- **F1 Score (61%):** It provides a balance between Precision and Recall.

The model identifies a good proportion of potential churn customers, although improving precision remains an important area for further experimentation.

## 🛠️ Technologies and Libraries Used

- Python
- Jupyter Notebook
- Pandas – Data manipulation and analysis
- NumPy – Numerical operations
- Matplotlib – Data visualization
- Seaborn – Statistical visualization
- Scikit-learn – Data preprocessing, SVM training, and model evaluation

## 📁 Project Structure

```text
Bank-Customer-Churn-Prediction-SVM/
│
├── Bank_Customer_Churn_Prediction_SVM.ipynb
├── Bank Customer Churn Prediction.csv
├── requirements.txt
└── README.md
```

## 🚀 How to Run This Project

### 1. Clone the repository

```bash
git clone https://github.com/YOUR-USERNAME/Bank-Customer-Churn-Prediction-SVM.git
```

### 2. Navigate to the project folder

```bash
cd Bank-Customer-Churn-Prediction-SVM
```

### 3. Install the required libraries

```bash
pip install -r requirements.txt
```

### 4. Open Jupyter Notebook

```bash
jupyter notebook
```

### 5. Run the notebook

Open `Bank_Customer_Churn_Prediction_SVM.ipynb` and execute the cells in order.

**Note:** Keep the CSV dataset in the same folder as the notebook. If you distribute the dataset, make sure its license permits redistribution.

## 🔮 Future Improvements

There is still room to improve this project. Some possible future improvements include:

- Experimenting with additional SVM hyperparameter combinations.
- Improving churn prediction precision while maintaining good recall.
- Comparing SVM with other classification algorithms such as Logistic Regression, Decision Tree, Random Forest, and XGBoost.
- Using cross-validation for more reliable model selection.
- Deploying the trained model through a simple web application.
- Building a system that helps banks identify and prioritize customers who may be at risk of leaving.

## 📚 Key Takeaway

This project helped me understand that Machine Learning is not just about training a model and checking its accuracy. It involves understanding the data, preprocessing it correctly, selecting suitable algorithms, experimenting with different parameters, and evaluating the results using appropriate metrics.

Most importantly, this project strengthened my practical understanding of **Support Vector Machine (SVM)** and the overall Machine Learning workflow.

---

**Project Type:** Machine Learning | Supervised Learning | Binary Classification

**Algorithm:** Support Vector Machine (SVM)

**Learning Focus:** Practical understanding of Machine Learning concepts, especially SVM.
