# 🎮 Gamer Type Classification

This project classifies gamers into four categories based on their behavior and preferences using supervised machine learning models.

## 🗂 Dataset

- **Original File**: `Gamer Type Classification for PlayArena.csv`
- **Processed File**: `classification.csv`
- **Samples**: 1000
- **Target Labels**: 
  - `GamerType_Casual`
  - `GamerType_Strategist`
  - `GamerType_Socializer`
  - `GamerType_Explorer`

Features include:
- Session time per week
- Streaming hours
- Total session time
- In-game purchases
- Number of friends
- Preferred game genre (one-hot encoded)

## 📊 Preprocessing

- One-hot encoding for categorical columns
- Target variable converted from one-hot to class index
- Split into train/test using `train_test_split`
- Also Label encodind the target column

## 🧠 Models Tried

- **ANN**
- **SVM**
- **Logistic Regression**
- **Random Forest**
- **XGBoost**
- **Voting Ensemble** (Logistic + RF)

### 🔍 Best Accuracy:
**35.5%** using `VotingClassifier` with hard voting.

> ⚠️ Accuracy is low due to weakly informative features and small sample size.

## 🛠 Tools & Libraries

- Python 3.x
- Pandas, NumPy
- scikit-learn
- XGBoost
- Matplotlib / Seaborn (for visualization)
- Tensorflow

## 📁 Folder Structure
- Gamer Type Classification for PlayArena.csv # Original data
- Outputs / Preprocessed Data # Preprocessed data
- Outputs / EDA report.html # Download and use the file 
- model.py  # Training and evaluation scripts
- Drive link for model_ipynb.md # to access model.ipynb
- README.md
