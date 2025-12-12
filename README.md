# Movie Recommender System 🎬

A content-based movie recommender system that suggests movies similar to your favorites.

## 📌 Overview
This project implements a movie recommendation engine using **Cosine Similarity**. It suggests 5 similar movies based on a selected movie's metadata (genres, keywords, cast, crew, etc.). The processed data is powered by the **TMDB 5000 Movie Dataset**.

## 🚀 Features
- **Interactive UI**: Built with Streamlit for a smooth user experience.
- **Movie Posters**: Fetches and displays real-time movie posters using the TMDB API.
- **Accurate Recommendations**: Uses a pre-computed similarity matrix to find the closest matches.

## 🛠️ Tech Stack
- **Python**
- **Streamlit** (Frontend)
- **Pandas** (Data Manipulation)
- **Scikit-learn** (Similarity Metric - used in preprocessing)
- **Requests** (API calls for posters)

## 📂 Project Structure
- `movies_recom.py`: The main Streamlit application file.
- `movie_recommender_system.ipynb`: Jupyter notebook used for data cleaning, preprocessing, and model generation.
- `tmdb_5000_movies.csv` & `tmdb_5000_credits.csv`: Raw datasets.
- `movies_dict.pkl`: Pre-processed movie dictionary.
- `similarity.pkl`: Pre-computed similarity matrix.

## ⚙️ Installation & Usage

1.  **Clone the repository** (or download the files).

2.  **Install dependencies**:
    ```bash
    pip install streamlit pandas requests
    ```

3.  **Download Data Files**:
    Download the CSV and PKL files from [Google Drive](https://drive.google.com/drive/folders/1XvmRBu4rmHn305YIODy0myXb8sI67tor?usp=sharing) and place them in the project directory.

4.  **Run the application**:
    ```bash
    streamlit run movies_recom.py
    ```

4.  **Select a movie** from the dropdown and click "Show Recommendation" to see similar movies!

## 📝 Note
The application fetches movie posters using the TMDB API. If you encounter issues with images, ensure you have an active internet connection.
