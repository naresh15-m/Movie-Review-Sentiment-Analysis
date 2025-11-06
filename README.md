# Movie-Review-Sentiment-Analysis
A machine learning web application that classifies movie reviews as positive or negative using Natural Language Processing (NLP) and sentiment analysis.

📋 Project Overview
This project implements a sentiment analysis system for movie reviews using:

Machine Learning: Logistic Regression classifier

NLP Processing: TF-IDF vectorization with stopword removal

Web Interface: Streamlit-based web application

Data Processing: Pandas and NLTK for text preprocessing

🚀 Features
Real-time Prediction: Instant sentiment analysis of movie reviews

User-friendly Interface: Clean and intuitive web interface

Accurate Classification: Trained on 500 movie reviews dataset

Preprocessing Pipeline: Comprehensive text cleaning and normalizationStep 1: Clone the Repository

git clone https://github.com/yourusername/movie-review-sentiment-analysis.git
cd movie-review-sentiment-analysis

Step 2: Install Dependencies

pip install -r requirements.txt
If requirements.txt is not available, install packages manually:

pip install pandas numpy scikit-learn streamlit nltk matplotlib

Step 3: Download NLTK Data
python
import nltk
nltk.download('stopwords')

📁 Project Structure

movie-review-sentiment-analysis/
│
├── data.ipynb                 # Jupyter notebook for data preprocessing and model training
├── app.py                     # Streamlit web application
├── model.pkl                  # Trained machine learning model
├── vectorizer.pkl            # TF-IDF vectorizer
├── Movie_Review.csv          # Dataset (500 movie reviews)
└── README.md                 # Project documentation
🔧 Usage
Running the Web Application
bash
streamlit run app.py
The application will open in your default web browser at http://localhost:8501

Using the Application
Enter a movie review in the text input field

Click the "Predict" button

View the sentiment prediction:

😊 Positive Review

😞 Negative Review

Example Reviews to Test
Positive Review:

"This movie was absolutely fantastic! The acting was superb and the storyline kept me engaged from beginning to end."

Negative Review:

"I was very disappointed with this film. The plot was predictable and the characters were poorly developed."

🏗️ Model Training
Data Preprocessing
The data preprocessing pipeline includes:

Loading and cleaning the movie review dataset

Handling missing values and data type conversions

Stopword removal using NLTK's English stopwords

Text normalization and cleaning

Model Architecture
Vectorizer: TF-IDF (Term Frequency-Inverse Document Frequency)

Classifier: Logistic Regression

Feature Engineering: Text vectorization with proper preprocessing

Training Process
Load and preprocess the Movie_Review.csv dataset

Split data into features (text) and labels (sentiment)

Train TF-IDF vectorizer on the text data

Train Logistic Regression classifier

Save model and vectorizer as pickle files

📊 Dataset
The project uses a dataset containing 500 movie reviews with sentiment labels:

263 negative reviews

237 positive reviews

Each review is labeled as either "positive" or "negative" sentiment.
