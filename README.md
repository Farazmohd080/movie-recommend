# 🎥 Movie Recommendation System


A **Machine Learning-based Movie Recommendation System** that suggests movies to users based on similarities in movie content such as **genres**, **keywords**, **cast**, and **crew**.  

Built using **Python**, **Flask**, and **Scikit-learn**, this project offers personalized movie recommendations through a simple web interface.

---

## 🧠 Features
✅ Recommends movies similar to the one selected by the user  
✅ Uses **Cosine Similarity** and **TF-IDF / Count Vectorizer** for recommendations  
✅ Interactive **Flask web app interface**  
✅ Clean and simple **HTML frontend**  
✅ Pre-trained model for fast recommendations  

---

## 📂 Project Structure
```
Movie-Recommendation-System/
│
├── app.py                            # Flask web application
├── movie-recommendation-system.ipynb # Jupyter notebook for model building
├── model/
│   └── movie_rec.pkl                 # Pre-trained recommendation model
│
├── templates/
│   └── index.html                    # Webpage for user interaction
│
├── tmdb_5000_movies.csv              # Dataset containing movie details
├── tmdb_5000_credits.csv             # Dataset containing cast & crew details
├── requirements.txt                  # Python dependencies
└── README.md                         # Project documentation
```

---

## ⚙️ Installation & Setup


### 2️⃣ Install Dependencies
Make sure Python 3.8+ is installed, then run:
```bash
pip install -r requirements.txt
```

If you don’t have the file, install manually:
```bash
pip install flask pandas scikit-learn numpy
```

---

## 🚀 How to Run the Project

### 🔹 Run the Flask App
```bash
python app.py
```

Then open your browser and go to:
```
http://127.0.0.1:5000/
```

You’ll see a simple interface to **enter or select a movie title**.  
Click **Recommend** to get similar movies instantly! 🎬  

---

## 🧠 How It Works
1. Data from `tmdb_5000_movies.csv` and `tmdb_5000_credits.csv` is preprocessed.  
2. Key features (overview, genres, keywords, cast, crew) are combined into a single text field.  
3. A **CountVectorizer** or **TF-IDF Vectorizer** converts the text into numerical form.  
4. **Cosine Similarity** is calculated between all movies.  
5. The Flask app (`app.py`) loads the pre-trained `movie_rec.pkl` model and returns top 5 similar movies.  

---

## 🧰 Technologies Used
- **Python 3**
- **Flask** (Web Framework)
- **Scikit-learn** (ML Toolkit)
- **Pandas / NumPy** (Data Processing)
- **HTML / CSS / Bootstrap** (Frontend)
- **Jupyter Notebook** (Model training & testing)

---

## 🎬 Example Output

**Input Movie:** Inception  
**Top 5 Recommended Movies:**  
1️⃣ Interstellar  
2️⃣ The Dark Knight Rises  
3️⃣ The Prestige  
4️⃣ Memento  
5️⃣ The Matrix  





---

### ⭐ If you like this project, please give it a star on GitHub! ⭐
