# Text Mining and Sentiment Analysis on Yelp Reviews

A text mining project that quantifies sentiment and text quality across 10,000 Yelp
reviews and relates them to user engagement attributes.

> **Note on dates:** This project was originally completed in December 2019 as part of
> my MS in Business Analytics at California State University, East Bay. It was uploaded
> to GitHub in June 2026 after my previous GitHub account was deleted. Commit dates are
> set to reflect the original completion date.

## Overview

This project works with a dataset of 10,000 Yelp text reviews. Each review carries
attributes such as Stars, Useful, Funny, and Cool. The data is explored through summary
statistics and visualizations. Sentiment analysis quantifies the amount of positive,
negative, and neutral sentiment in each review. Text quality is measured using TF-IDF
and Lexical Diversity, and these measures are placed in a linear model that relates
Yelp's engagement attributes (Useful, Funny, Cool) to text quality.

## Dataset

- **Source:** Yelp reviews dataset from Kaggle
- **Size:** 10,000 reviews, 10 columns
- **Attributes:** `business_id`, `date`, `review_id`, `text`, `type`, `user_id`,
  `stars`, `cool`, `useful`, `funny`
  - `business_id`, `review_id`, `user_id` are unique identifiers
  - `stars` is a categorical rating from 1 to 5
  - `cool`, `useful`, `funny` are vote counts from other users

## Steps Performed

1. **Exploratory data analysis** with summary statistics
2. **Word Cloud** visualization of review text
3. **Correlation analysis and heat maps** of the parameters
4. **Cross tabulation** between parameters
5. **Sentiment analysis** with polarity scores
6. **Text quality measures** using TF-IDF and Lexical Diversity
7. **Linear model** relating engagement attributes to text quality

## Tech Stack

Python, Pandas, NumPy, Matplotlib, Seaborn, NLTK / TextBlob, WordCloud, Scikit-learn,
Jupyter Notebook.

## Files

- `TextminingKedar.ipynb` - main notebook
- `textminingkedar.py` - Python script export
- `Text Mining Final .docx.pdf` - project report
- `Project Overview.docx` - project summary

## How to Run

```bash
git clone https://github.com/kedar-patil-engineer/yelp-sentiment-analysis-text-mining.git
cd yelp-sentiment-analysis-text-mining
python -m venv venv
venv\Scripts\activate          # Windows  (use: source venv/bin/activate on macOS/Linux)
pip install -r requirements.txt
jupyter notebook
```

Then open `TextminingKedar.ipynb` and run all cells.

## License

This project is released under the MIT License. See [LICENSE](LICENSE).

## Author

Kedar Patil - MS Business Analytics, California State University, East Bay
