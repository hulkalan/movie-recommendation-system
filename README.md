# 🎬 Movie Recommendation System

A content-based movie recommender system built using **Python**, **Streamlit**, and **The Movie Database (TMDB) API**. This app recommends 5 similar movies based on your selected movie and displays their posters.

---

## 🚀 Demo

> 👉 [Deployed on Render](#) *(update with your deployment URL if available)*

---

## 📌 Features

- Recommend 5 similar movies
- Fetch posters dynamically using TMDB API
- Case-insensitive movie search
- Clean and interactive UI with Streamlit

---

## 🧠 How It Works

- Movie data is taken from TMDB’s public dataset (`tmdb_5000_movies.csv` and `tmdb_5000_credits.csv`)
- Content-based filtering using:
  - Overview
  - Genre
  - Keywords
  - Cast
  - Director
- Cosine similarity is calculated on TF-IDF vectors
- TMDB API is used to fetch movie posters using `movie_id`

---

## 🛠️ Tech Stack

- Python
- Pandas, Scikit-learn, Requests
- Streamlit
- TMDB API

---

## 📂 Project Structure

movie-recommendation-system/
├── app.py # Main Streamlit app
├── requirements.txt # Required Python libraries
├── Procfile # For deployment (Heroku/Render)
├── movies.pkl # Preprocessed movie metadata
├── similarity.pkl # Precomputed similarity matrix
├── tmdb_5000_credits.csv # Raw data
├── tmdb_5000_movies.csv # Raw data
└── .gitignore



---

## ⚙️ Installation & Run Locally

### 1. Clone the repo

git clone https://github.com/hulkalan/movie-recommendation-system.git
cd movie-recommendation-system

---

#### Create virtual environment (optional but recommended)

python -m venv venv
venv\Scripts\activate  # On Windows
source venv/bin/activate  # On Linux/Mac

---

### Install dependencies

pip install -r requirements.txt


---

### Add your TMDB API Key

API_KEY = 'your_tmdb_api_key_here

---

### Run the App

streamlit run app.py




#### **Then open the browser at:**

http://localhost:8501

🌐 Deployment (Render, Hugging Face Spaces, etc.)
Keep requirements.txt and Procfile in the root.

Set your TMDB API key as an environment variable or inside app.py.

For Render, set the Start Command as:  streamlit run app.py



**🙋‍♂️ Author**
Alan Mathew
GitHub: @hulkalan