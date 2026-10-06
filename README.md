# Pakistan Housing Market — Exploratory Data Analysis

An exploratory analysis of about 99,000 property listings from Pakistan's five largest markets (Karachi, Lahore, Islamabad, Rawalpindi, Faisalabad), looking at how sale prices and rents vary by city, property type, size and neighbourhood.

## Key findings

- Sale and rent are two separate markets: the typical sale listing is PKR 12.1M, the typical rent PKR 50k per month.
- Lahore is the most expensive city to buy in, both in total price (median PKR 14.0M) and per Marla (PKR 2.0M).
- Location matters more than size: price per Marla differs about 5x between the most and least expensive neighbourhoods.
- Houses cost about twice as much as flats, to buy and to rent.
- Flats give a higher gross rental yield than houses in every city with rental data (4.0% to 7.6% a year overall).

## Files

| File | Contents |
|---|---|
| `house-price-eda.ipynb` | The analysis: data quality checks, feature engineering, charts and findings |
| `Cleaned_data_for_model.csv` | Pre-cleaned extract of the dataset (area unified to Marla) |

## Data

Source: [House Prices 2023 Dataset](https://www.kaggle.com/datasets/howisusmanali/house-prices-2023-dataset/data) on Kaggle.
Prices are in Pakistani Rupees (PKR); area is in Marla (1 Kanal = 20 Marla).

## Run it

```bash
pip install pandas numpy matplotlib seaborn notebook
jupyter notebook house-price-eda.ipynb
```

## Limitations

- The extract has no sale listings above PKR 45M, so the luxury market is not covered.
- Lahore has no rental listings in this extract.
- Prices are asking prices from listings, not completed transactions.
