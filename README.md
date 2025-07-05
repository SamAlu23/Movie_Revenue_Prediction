# 🎬 Movie Revenue Prediction (TMDB Dataset)

This project explores and predicts movie revenue using metadata from the TMDB 5000 Movies Dataset. The goal is to understand what factors contribute most to box office success.

## 📂 Dataset
- `tmdb_5000_movies.csv`
- `tmdb_5000_credits.csv`

## 🧪 Key Features Engineered
- **Genres**: extracted from JSON format
- **Top 3 Cast Members**: extracted per movie
- **Director**: extracted from crew column
- **Release Year/Month**: derived from date
- **TF-IDF Vectorized Metadata**: genres, cast, and director combined
- **Budget, Runtime, Popularity**: numeric predictors

## 🤖 Model
- Trained a **Random Forest Regressor**
- Achieved **R² ≈ 0.79** on test data
- Key drivers of revenue: **popularity**, **budget**

## 📊 Results
- Strong performance on most movies
- Struggled slightly on extremely high-budget blockbusters (common in real-world data)

## 📈 Tools Used
- Python, Pandas, NumPy, Scikit-learn, Matplotlib, Seaborn
- Jupyter Notebook

## 🔮 Next Steps
- Hyperparameter tuning
- Try other models (XGBoost, LightGBM)
- Incorporate more metadata (e.g., spoken_languages, keywords)
