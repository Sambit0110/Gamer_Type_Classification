# Gamer_Type_Classification
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
- Session time
- Streaming hours
- In-game purchases
- Number of friends
- Preferred game genre (one-hot encoded)

## 📊 Preprocessing

- One-hot encoding for categorical columns
- Target variable converted from one-hot to class index
- Split into train/test using `train_test_split`

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

## 📈 Future Improvements

- Add feature engineering (e.g. EngagementScore)
- Use PCA/t-SNE to visualize class separability
- Explore unsupervised clustering (e.g. KMeans)
- Try deep learning only after more data is available

## 📁 Folder Structure
├── Gamer Type Classification for PlayArena.csv # Original data
├── classification.csv # Preprocessed data
├── model.ipynb / model.py # Training and evaluation scripts
└── README.md
