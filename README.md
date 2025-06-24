# 🎮 GAME-AI: PUBG Winner Prediction

**Project Type**: Machine Learning · Regression · Game Analytics  
**Goal**: Predict a player’s win placement percentage (`winPlacePerc`) in PUBG based on their in-game performance metrics.

---

## 🧠 Problem Statement

The objective of this project is to develop a machine learning model that predicts the **win probability of a PUBG player** based on game telemetry data such as kills, damage dealt, movement distance, and item usage.

This solution provides insights into the key factors that influence winning and can be used to improve gameplay strategy, build analytics dashboards, or enhance competitive matchmaking.

---

## 📁 Dataset Overview

- 📊 **Records**: 4.4 million+ PUBG match entries
- 🏷️ **Target**: `winPlacePerc` (continuous value between 0.0 and 1.0)
- 📦 **Features**: 28 gameplay variables including:
  - `kills`, `damageDealt`, `heals`, `walkDistance`, `boosts`
  - `killPlace`, `killPoints`, `weaponsAcquired`, `rideDistance`, etc.



---

## 📊 Exploratory Data Analysis (EDA)

- Performed feature correlation and distribution analysis.
- Identified multicollinearity and engineered meaningful predictors.
- Visualized impact of metrics like distance traveled and damage dealt on winning percentage.
- Removed nulls, outliers, and redundant columns (`Id`, `groupId`, `matchId`, etc.).



---

## 🤖 Models Implemented

| Model               | R² Score | Notes                              |
|--------------------|----------|-------------------------------------|
| Linear Regression   | 0.83     | Simple baseline, underfit          |
| Random Forest       | 0.91     | Strong performance, low variance   |
| XGBoost Regressor   | ✅ **0.92** | Best performer overall             |
| MLP Neural Network  | 0.89     | Tuned using Keras Tuner            |

- Feature scaling applied to improve neural network performance.
- Hyperparameter tuning with `GridSearchCV` and `KerasTuner`.

---

## 🧠 Key Insights

- `walkDistance`, `damageDealt`, and `boosts` are top predictors of win probability.
- Players with consistent movement and resource usage score higher.
- Neural networks are effective but tree-based models like **XGBoost** deliver faster and better results for this structured data.

---

## 🛠️ Tools & Technologies

- **Python**, **Pandas**, **Scikit-learn**, **XGBoost**
- **Keras + TensorFlow** for deep learning
- **Matplotlib**, **Seaborn** for visualizations
- **GridSearchCV**, **Keras Tuner** for hyperparameter optimization
- Jupyter Notebook (development environment)

---

---

## 👨‍💻 Author

**Shubham Thanki**  
📍 Toronto, ON  
📫 [shubham.thanki12@gmail.com](mailto:shubham.thanki12@gmail.com)  
🔗 [LinkedIn](https://linkedin.com/in/shubham-thanki) | [Portfolio](https://yourportfolio.com) | [GitHub](https://github.com/ShubhamThanki)

---

## ⭐️ If you found this useful, please give it a star and connect!
