# YouTube Data Analysis Project

Analysis of YouTube trending videos and user engagement patterns across multiple countries.

## Overview

This project analyzes YouTube trending videos and user comments to extract insights about content performance, user engagement, and sentiment patterns. The analysis covers 10 countries and 691,374 comments from trending videos.

## Key Results

- Average Sentiment Polarity: 0.138 (slightly positive)
- Most Engaging Category: Music (158,632 average likes)
- Top Trending Channel: The Late Show with Stephen Colbert (710 trending videos)
- Engagement Metrics: 3.64% like rate, 0.22% dislike rate, 0.57% comment rate
- Sentiment Distribution: 38.9% Positive, 49.1% Neutral, 11.9% Negative comments

## Analysis Features

- Sentiment Analysis using TextBlob
- Word Cloud Generation for positive/negative sentiment
- Emoji Usage Analysis
- Category Performance Analysis
- Channel Trending Analysis
- Engagement Metrics Calculation
- Content Characteristics Analysis
- Data Export (CSV, JSON, SQLite)

## Technologies Used

- Python 3.x
- Pandas, NumPy
- Matplotlib, Seaborn
- TextBlob, WordCloud
- SQLite, SQLAlchemy
- Jupyter Notebook

## Installation

1. Clone the repository
   ```bash
   git clone https://github.com/nishant-bansod/youtube-data-analysis.git
   cd youtube-data-analysis
   ```

2. Install required packages
   ```bash
   pip install pandas numpy matplotlib seaborn textblob wordcloud sqlalchemy emoji
   ```

3. Run the analysis
   ```bash
   jupyter notebook youtube_data_analysis.ipynb
   ```

## Dataset Information

### Video Data
- Countries: US, CA, DE, FR, GB, IN, JP, KR, MX, RU
- Total Videos: 339,525 (after deduplication)
- Categories: 18 different video categories
- Time Period: 2017-2018 trending data

### Comments Data
- Total Comments: 691,374
- Features: video_id, comment_text, likes, replies
- Sentiment Analysis: Polarity scores (-1 to 1)

## Top Categories by Average Likes

1. Music (158,632 avg likes)
2. Comedy (38,771 avg likes)
3. Nonprofits & Activism (30,698 avg likes)
4. Science & Technology (27,634 avg likes)
5. Entertainment (24,421 avg likes)
6. Gaming (24,131 avg likes)
7. Film & Animation (23,875 avg likes)
8. Movies (19,808 avg likes)
9. Howto & Style (17,479 avg likes)
10. Sports (15,426 avg likes)

## Usage Example

```python
import pandas as pd
from textblob import TextBlob

# Load data
comments = pd.read_csv('data/UScomments.csv')
videos = pd.read_csv('additional_data/USvideos.csv')

# Analyze sentiment
polarity = TextBlob("This video is amazing!").sentiment.polarity
print(f"Sentiment polarity: {polarity}")
```

## Author

Nishant Bansod
- GitHub: [@nishant-bansod](https://github.com/nishant-bansod)
