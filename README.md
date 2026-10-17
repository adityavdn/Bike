# Bike Sharing Demand

Linear regression analysis of daily bike-sharing demand (`cnt`) based on weather and seasonal features.

## What the notebook does

- Loads the daily bike-sharing data (`day.csv`)
- Turns coded columns (season, weather situation, month, weekday) into readable labels
- Drops columns that leak the target or are just indexes (`instant`, `casual`, `registered`)
- Explores correlations between the numeric features
- One-hot encodes the categorical variables, scales the features and fits a linear regression model on a train/test split

## Data

Uses `day.csv` from the [UCI Bike Sharing Dataset](https://archive.ics.uci.edu/dataset/275/bike+sharing+dataset). It isn't included in this repo. Download it, then update the path in the `pd.read_csv(...)` cell.

## Running it

```bash
pip install -r requirements.txt
jupyter notebook "bike 1.ipynb"
```
