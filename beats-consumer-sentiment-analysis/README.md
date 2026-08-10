# Beats by Dre Consumer Sentiment Analysis

An end-to-end Python NLP and exploratory data analysis project analyzing Amazon customer reviews for Beats Solo 4 and competing headphone products.

## Project Overview

The project analyzes consumer feedback to understand:

- Customer satisfaction and rating distributions
- Positive, neutral, and negative sentiment
- Product-level sentiment differences
- Consumer preferences around comfort, fit, sound quality, battery life, and ANC
- Competitive positioning
- Potential product and marketing improvements

The original project workflow used Amazon reviews collected through the Oxylabs API, followed by data cleaning, EDA, TextBlob sentiment analysis, Gemini AI-assisted insight extraction, and competitive analysis.

## Repository Structure

```text
beats-consumer-sentiment-analysis/
│
├── notebooks/
│   └── beats_consumer_sentiment_analysis.ipynb
│
├── data/
│   ├── raw/
│   │   └── reviews.csv              # Add original dataset here (not included)
│   └── sample/
│       └── README.md
│
├── outputs/
│   └── README.md
│
├── .env.example
├── .gitignore
├── requirements.txt
├── DATA_DICTIONARY.md
└── README.md
```

## Dataset

The original report describes review fields including:

`review_id`, `product_name`, `product_id`, `title`, `author`, `rating`, `content`, `timestamp`, `profile_id`, `is_verified`, `helpful_count`, and `product_attributes`.

The raw Amazon review dataset is not included in this repository package. Add it locally as:

```text
data/raw/reviews.csv
```

Do not commit restricted, private, licensed, or API-derived data unless you have the right to redistribute it.

## How to Run

### 1. Clone the repository

```bash
git clone <your-github-repository-url>
cd beats-consumer-sentiment-analysis
```

### 2. Create a virtual environment

```bash
python -m venv .venv
```

Windows:

```bash
.venv\Scripts\activate
```

macOS/Linux:

```bash
source .venv/bin/activate
```

### 3. Install dependencies

```bash
pip install -r requirements.txt
```

### 4. Add the dataset

Place the original review dataset here:

```text
data/raw/reviews.csv
```

### 5. Open the notebook

```bash
jupyter notebook notebooks/beats_consumer_sentiment_analysis.ipynb
```

Or use VS Code / Google Colab.

## Analysis Pipeline

1. Load review data
2. Standardize column names
3. Handle missing values
4. Normalize product names
5. Parse timestamps
6. Remove duplicates
7. Clean review text
8. Generate descriptive statistics
9. Visualize rating distributions
10. Apply TextBlob sentiment analysis
11. Categorize sentiment
12. Compare products
13. Explore consumer themes
14. Optionally use Gemini AI for qualitative summaries
15. Export cleaned data and analysis tables

## Key Technologies

- Python
- Pandas
- NumPy
- Matplotlib
- Seaborn
- TextBlob
- SciPy
- Jupyter Notebook
- Optional: Gemini API
- Original data collection: Oxylabs API

## Important Reproducibility Note

The project report contains aggregate findings such as the reported Beats Solo 4 average rating of 4.56 and an overall sentiment split of approximately 80% positive, 15% neutral, and 5% negative. Those values are not hard-coded into the notebook. The notebook calculates results from the raw dataset so the analysis remains reproducible and transparent.

## Portfolio Skills Demonstrated

- Data cleaning and preprocessing
- Exploratory data analysis
- Statistical analysis
- NLP
- Sentiment analysis
- Feature engineering
- Data visualization
- Competitive benchmarking
- Business insight generation
- AI-assisted qualitative analysis
- Translating analytics into recommendations
