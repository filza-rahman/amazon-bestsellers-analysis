# amazon-bestsellers-analysis
An exploratory data analysis of Amazon's Top 50 Bestselling Books from 2009 to 2019, examining genre trends, author dominance, pricing patterns, and reader ratings across a decade of bestseller data.

---

## Overview

This project investigates what patterns emerge among 550 Amazon bestseller entries spanning 2009–2019. The analysis explores how genre, price, reviews, and publication year relate to a book's bestseller presence — and where the surprising outliers lie.

**Questions explored:**
- Does Fiction or Non-Fiction dominate the bestseller list?
- Which authors appeared most frequently across the decade?
- Is there a relationship between price and rating?
- How did genre representation shift year over year?

---

## Dataset

**Source:** [Amazon Top 50 Bestselling Books 2009–2019](https://www.kaggle.com/datasets/sootersaalu/amazon-top-50-bestselling-books-2009-2019) — Kaggle  
**Size:** 550 entries × 7 columns | No missing values

| Column | Description |
|---|---|
| `Name` | Book title |
| `Author` | Author name |
| `User Rating` | Average rating (3.3 – 4.9 out of 5) |
| `Reviews` | Number of user reviews (37 – 87,841) |
| `Price` | Price in USD ($0 – $105) |
| `Year` | Year the book appeared on the list |
| `Genre` | Fiction or Non-Fiction |

---

## Analysis Highlights

| Section | Chart Type | Finding |
|---|---|---|
| Genre Distribution | Bar chart | Non-Fiction (310) edges out Fiction (240) overall |
| Top 10 Authors | Horizontal bar | Jeff Kinney, Suzanne Collins, Rick Riordan dominate |
| Avg Rating by Genre | Bar chart | Fiction averages 4.65 vs Non-Fiction 4.60 |
| Yearly Bestseller Trends | Line plot | 2014 was the peak Fiction year; Non-Fiction leads most others |
| Price vs. Rating | Scatter plot | No meaningful correlation — price doesn't predict quality |
| Correlation Heatmap | Heatmap | Price and Reviews have a slight negative correlation |

### Notable data points
- **Most reviewed book:** *Where the Crawdads Sing* — 87,841 reviews (Fiction)
- **Most expensive:** *DSM-5* at $105, appearing twice (Non-Fiction)
- **Lowest rated bestseller:** *The Casual Vacancy* at 3.3 stars
- **12 books listed at $0** — likely Kindle editions at time of data collection
- **Gary Chapman** appeared across the most distinct years (11), followed closely by Jeff Kinney

---

## Repository Structure

```
amazon-bestsellers-analysis/
│
├── amazon/
│   ├── amazon_bestsellers.ipynb   # Main analysis notebook
│   └── bestsellers.csv            # Dataset
│
└── README.md
```

---

## Tech Stack

- **Python 3**
- **pandas** — data loading, cleaning, aggregation
- **matplotlib** — all visualizations

---

## Getting Started

**1. Clone the repository**
```bash
git clone https://github.com/filza-rahman/amazon-bestsellers-analysis.git
cd amazon-bestsellers-analysis
```

**2. Install dependencies**
```bash
pip install pandas matplotlib notebook
```

**3. Launch the notebook**
```bash
jupyter notebook amazon/amazon_bestsellers.ipynb
```
---

*Dataset credit: [Souter Saalu on Kaggle](https://www.kaggle.com/datasets/sootersaalu/amazon-top-50-bestselling-books-2009-2019).*

♡♡♡♡
