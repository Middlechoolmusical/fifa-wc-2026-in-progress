# FIFA World Cup Predictor & Simulator 🏆 (In Progress)

This is a prototype of a FIFA World Cup Predictor. It currently features a basic machine learning model trained on historical World Cup matches and tournament qualifiers, with a clean Streamlit interface to predict individual matches.

This project is marked as **In Progress** as we work to build a full tournament simulation engine.

---

## 📂 Project Files

* **`results.csv`**: Raw dataset containing historical international match results from 1872 to the present.
* **`app.py`**: A Streamlit application that loads the dataset, filters for World Cup fixtures, trains a Random Forest Classifier on historical match pairs, and predicts win/draw/loss probabilities for any selected teams.
* **`README.md`**: Project documentation and development roadmap.

---

## ⚡ Setup & Run

### 1. Install dependencies
```bash
pip install streamlit pandas scikit-learn
```

### 2. Launch the Web UI
```bash
streamlit run app.py
```

---

## 🛠️ Development Roadmap (Planned Features)

The current model is a simple head-to-head match predictor. In future updates, we plan to implement:
1. **Dynamic Elo Rating System**: Instead of simple team codes, we will calculate dynamic rating strengths for each country based on their historical results (giving more weight to recent matches and competitive tournaments).
2. **Monte Carlo Tournament Simulation**: We will build an engine that simulates all 8 groups in the World Cup round-robin stage, determines who qualifies, generates the knockout brackets (Round of 16, Quarterfinals, Semifinals, Final), and runs the entire tournament 10,000 times to calculate the probability of each country winning the World Cup.
