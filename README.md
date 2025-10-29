# 🎬 Movie Recommender System (Streamlit App)

A simple **Content-Based Movie Recommender System** built using **Python, Streamlit, and The Movie Database (TMDb) API**.  
It recommends movies similar to a selected title along with their posters.

🚀 **Live Demo:** [Movie Recommender App](https://cbmrs-proj.streamlit.app/)

---

## 🧠 Project Overview

This project uses **content-based filtering** to recommend movies.  
It compares the selected movie with others in the dataset using **cosine similarity**, and suggests the top 5 most similar titles.  
Movie posters are fetched dynamically from **TMDb API**.

### ✨ Key Features
- Search and select any movie from the dropdown.
- Instantly get the top 5 movie recommendations.
- Displays movie posters fetched via TMDb API.
- Responsive and clean Streamlit interface.

---

## 🗂️ Repository Structure

```
├── app.py                 # Main Streamlit app
├── code.ipynb             # Jupyter notebook for preprocessing and model creation
├── movie_list.pkl         # Movie metadata
├── similarity.zip         # Compressed similarity matrix (auto-extracted in app.py)
├── requirements.txt       # Dependencies
└── README.md              # Documentation
```

---

## ⚙️ Installation and Setup

### 1. Clone the repository
```bash
git clone https://github.com/avulapuneethkumarreddy/Content_Based_Recommendation_System
cd Content_Based_Recommendation_System
```

### 2. Create and activate a virtual environment
```bash
python -m venv .venv
# On Windows
.venv\Scripts\activate
# On macOS/Linux
source .venv/bin/activate
```

### 3. Install dependencies
```bash
pip install -r requirements.txt
```

### 4. Run the app
```bash
streamlit run app.py
```

---

## 📦 Data Files

- **movie_list.pkl** → Contains all movie titles and IDs  
- **similarity.zip** → Compressed similarity matrix (automatically decompressed in the app)

---

## 🧩 How It Works

1. Loads movie list and similarity matrix.
2. Computes top 5 similar movies using cosine similarity.
3. Fetches movie posters via TMDb API.
4. Displays movie titles and posters in a clean layout.

---

## 🔑 API Usage

You need a TMDb API key to fetch posters.  
Get your key from: [https://www.themoviedb.org/settings/api](https://www.themoviedb.org/settings/api)

Update this line in `app.py`:
```python
api_key = "YOUR_TMDB_API_KEY"
```

---

## 🌐 Deployment

This project is deployed for free using **Streamlit Community Cloud**.  

### Deployment Steps
1. Push your code to GitHub.  
2. Visit [https://share.streamlit.io](https://share.streamlit.io).  
3. Connect your repo and set the entry file as `app.py`.  
4. Deploy and access your app live!  

---

## 📊 Example Output

| Recommended Movie | Poster |
|--------------------|--------|
| Movie 1 | 🎞️ Poster |
| Movie 2 | 🎞️ Poster |
| Movie 3 | 🎞️ Poster |
| Movie 4 | 🎞️ Poster |
| Movie 5 | 🎞️ Poster |

---

## 🧑‍💻 Built With
- [Python](https://www.python.org/)
- [Streamlit](https://streamlit.io/)
- [scikit-learn](https://scikit-learn.org/)
- [pandas](https://pandas.pydata.org/)
- [TMDb API](https://www.themoviedb.org/)

---

## 📜 License
This project is licensed under the **MIT License**.

---

## 💬 Acknowledgements
- TMDb for movie data and posters  
- Streamlit for free hosting  
- scikit-learn for similarity computation  

---

### 👨‍💻 Author
**Avula Puneeth Kumar Reddy**  
🎓 B.Tech in Information Technology at Atal Bihari Vajpayee Indian Institute of Information Technology and Management
📍 Anantapur, Andhra Pradesh
