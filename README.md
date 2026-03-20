# NCAAB Historical Closing Odds Dataset (2008–2026)

**76,449 matches · 18 seasons · American Moneyline format · ML-ready**

Free 50-row structural sample. Full dataset available on [Gumroad](https://sportsdataolivier.gumroad.com/l/chbrtv).

---

## Dataset specifications

| Field | Value |
|---|---|
| Total matches | 76,449 |
| Seasons | 2008/2009 → 2025/2026 |
| Odds type | Moneyline closing (American format) |
| Coverage | Full NCAAB market — including obscure divisions and non-conference games |
| Missing values | 0 |
| Separator | Semicolon (`;`) |
| Encoding | UTF-8 |

---

## Columns

| Column | Description |
|---|---|
| `Country` | Country where the match was played (USA) |
| `League` | League identifier (NCAAB) |
| `Date` | Official match date |
| `Type` | Match phase: Regular Season or Play Offs |
| `Home_Team` | Name of the home collegiate team |
| `Home_Points` | Final points scored by the home team |
| `Away_Points` | Final points scored by the away team |
| `Away_Team` | Name of the away collegiate team |
| `Note` | Special condition: OT (Overtime) or empty |
| `Odds_Home` | Moneyline closing odds — home team (American format) |
| `Odds_Away` | Moneyline closing odds — away team (American format) |
| `End_Of_RT` | Result at end of regular time: Home, Away, or Draw |
| `Number of Points - TOTAL` | Combined score of both teams |
| `Number of Points - INTERVAL` | Categorical bin of total points scored |
| `Winning Margin` | Point differential between winning and losing team |

---

## Quickstart

```python
import pandas as pd

df = pd.read_csv('Sample_NCAAB.csv', sep=';')

print(df.shape)
# (50, 15)

print(df.isnull().sum().sum())
# 0

print(df.head())
```

---

## EDA notebook

Full exploratory analysis — schema, missing values check, odds distribution,
implied probability validation, and XGBoost feature matrix example:

[kaggle.com/code/oliviersportsdata/ncaab-closing-odds-18-seasons-market-analysis](https://www.kaggle.com/code/oliviersportsdata/ncaab-closing-odds-18-seasons-market-analysis)

---

## Full dataset

The complete 76,449-match archive is available here:

[sportsdataolivier.gumroad.com/l/chbrtv](https://sportsdataolivier.gumroad.com/l/chbrtv)

---

## License

This sample is released for research and educational purposes.  
Redistribution or resale of the purchased full dataset is strictly prohibited.

---

*Olivier Vignez — Sports Betting Data Engineer*  
[sportsdataolivier.gumroad.com](https://sportsdataolivier.gumroad.com)
