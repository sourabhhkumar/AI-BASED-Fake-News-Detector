# 📰 Fake News Detector – Streamlit App

> **Detect misinformation instantly with the power of machine learning.**

---

## 🚀 Live Demo

👉 [**Click here to try the Fake News Detector live!**]



## 📖 Overview

In a world overwhelmed with information, identifying **fake news** is critical. This interactive web app allows users to **predict whether a news article or headline is REAL or FAKE**, using an efficient and lightweight machine learning pipeline.

Built with **Python** and **Streamlit**, the app demonstrates a full-stack NLP pipeline — from **data cleaning and TF-IDF extraction** to **model training and deployment**.

---

## ✨ Key Features

- 🎨 **Beautiful Streamlit UI** – Clean, responsive, and mobile-friendly
- 📝 **Flexible Input** – Analyze both short headlines and full articles
- ⚡ **Real-Time Prediction** – One click for instant results (REAL or FAKE)
- 🧹 **Preprocessing Preview** – See how your text is transformed before analysis
- ✅ **Clear Visual Feedback** – Colored labels, icons, and animations for better UX
- 📢 **Disclaimer** – Transparent about limitations of the model

---

## 🧠 How It Works

### 1. 📊 **Data Acquisition**
- Uses labeled datasets: `True.csv` and `Fake.csv` from Kaggle  
- Merged and shuffled for balanced training

### 2. 🧼 **Text Preprocessing**
- Lowercasing  
- Removing punctuation and numbers  
- Filtering stopwords using `nltk`  
- Lemmatization for word normalization

### 3. ✍️ **Feature Extraction with TF-IDF**
- Calculates how important each word is  
- Converts cleaned text into numerical vectors  
- Keeps top 5000 features for efficiency

### 4. 🤖 **Model Training**
- **Passive Aggressive Classifier** from `scikit-learn`
- Learns fast and adjusts aggressively on misclassifications
- Outputs binary classification: REAL or FAKE

### 5. ✅ **Real-Time Prediction**
- User input is preprocessed and vectorized  
- Trained model predicts class label  
- Streamlit displays the result in real-time

---

## 🛠️ Tech Stack

- **Python 3.x**
- **Streamlit** – Web UI
- **scikit-learn** – ML Model & TF-IDF
- **nltk** – Text preprocessing
- **pandas** – Data wrangling
- **joblib** – Model persistence

---

## 🧪 Run Locally

```bash
# 1. Clone the repository
git clone https://github.com/YOUR_USERNAME/Fake-News-Detector-Streamlit-App.git
cd Fake-News-Detector-Streamlit-App

# 2. (Optional) Create and activate virtual environment
python -m venv venv
source venv/bin/activate  # or .\venv\Scripts\activate on Windows

# 3. Install dependencies
pip install -r requirements.txt

# 4. Download NLTK data
python -c "import nltk; nltk.download('wordnet'); nltk.download('stopwords')"

# 5. Add the dataset
# Place Fake.csv and True.csv inside the ./data/ directory

# 6. Train the model
python main.py

# 7. Run the Streamlit app
streamlit run app.py
```

---

## 🚧 Limitations

- ⚠️ **No factual verification** – based only on learned patterns
- 🧩 **Dataset-dependent** – may reflect biases or gaps in training data
- 📉 **Short input limitations** – short texts may lack enough signal
- 🌍 **No context awareness** – doesn’t check source or author credibility

---

## 🔮 Future Improvements

- 🧠 Use **transformer models** (e.g., BERT) for deeper understanding  
- 🔍 Add **explainability** (e.g., SHAP, LIME)  
- 🛰️ Integrate **external fact-checking APIs**  
- 🖼️ Detect **image/video-based fake news**  
- 🧵 Include **source credibility** analysis  
- 🗣️ Support **multilingual detection**

---

## 👨‍💻 Author

  
GitHub: https://github.com/sourabhhkumar
LinkedIn: https://www.linkedin.com/in/sourabhhkumar163/


## 📄 License

None
"# AI-BASED-Fake-News-Detector" 
