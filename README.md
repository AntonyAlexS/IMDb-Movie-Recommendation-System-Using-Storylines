# IMDb-Movie-Recommendation-System-Using-Storylines
This project builds a content-based movie recommender system that suggests similar movies based on user-input storylines. 
## 🔍 Problem Statement

Help users find similar movies based on storyline input. The system extracts 2024 IMDb movie data (name + storyline) and recommends the top 5 most similar movies using NLP techniques.

**Workflow Overview**

# 1. Data Collection
- Scraped 2024 movie names and storylines from IMDb using Selenium.
- Stored data into `Movies_data.csv`.

# 2. NLP Processing
- Cleaned storylines: removed stopwords and punctuation
- Converted storylines into vectors using **TF-IDF Vectorizer**.

# 3. Similarity Matching
- Computed pairwise **cosine similarity** between all movie vectors.
- Defined a function to recommend top 5 similar movies given a storyline.

# 4. Streamlit App
- Users input a storyline.
- App returns the 5 most similar movie recommendations.
