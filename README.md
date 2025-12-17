# ⚽ Predictive Soccer Analytics

A Python machine learning project that predicts soccer match outcomes using advanced performance metrics such as **Expected Goals (xG)** and **Expected Goals Against (xGA)**.

---

## 📌 Project Overview

Traditional soccer statistics (shots, possession, goals) often fail to capture true team performance. This project leverages **expected goals–based analytics** to model match outcomes more accurately using supervised machine learning techniques.

The goal is to explore how underlying chance quality and defensive strength translate into match results and to build a scalable prediction pipeline.

---

## 🔍 Features

- Match outcome prediction (Win / Draw / Loss)
- Feature engineering using xG and xGA
- Train/test evaluation with multiple ML models
- Reproducible data preprocessing pipeline
- Extensible framework for additional metrics (shots, possession, Elo, etc.)

---

## 📊 Data

This project uses **public, historical match-level expected goals (xG) data** from Europe’s top five leagues
(Premier League, La Liga, Bundesliga, Serie A, and Ligue 1).

Each raw match record includes:

- **Home team xG**
- **Away team xG**
- Final score (used for label generation)
- Match metadata (date, venue, referee, attendance)

### Feature Engineering

Some stats used by the model are **created from the raw data**, including:

- **xGA (Expected Goals Against)** — computed as opponent xG  
- Rolling team form metrics (e.g. last *N* matches xG / xGA)
- Home vs. away performance splits
- Match outcome labels (win / draw / loss)

### Notes

- No private or paid APIs are required  
- All features are generated from raw xG match data  
- The preprocessing pipeline is fully reproducible
  
> Raw data comes from [OpenDataBay: Big Five Football xG Data](https://www.opendatabay.com/data/dataset/bbb1a478-5f55-4c6e-84f0-63596624f1f6). The preprocessing scripts in `src/data/` assume the CSVs are downloaded locally.

---

## 🧠 Models

Initial models explored:

- Logistic Regression (baseline)
- Random Forest
- XGBoost

Model performance is evaluated using:
- Accuracy
- Precision / Recall
- Confusion Matrix
- Cross-validation

---

## 📈 Results

Will be posted after more testing and implementation.

---

## 🧪 Future Improvements

- Add player-level features
- Incorporate betting odds or Elo ratings
- Multi-class vs regression (goal difference)
- Time-series modeling for form and momentum
- Web app or API deployment

---

## 📄 License

This project is licensed under the MIT License.

---

## 📬 Contact

Created by Ryan Spencer
If you’re interested in soccer analytics, machine learning, or collaboration, feel free to reach out!

