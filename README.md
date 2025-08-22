📰 Fake News Detection System (English + Hindi)
📌 Project Overview

This project is a machine learning-based Fake News Detection System that can classify news articles as Real or Fake.
It supports both English and Hindi datasets and includes a fact-check link retriever that suggests reliable sources for verification.

✨ Features

✅ Preprocessing of English & Hindi text with stopword removal and stemming.

✅ TF-IDF vectorization for feature extraction.

✅ Logistic Regression model for classification.

✅ Model evaluation with Accuracy, Confusion Matrix, and Classification Report.

✅ Function to test custom news input (test_with_input).

✅ Fact-check link retriever (get_fact_check_link) to suggest credible sources.

🛠️ Tech Stack

Python

Pandas, NumPy

NLTK (Natural Language Toolkit)

Scikit-learn

Matplotlib

Logistic Regression

TF-IDF Vectorizer

📂 Dataset

True & Fake News Dataset (English) – CSV files.

Bharat Fake News Kosh (Hindi) – Excel file with Hindi and English translations.

Each dataset was cleaned, merged, and standardized into a single dataframe with labels:

1 → Real News

0 → Fake News

⚙️ How It Works

Load English & Hindi datasets.

Preprocess text (remove stopwords, stemming, clean mixed-language text).

Convert text into numerical features using TF-IDF.

Train Logistic Regression on training data.

Evaluate performance using test data.

Allow users to test their own news text & get a prediction + fact-check link.

📊 Model Performance

Accuracy: ~85–90% (depending on dataset split).

Evaluation Metrics: Confusion Matrix & Classification Report included.

▶️ Usage

Clone this repository and run the Jupyter Notebook:

git clone https://github.com/your-username/fake-news-detection.git
cd fake-news-detection
jupyter notebook

Example:
input_text = "The government announced a new policy to boost agriculture in rural areas."
prediction = test_with_input(model, tfidf_vectorizer, input_text)
print("Prediction:", prediction)

link = get_fact_check_link(input_text, new_merged_df)
print("Fact Check Link:", link)

Output:
Prediction: Real News
Fact Check Link: https://examplefactcheck.com/article123


<img width="1920" height="1080" alt="Screenshot (27)" src="https://github.com/user-attachments/assets/bb4cfe1e-ec0e-43ca-8e36-4bf47df9104b" />
<img width="1920" height="1080" alt="Screenshot (26)" src="https://github.com/user-attachments/assets/80309ab3-368a-44e1-9da0-9850e96b7813" />



📌 Future Improvements

🔹 Expand multilingual support (more Indian languages).

🔹 Deep learning models (LSTM, BERT) for better accuracy.

🔹 Web app with user-friendly interface for real-time predictions.

🔹 API integration for fact-check sources.

🤝 Contributing

Pull requests are welcome. For significant changes, please open an issue first to discuss the proposed modifications.

📧 Contact

👤 Your Ravi kumar
📩 your.ravisingh07462@gmail.com.com
