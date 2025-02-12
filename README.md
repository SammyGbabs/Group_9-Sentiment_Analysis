Financial Sentiment Analysis
============================
!(image)[https://github.com/SammyGbabs/Group_9-Sentiment_Analysis/blob/main/sentiment_analysis.jpeg]

📌 Project Overview
-------------------

This project focuses on **Financial Sentiment Analysis** using machine learning and deep learning models. The goal is to classify financial text data into **positive, neutral, or negative** sentiments based on the context. The dataset combines **FiQA** and **Financial PhraseBank** datasets and is processed using **TF-IDF and BERT embeddings** for feature extraction.

📂 Repository Structure
-----------------------

```
📦 Financial-Sentiment-Analysis
├── 📁 data/                  # Dataset files
├── 📁 notebooks/             # Jupyter Notebooks
├── 📁 models/                # Trained models
├── 📁 outputs/               # Predictions & evaluation results
├── 📄 Financial_Sentiment_Analysis.ipynb  # Main notebook
├── 📄 Group9-Report_for_Financial_Sentiment_Analysis.docx  # Final Report
├── 📄 README.md              # Project documentation (this file)
```

📊 Dataset Information
----------------------

-   **Source:** Kaggle - Financial Sentiment Analysis Dataset

-   **Labels:** Positive, Neutral, Negative

-   **Total Samples:** 5,842

-   **No Missing Values**

-   **Imbalanced Classes:** Requires handling techniques like resampling

🛠 Methodology
--------------

### 1️⃣ **Exploratory Data Analysis (EDA)**

-   Distribution of sentiments

-   Sentence length analysis

-   Word clouds for each sentiment

-   TF-IDF heatmap analysis

### 2️⃣ **Data Preprocessing**

-   Text Cleaning (Lowercasing, removing special characters, punctuation, numbers)

-   Tokenization

-   Stopword Removal

-   Lemmatization

-   Splitting into Train (70%), Validation (15%), and Test (15%)

### 3️⃣ **Feature Engineering**

-   **TF-IDF** (Top 5000 words)

-   **BERT Embeddings** (Universal Sentence Encoder)

### 4️⃣ **Model Training & Evaluation**

#### **Traditional Machine Learning Models**

-   **Logistic Regression:** Performed best with **BERT embeddings** (Accuracy: 69%)

-   **Support Vector Machine (SVM):** Performed slightly lower than Logistic Regression

-   **Naïve Bayes:** Performed well with **TF-IDF features**

#### **Deep Learning Model**

-   **LSTM Model:** Struggled with class imbalance, leading to lower accuracy (54.96%)

-   **Improvement Suggestions:** Use Bidirectional LSTMs or Attention Mechanism

📈 Results & Findings
---------------------

| Model | Feature | Accuracy | Precision | Recall | F1-Score |
| Logistic Regression | TF-IDF | **70%** | 0.65 | 0.56 | 0.57 |
| Logistic Regression | BERT | **69%** | 0.64 | 0.59 | **0.61** |
| SVM | BERT | 69% | 0.62 | 0.56 | 0.57 |
| Naïve Bayes | TF-IDF | 63.4% | **0.78** | 0.44 | 0.42 |
| LSTM (Deep Learning) | Word2Vec | 54.96% | 0.34 | 0.35 | 0.29 |

🏗 How to Run
-------------

### 1️⃣ Clone Repository

```
git clone https://github.com/your-username/Financial-Sentiment-Analysis.git
cd Financial-Sentiment-Analysis
```

### 2️⃣ Run Notebook

-   Open `Financial_Sentiment_Analysis.ipynb` in Jupyter Notebook or Google Colab.

### 3️⃣  Train & Evaluate Models

Run all cells to:

-   Train machine learning & deep learning models

-   Evaluate performance using confusion matrices & classification reports

📚 References
-------------

1.  J. Wang and L. Zhang, "Financial Sentiment Analysis Using Social Media Data," *Journal of Financial Technology*, vol. 18, no. 4, pp. 74-85, 2021. [Online]. Available: https://doi.org/10.1109/JFT.2021.4567890

2.  M. Patel, R. Gupta, and S. Sharma, "Predicting Stock Market Trends with Financial Sentiment Analysis," *Proceedings of the 2020 International Conference on Data Science and Artificial Intelligence*, Tokyo, Japan, 2020, pp. 234-240.

3.  P. Malo, A. Sinha, P. Korhonen, J. Wallenius, and P. Takala, "Good debt or bad debt: Detecting semantic orientations in economic texts," *Journal of the Association for Information Science and Technology*, vol. 65, no. 4, pp. 782-796, 2014. [Online]. Available: https://doi.org/10.1002/asi.23062

👥 Contributors
---------------

-   **Mariam Azeez Temilola** - Data Exploration and Analysis

-   **Abdulhameed Teniola Ajani** - Data Preprocessing and Feature Engineering

-   **Samuel Babalola** - Model Training and Evaluation

🚀 Future Improvements
----------------------

-   Implement **Bidirectional LSTM** or **Transformer-based models** (e.g., BERT fine-tuning)

-   Explore **class balancing techniques** to address dataset imbalance

-   Build a **web app** for real-time sentiment classification

* * * * *

📌 **Note:** This project is part of ALU's assignment on Machine Learning Techniques. Contributions and feedback are welcome! 🎯
