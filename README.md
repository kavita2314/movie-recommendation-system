# 🎬 Movie Recommendation System

A **Content-Based Movie Recommendation System** built using **Python**, **Pandas**, and **Scikit-learn**. This project uses **Natural Language Processing (NLP)** techniques to recommend movies based on their **overview** and **genre** using **TF-IDF Vectorization** and **Cosine Similarity**.

---

## 📌 Project Objective

To build an intelligent system that recommends movies similar to a given title based on their content description and genre, helping users discover films aligned with their interests.

---

## 🧰 Technologies Used

- **Python**
- **Pandas**
- **Scikit-learn** (TF-IDF, Cosine Similarity)
- **SciPy** (Sparse Matrix)
- **Jupyter Notebook / VS Code**

---

## 📁 Dataset

- **Name:** IMDb Top 1000 Movies
- **Format:** CSV
- **Important Columns:**
  - `Series_Title` – Movie Title
  - `Overview` – Short description
  - `Genre` – Genres
  - `IMDB_Rating` – IMDb Rating

---

## 🧠 NLP Techniques Used

| NLP Task             | Implementation                                       |
|----------------------|------------------------------------------------------|
| Text Cleaning        | Fill NA in `Overview` and `Genre`                    |
| Feature Extraction   | `TfidfVectorizer` with stop word removal             |
| Text Vectorization   | TF-IDF Matrix created from combined text             |
| Similarity Detection | Cosine Similarity based on TF-IDF matrix             |

---

## 🔍 How It Works

1. **Data Preprocessing:**
   - Missing values filled with empty strings.
   - Created a new column `Combined` from `Overview + Genre`.

2. **Vectorization:**
   - Applied TF-IDF vectorizer to transform the text into numeric format.

3. **Similarity Computation:**
   - Calculated cosine similarity between all movie pairs.

4. **Recommendation Logic:**
   - Given a movie title, returns top 10 most similar movies based on content.

---

## 🚀 How to Run the Project

1. Clone the repository:
   ```bash
   git clone https://github.com/your-username/movie-recommendation-system.git
