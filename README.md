# 🎮 Online Gaming Player Engagement Prediction Using Random Forest

## 📌 Project Overview

This project applies Machine Learning to predict online gaming player engagement levels based on their gaming behavior and activities.

Using the **Random Forest Classifier**, the model predicts whether a player has Low, Medium, or High engagement.

This project demonstrates a complete Supervised Machine Learning workflow, from data exploration and preprocessing to model training, evaluation, and prediction using unseen data.

## 🎯 Project Objectives

- Analyze online gaming player behavior.
- Explore factors associated with player engagement.
- Develop a multiclass classification model.
- Predict player engagement levels.
- Evaluate model performance using classification metrics.
- Identify important features using Random Forest feature importance.

## 📂 Dataset Information

**Dataset:** `online_gaming_behavior_dataset.csv`

**Dataset Size:** 40,034 records and 13 columns.

### Features Description

| Feature | Description |
|---|---|
| PlayerID | Unique player identifier |
| Age | Player's age |
| Gender | Player's gender |
| Location | Player's location |
| GameGenre | Type of game played |
| PlayTimeHours | Hours spent playing |
| InGamePurchases | In-game purchase information |
| GameDifficulty | Game difficulty level |
| SessionsPerWeek | Number of weekly sessions |
| AvgSessionDurationMinutes | Average session duration |
| PlayerLevel | Player's current level |
| AchievementsUnlocked | Number of achievements unlocked |
| EngagementLevel | Target variable |

### Target Variable

The target variable is `EngagementLevel`, which contains three categories:

- Low
- Medium
- High

## 🤖 Machine Learning Approach

| Category | Description |
|---|---|
| Learning Type | Supervised Learning |
| Problem Type | Multiclass Classification |
| Algorithm | Random Forest Classifier |
| Target Variable | EngagementLevel |
| Training Split | 80% |
| Testing Split | 20% |

### Why Random Forest?

Random Forest is an ensemble learning algorithm that combines multiple Decision Trees to generate predictions.

Advantages:

- Combines multiple Decision Trees.
- Handles nonlinear relationships.
- Supports multiclass classification.
- Provides feature importance analysis.
- Reduces dependence on a single decision tree.

## ⚙️ Technologies & Libraries

- Python
- PyCharm
- Jupyter Notebook
- Pandas
- NumPy
- Matplotlib
- Seaborn
- Scikit-learn

## 🔄 Machine Learning Workflow

The project follows these steps:

1. Dataset Loading
2. Data Understanding
3. Exploratory Data Analysis (EDA)
4. Missing Value Analysis
5. Duplicate Checking
6. Feature Selection
7. Categorical Feature Encoding
8. Train-Test Splitting
9. Random Forest Model Building
10. Model Training
11. Model Prediction
12. Model Evaluation
13. Confusion Matrix Visualization
14. Feature Importance Analysis
15. Prediction on Unseen Data

## 🌳 Random Forest Model Configuration

The model uses the following configuration:

```python
RandomForestClassifier(
    n_estimators=100,
    max_depth=None,
    random_state=42,
    class_weight="balanced",
    n_jobs=-1
)
```

| Parameter | Description |
|---|---|
| n_estimators | Number of decision trees |
| max_depth | Maximum depth of each tree |
| random_state | Ensures reproducibility |
| class_weight | Adjusts weights for class imbalance |
| n_jobs | Uses available CPU cores |

## 📊 Model Evaluation

The model performance is evaluated using:

- Accuracy Score
- Precision
- Recall
- F1-Score
- Confusion Matrix

These metrics help measure how effectively the model predicts the three engagement categories.

**Note:** Actual model performance results will be added after completing the experiments.

## 📈 Feature Importance

Random Forest provides feature importance scores to identify which gaming behavior features contribute most to the model's predictions.

A feature importance visualization is used to display the top 10 important features.

## 🔮 Unseen Data Prediction

The trained model can predict the engagement level of a new player based on their gaming behavior.

Example:

```text
Input:
Age: 22
PlayTimeHours: 15.5
SessionsPerWeek: 12
PlayerLevel: 45

Output:
Predicted Engagement: High
```

*Illustrative example only.*

## 📁 Project Structure

```text
online-gaming-engagement-prediction/
│
├── online_gaming_behavior_dataset.csv
│
├── Random_Forest_Classification.ipynb
│
├── requirements.txt
│
├── README.md
│
└── .gitignore
```

## 🚀 Installation & Usage

### 1. Clone the Repository

```bash
git clone YOUR_GITHUB_REPOSITORY_URL
```

### 2. Navigate to the Project Folder

```bash
cd online-gaming-engagement-prediction
```

### 3. Create a Virtual Environment

```bash
python -m venv venv
```

Activate the environment:

**Windows:**
```bash
venv\Scripts\activate
```

**Linux / macOS:**
```bash
source venv/bin/activate
```

### 4. Install Dependencies

```bash
pip install -r requirements.txt
```

### 5. Open the Jupyter Notebook

Open the project in PyCharm and execute:

`Random_Forest_Classification.ipynb`

Run the notebook cells sequentially to reproduce the analysis and model training.

## 📚 Key Learning Outcomes

Through this project, I explored:

- Supervised Machine Learning.
- Multiclass Classification.
- Exploratory Data Analysis.
- Data preprocessing.
- Categorical Encoding.
- Train-Test Splitting.
- Decision Tree fundamentals.
- Random Forest Classification.
- Ensemble Learning.
- Model Evaluation.
- Feature Importance.
- Prediction on Unseen Data.

## 🔮 Future Improvements

- Hyperparameter tuning using GridSearchCV.
- Compare Random Forest with Decision Tree, SVM, and Logistic Regression.
- Experiment with different numbers of decision trees.
- Improve model performance.
- Develop an interactive dashboard using Streamlit.

## 👩‍💻 Author

**Data Science Undergraduate**

Interested in Machine Learning, Data Science, and Artificial Intelligence.

---

⭐ If you find this project interesting, consider giving the repository a star!
