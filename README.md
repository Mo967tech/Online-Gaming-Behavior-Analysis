# Online Gaming Behavior Analysis

## **Overview**
This project analyzes the **Online Gaming Behavior Dataset** to predict **Engagement Levels** of players using machine learning. The dataset offers insights into player activities, enabling us to develop models that can forecast future engagement and tailor strategies for improved user retention.

---

## **Dataset Details**

- **Dataset Source**: Kaggle  
- **Number of Instances**: 40,034  
- **Number of Attributes**: 13 (12 features + 1 target variable)

### **Attributes**:
1. **PlayerID**: Unique identifier for each player.  
2. **Age**: Age of the player.  
3. **Gender**: Gender of the player.  
4. **Location**: Geographic location of the player.  
5. **GameGenre**: Genre of the game the player is engaged in.  
6. **PlayTimeHours**: Average hours spent playing per session.  
7. **InGamePurchases**: Indicates whether the player makes in-game purchases (0 = No, 1 = Yes).  
8. **GameDifficulty**: Difficulty level of the game.  
9. **SessionsPerWeek**: Number of gaming sessions per week.  
10. **AvgSessionDurationMinutes**: Average duration of each gaming session in minutes.  
11. **PlayerLevel**: Current level of the player in the game.  
12. **AchievementsUnlocked**: Number of achievements unlocked by the player.  

### **Target Variable**:
- **EngagementLevel**: Categorized engagement level reflecting player retention. Values:  
  - Low  
  - Medium  
  - High  

---

## **Steps Followed**

### **1. Data Preprocessing**
- Converted categorical columns (e.g., Gender, Location) into numerical format using **Label Encoding** and **One-Hot Encoding**.  
- Scaled numerical features using **StandardScaler** to normalize data distribution.

### **2. Exploratory Data Analysis (EDA)**
- Visualized feature correlations using a **heatmap**.  
- Examined target variable distribution to understand engagement patterns.

### **3. Model Development**
- **Gaussian Naive Bayes**  
- **K-Nearest Neighbors (KNN)**  
- **Decision Tree Classifier**  
- **Random Forest Classifier**

### **4. Model Evaluation**
- Metrics used:
  - **Accuracy**  
  - **Confusion Matrix**  
  - **ROC Curves** for multi-class performance visualization  

---

## **Key Results**

### **1. Accuracy Scores**
- **Gaussian Naive Bayes**: Moderate performance due to assumptions of feature independence.  
- **KNN**: Performed well but sensitive to scaling and parameter tuning.  
- **Decision Tree**: High training accuracy but prone to overfitting.  
- **Random Forest**: Best-performing model with high test accuracy and generalization ability.

### **2. ROC Curves**
- Used **label_binarize** to compute class-wise ROC curves, showing model performance for each engagement level.

### **3. Confusion Matrix**
- Analyzed prediction accuracy per class, identifying areas where models could be improved.

---

## **Technologies Used**

- **Programming Language**: Python  
- **Libraries**:
  - `numpy`, `pandas` (Data Manipulation)  
  - `matplotlib`, `seaborn` (Visualization)  
  - `scikit-learn` (Machine Learning Models and Metrics)  

---

## **Conclusion**
The project highlights the importance of data preprocessing and model evaluation in building effective predictive systems. **Random Forest** proved to be the most robust model for predicting player engagement levels.

---
