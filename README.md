# Player Subscription Prediction

## Project Overview

In the realm of gaming communities, maintaining player engagement and communication is critical for long-term success. One strategy is to encourage players to subscribe to newsletters, providing updates, event information, and community news. However, it is not always clear which players are most likely to subscribe based on their in-game behavior and characteristics.

This project investigates the relationship between player attributes and newsletter subscription behavior within a gaming environment.  
Specifically, it seeks to answer: **Which player characteristics and behaviors are most predictive of subscribing to a game-related newsletter, and how do these features differ across various player types?**

Understanding these dynamics will help gaming communities and developers design better outreach strategies and enhance player retention.

---

## Data Description

The analysis uses a dataset containing player information collected from an online multiplayer game environment.

Each row in the dataset represents an individual player. Below is a summary of the key variables:

| Variable Name   | Description | Type | Notes |
|:----------------|:------------|:-----|:------|
| experience      | Player's self-reported experience level (e.g., Noob, Pro, Veteran) | Categorical | Ordered |
| subscribe       | Whether the player is subscribed to the newsletter (TRUE/FALSE) | Boolean | Target variable |
| played_hours    | Total number of hours played on the server | Numeric | Includes both active and idle time |
| age             | Player's age in years | Numeric | Some age ranges may be underrepresented |
| gender          | Player's gender identity | Categorical | Possible data imbalance |
| additional features | Various other gameplay or personal attributes | Mixed | May require feature engineering |

---

## Methodology

To explore and model the subscription behavior:

### 1. Exploratory Data Analysis (EDA)
- Visualize distributions of key variables (e.g., age, experience level, playtime).
- Analyze correlations between player behaviors and subscription rates.

### 2. Predictive Modeling
- Use classification models (e.g., logistic regression, decision trees) to predict newsletter subscription.
- Perform feature importance analysis to identify the most influential factors.
- Compare model performance using accuracy, precision, recall, and AUC metrics.

### 3. Player Type Comparison
- Segment players based on characteristics such as experience level or playing time.
- Investigate how predictive features vary across different player groups.

---

## Justification for Methodology

- **Logistic Regression** provides clear interpretability, ideal for understanding how individual features influence subscription likelihood.
- **Decision Trees** are included to capture non-linear relationships and offer intuitive visualization of decision rules.
- Feature importance analysis helps prioritize player traits for targeted outreach strategies.
- The choice of models ensures scalability as player data grows over time.

---

## Project Goals

- Identify behavioral and demographic factors most associated with newsletter subscription.
- Differentiate predictors across various player types to inform tailored communication strategies.
- Provide actionable insights for community managers and developers seeking to grow and engage their player base.

---

## Technologies Used

- Python
- Pandas, NumPy
- Scikit-learn
- Matplotlib, Seaborn
- Jupyter Notebook

---

## License

This project is available for educational and research purposes.

---
*Developed as part of a Data Science initiative exploring predictive analytics in gaming communities.*
