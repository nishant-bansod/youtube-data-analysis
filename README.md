# YouTube Data Analysis Project

**Company Name:** YouTube (Google)

**Problem:** Understanding user engagement patterns and content performance across different countries and categories to optimize content strategy and improve user experience.

## Simple Insights:

• **Sentiment Analysis:** 38.9% positive, 49.1% neutral, 11.9% negative comments across 691K+ user comments

• **Category Performance:** Music leads with 158,632 average likes, followed by Comedy (38,771) and Nonprofits & Activism (30,698)

• **Top Trending Channel:** The Late Show with Stephen Colbert with 710 trending videos

• **Engagement Metrics:** 3.64% like rate, 0.22% dislike rate, 0.57% comment rate

• **Geographic Coverage:** Analysis across 10 countries (US, CA, DE, FR, GB, IN, JP, KR, MX, RU)

• **Most Used Emojis:** 😂 (36,987 times), 😍 (33,453 times), ❤️ (31,119 times)

## Aims Grid:

• **Purpose of the project:** To analyze YouTube trending videos and user engagement patterns to extract actionable insights about content performance, user sentiment, and engagement metrics across multiple countries

• **Stakeholders:** Content Creators, Marketing Teams, Data Analytics Teams, Product Managers, Business Intelligence Teams

• **End Result:** Comprehensive analysis providing insights into user sentiment, category performance, channel success factors, and engagement patterns to support data-driven content strategy decisions

• **Success Criteria:**
    - Successfully analyzed 691K+ comments and 339K+ video records
    - Identified key performance indicators for content categories
    - Generated actionable insights for content optimization
    - Created multiple data export formats for stakeholder consumption
    - Demonstrated proficiency in data analysis, sentiment analysis, and visualization

## Dataset Information:

**Video Data:**
- Countries: US, CA, DE, FR, GB, IN, JP, KR, MX, RU
- Total Videos: 339,525 (after deduplication)
- Categories: 18 different video categories
- Time Period: 2017-2018 trending data

**Comments Data:**
- Total Comments: 691,374
- Features: video_id, comment_text, likes, replies
- Sentiment Analysis: Polarity scores (-1 to 1)

## Key Visualizations:

![Sentiment Analysis](screenshots/sentiment_analysis.png)
*Distribution of sentiment polarity across user comments*

![Category Performance](screenshots/category_performance.png)
*Average likes by video category*

![Word Cloud](screenshots/word_cloud.png)
*Word cloud visualization of positive comments*

![Channel Analysis](screenshots/channel_analysis.png)
*Top channels by number of trending videos*

## Concepts Used:

• **Data Cleaning & Preprocessing:** Handling missing values, removing duplicates, data validation

• **Sentiment Analysis:** TextBlob implementation for polarity scoring

• **Statistical Analysis:** Correlation analysis, descriptive statistics, pattern recognition

• **Data Visualization:** Matplotlib, Seaborn for charts, histograms, heatmaps, word clouds

• **Database Management:** SQLite integration for data storage and retrieval

• **Feature Engineering:** Creating engagement metrics (like_rate, comment_rate, dislike_rate)

• **Exploratory Data Analysis:** Understanding data distribution and relationships

## Technologies Used:

- **Python 3.x**
- **Pandas, NumPy** - Data manipulation and analysis
- **Matplotlib, Seaborn** - Data visualization
- **TextBlob, WordCloud** - Natural language processing
- **SQLite, SQLAlchemy** - Database management
- **Jupyter Notebook** - Development environment

## Installation:

```bash
git clone https://github.com/nishant-bansod/youtube-data-analysis.git
cd youtube-data-analysis
pip install pandas numpy matplotlib seaborn textblob wordcloud sqlalchemy emoji
jupyter notebook youtube_data_analysis.ipynb
```

**GitHub Repository:** [https://github.com/nishant-bansod/youtube-data-analysis](https://github.com/nishant-bansod/youtube-data-analysis)

