# SMS Spam Detection using Naive Bayes

## 📌 Project Overview
This notebook builds a **Naive Bayes classifier** to detect spam messages in SMS texts. The model achieves **97.4% accuracy** in distinguishing between spam and legitimate (ham) messages.

## 📂 Dataset: SMS Spam Collection
- **Source**: UCI Machine Learning Repository
- **Total messages**: 5,572 SMS messages
- **Classes**: 
  - **Ham** (legitimate): 4,825 messages (86.6%)
  - **Spam**: 747 messages (13.4%)

## 📊 Exploratory Data Analysis
- **Class Distribution**: Imbalanced dataset (86.6% ham, 13.4% spam)
- **Message Length**: Spam messages tend to be longer (avg 139 chars) than ham (avg 71 chars)

## 🔧 Key Steps
1. **Data Loading**: Download dataset from GitHub
2. **Exploratory Data Analysis**: Visualize class distribution and message lengths
3. **Text Preprocessing**: TF-IDF vectorization with stop words removal (5000 features)
4. **Model Training**: Multinomial Naive Bayes classifier
5. **Evaluation**: Accuracy, confusion matrix, classification report
6. **Comparison**: Test different Naive Bayes variants
7. **Testing**: Predict custom messages
8. **Feature Analysis**: Identify top words associated with spam


## 📈 Results

### Model Performance

| Model | Accuracy |
|-------|----------|
| **MultinomialNB** | **97.40%** |
| BernoulliNB | 97.04% |
| GaussianNB | 85.83% |


### Classification Report
          precision    recall  f1-score   support
     Ham       0.97      1.00      0.99       966
    Spam       1.00      0.81      0.89       149
accuracy                           0.97      1115


### Confusion Matrix
      Predicted
      Ham  Spam


### Sample Predictions
✅ HAM: "Hey, are we still meeting for lunch tomorrow?" (99.7% confidence)
🚫 SPAM: "Congratulations! You've won a free iPhone..." (86.8% confidence)
🚫 SPAM: "URGENT: Your account has been compromised..." (83.9% confidence)


## 🛠️ Technologies Used
| Library | Purpose |
|---------|---------|
| **Scikit-learn** | Naive Bayes, TF-IDF, train-test split |
| **Pandas** | Data manipulation |
| **NumPy** | Numerical operations |
| **Matplotlib/Seaborn** | Data visualization |


## 🚀 How to Run
1. Open in Google Colab
2. Run all cells sequentially
3. Dataset downloads automatically
4. View results and predictions


## 🎯 Learning Outcomes
- ✅ Text classification with Naive Bayes
- ✅ TF-IDF vectorization for text data
- ✅ Handling imbalanced datasets
- ✅ Model evaluation metrics (precision, recall, f1-score)
- ✅ Feature importance analysis
- ✅ Comparing different Naive Bayes variants


## 🔍 Key Insights
- **MultinomialNB** works best for text classification
- Spam messages are **longer** on average than ham messages
- Words like **"free"**, **"txt"**, and **"claim"** are strong spam indicators
- The model is **very conservative** with spam (high precision) but misses some (lower recall).