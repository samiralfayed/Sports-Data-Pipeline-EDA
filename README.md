#  Sports Data Pipeline + EDA + Prediction

##  Objective
Build an end-to-end pipeline to clean, analyze, and predict outcomes based on real-world football player appearance data.

---

##  Dataset
- Source: [Kaggle - Player Scores Dataset](https://www.kaggle.com/datasets/davidcariboo/player-scores)
- File Used: `appearances.csv`
- Records: ~25,000 rows of match-level player appearances
- Fields include: player ID, minutes played, goals, assists, yellow/red cards, match ID, and club

---

##  Data Cleaning
- Dropped missing or irrelevant entries (e.g., players with 0 minutes)
- Parsed and converted date, goals, cards, assists to numeric
- Handled missing values and dropped duplicates
- Created new binary column `scored` indicating if a player scored in a match

---

##  Exploratory Data Analysis (EDA)
- Distribution of minutes played
- Top 10 scorers
- Top 10 assist providers
- Most penalized players (yellow + red cards)
- Goal trend over time

---

##  Machine Learning: Predicting If a Player Scores
- Binary classification: Will a player score in a match?
- Model: Logistic Regression
- Features used: `minutes_played`, `assists`, `yellow_cards`, `red_cards`
- Target: `scored` (1 if goals > 0, else 0)

###  Performance:
- **Accuracy**: 91.32%
- **Confusion Matrix**:  (visualized)
- **ROC Curve + AUC**:  included

---


##  Video Demo
https://drive.google.com/file/d/142QktaEPLAXauDPhVLizugN1VEBrSNkG/view?usp=sharing




---

##  Tools & Libraries
- Python, Pandas, Seaborn, Matplotlib, Plotly
- Scikit-learn (LogisticRegression, metrics)
- Google Colab (for notebook execution)

---

##  Contact
**Md. Samir Al Fayed Ifti**  
samiralfayedifti001@gmail.com

