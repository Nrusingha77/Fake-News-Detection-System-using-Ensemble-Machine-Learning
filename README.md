# 🕵️‍♂️ Fake News Detection System

![Python](https://img.shields.io/badge/Python-3.8%2B-blue)
![Machine Learning](https://img.shields.io/badge/Machine%20Learning-Scikit--Learn-orange)
![Status](https://img.shields.io/badge/Status-Active-green)

## 📜 Project Overview

In an era where misinformation spreads rapidly across digital platforms, distinguishing between authentic journalism and fabricated stories is critical. This project leverages **Machine Learning (ML)** and **Natural Language Processing (NLP)** techniques to build a robust system capable of classifying news articles as "Fake" or "True" with high precision.

The solution implements a comprehensive data preprocessing pipeline and compares the performance of four distinct classification algorithms to ensure the most effective logic is used for prediction.

## 🚀 Key Features

*   **Comprehensive Data Preprocessing:** Automated cleaning of raw text data, including the removal of URLs, special characters, punctuation, and stop words to prepare high-quality input.
*   **TF-IDF Vectorization:** Utilizes `TfidfVectorizer` to transform text into numerical feature vectors, capturing the statistical importance of words.
*   **Multi-Model Classification:** Implements and evaluates four powerful algorithms: Logistic Regression, Decision Tree, Gradient Boosting, and Random Forest.
*   **Performance Metrics:** Detailed evaluation using Accuracy Score and Classification Reports (Precision, Recall, F1-Score).
*   **Manual Testing Interface:** A user-friendly function that allows users to input raw news text and receive real-time validity predictions from all four models instantly.

## 🛠️ Technologies Used

*   **Language:** Python 🐍
*   **Libraries:**
    *   `pandas` & `numpy` (Data Manipulation & Analysis)
    *   `matplotlib` & `seaborn` (Data Visualization)
    *   `scikit-learn` (Model Training, Evaluation & Feature Extraction)
    *   `re` & `string` (Text Processing)

## 📂 Dataset

The project utilizes two datasets containing thousands of news articles:
1.  **Fake.csv:** Articles identified as fabricated or misinformation.
2.  **True.csv:** Authentic news articles.

*Note: The datasets are merged, labeled (0 for Fake, 1 for True), and shuffled to prevent bias during training.*

## 📊 Model Performance

We trained and tested four models to identify the best performer. Here is a summary of their accuracy on the test set:

| Model | Accuracy Score |
| :--- | :---: |
| **Gradient Boosting Classifier** | **99.54%** |
| Decision Tree Classifier | 99.46% |
| Random Forest Classifier | 98.90% |
| Logistic Regression | 98.66% |

*The **Gradient Boosting Classifier** achieved the highest accuracy, demonstrating exceptional reliability in distinguishing fake news.*

## ⚙️ How to Run

1.  **Clone the repository:**
    ```bash
    git clone https://github.com/your-username/Fake-News-Detection.git
    ```
2.  **Install dependencies:**
    ```bash
    pip install pandas numpy matplotlib seaborn scikit-learn
    ```
3.  **Run the Jupyter Notebook:**
    Open `Fake News Detection.ipynb` in Jupyter Notebook or JupyterLab and run the cells sequentially to train the models and see the results.

## 🧪 Manual Testing

The project includes a `manual_testing` function. You can input any news article text, and the system will output the classification result from all four models.

**Example Output:**
```text
LR Prediction: Fake News
DT Prediction: Fake News
GBC Prediction: Fake News
RFC Prediction: Fake News
```

## 🤝 Contributing

Contributions are welcome! If you have suggestions for improving the models or adding new features, feel free to open an issue or submit a pull request.

## 📝 License

This project is open-source and available under the MIT License.

---
*Built with ❤️ by [NRUSINGHA PRASADA KHADANGA]*