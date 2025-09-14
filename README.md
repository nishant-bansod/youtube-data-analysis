# 📊 YouTube Data Analysis Project

A comprehensive analysis of YouTube trending videos and user engagement patterns across multiple countries using Python data science tools.

## 🌟 Overview

This project analyzes YouTube trending videos and user comments to extract valuable insights about content performance, user engagement, and sentiment patterns. The analysis covers **10 countries** and **691,374 comments** from trending videos.

## 📈 Key Insights

- **Average Sentiment Polarity:** 0.138 (slightly positive)
- **Most Engaging Category:** Music (158,632 average likes)
- **Top Trending Channel:** The Late Show with Stephen Colbert (710 trending videos)
- **Engagement Metrics:** 3.64% like rate, 0.22% dislike rate, 0.57% comment rate
- **Sentiment Distribution:** 38.9% Positive, 49.1% Neutral, 11.9% Negative comments

## 🎯 Features

### ✅ Completed Analyses
- **Sentiment Analysis** - TextBlob analysis of user comments
- **Word Cloud Generation** - Visual representation of positive/negative sentiment
- **Emoji Usage Analysis** - Top 10 most used emojis (😂, 😍, ❤️)
- **Category Performance Analysis** - Performance metrics by video category
- **Channel Trending Analysis** - Most successful channels
- **Engagement Metrics Calculation** - Like, dislike, and comment rates
- **Content Characteristics Analysis** - Title punctuation impact
- **Multi-format Data Export** - CSV, JSON, and SQLite outputs

### 📊 Visualizations
- Sentiment polarity distribution histograms
- Word clouds for positive and negative comments
- Emoji frequency bar charts
- Category performance box plots
- Channel trending bar charts
- Correlation heatmaps
- Engagement metrics visualizations

## 🛠 Technologies Used

- **Python 3.x**
- **Data Processing:** Pandas, NumPy
- **Visualization:** Matplotlib, Seaborn
- **Natural Language Processing:** TextBlob, WordCloud
- **Database:** SQLite, SQLAlchemy
- **Development:** Jupyter Notebook

## 📁 Project Structure

```
YouTube_Data_Analysis_Project/
├── 📊 Data Sources
│   ├── additional_data/          # Video datasets from 10 countries
│   │   ├── CAvideos.csv, USvideos.csv, etc.
│   │   └── CA_category_id.json, etc.
│   ├── data/                     # User comments dataset
│   │   └── UScomments.csv (691,374 comments)
│   └── exports/                   # Processed data outputs
│       ├── youtube_analysis_sample.csv
│       ├── youtube_analysis_sample.json
│       └── youtube_analysis_sample.sqlite
├── 📓 Analysis Notebook
│   └── youtube_data_analysis.ipynb
├── 📄 Documentation
│   ├── README.md
│   └── README.txt
└── 🔧 Configuration
    └── .gitignore
```

## 🚀 Getting Started

### Prerequisites
- Python 3.7+
- Jupyter Notebook
- Required Python packages (see installation below)

### Installation

1. **Clone the repository**
   ```bash
   git clone https://github.com/yourusername/youtube-data-analysis.git
   cd youtube-data-analysis
   ```

2. **Install required packages**
   ```bash
   pip install pandas numpy matplotlib seaborn textblob wordcloud sqlalchemy emoji
   ```

3. **Run the analysis**
   ```bash
   jupyter notebook youtube_data_analysis.ipynb
   ```

## 📊 Dataset Information

### Video Data
- **Countries:** US, CA, DE, FR, GB, IN, JP, KR, MX, RU
- **Total Videos:** 339,525 (after deduplication)
- **Categories:** 18 different video categories
- **Time Period:** 2017-2018 trending data

### Comments Data
- **Total Comments:** 691,374
- **Features:** video_id, comment_text, likes, replies
- **Sentiment Analysis:** Polarity scores (-1 to 1)

## 🔍 Analysis Results

### Top 10 Most Used Emojis
1. 😂 (36,987 times)
2. 😍 (33,453 times)
3. ❤️ (31,119 times)
4. 🔥 (8,694 times)
5. 😭 (8,398 times)
6. 👏 (5,719 times)
7. 😘 (5,545 times)
8. 👍 (5,476 times)
9. 💖 (5,359 times)
10. 💕 (5,147 times)

### Top 10 Categories by Average Likes
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

## 📈 Usage Examples

### Basic Data Loading
```python
import pandas as pd
import numpy as np

# Load comments data
comments = pd.read_csv('data/UScomments.csv')
print(f"Loaded {len(comments)} comments")

# Load video data
videos = pd.read_csv('additional_data/USvideos.csv')
print(f"Loaded {len(videos)} videos")
```

### Sentiment Analysis
```python
from textblob import TextBlob

# Analyze sentiment
polarity = TextBlob("This video is amazing!").sentiment.polarity
print(f"Sentiment polarity: {polarity}")
```

## 🤝 Contributing

1. Fork the repository
2. Create a feature branch (`git checkout -b feature/AmazingFeature`)
3. Commit your changes (`git commit -m 'Add some AmazingFeature'`)
4. Push to the branch (`git push origin feature/AmazingFeature`)
5. Open a Pull Request

## 📝 License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

## 👨‍💻 Author

**Your Name**
- GitHub: [@yourusername](https://github.com/yourusername)
- LinkedIn: [Your LinkedIn](https://linkedin.com/in/yourprofile)

## 🙏 Acknowledgments

- YouTube for providing the dataset
- The Python data science community for excellent libraries
- Contributors and reviewers

## 📞 Contact

If you have any questions or suggestions, feel free to reach out:
- Email: your.email@example.com
- GitHub Issues: [Create an issue](https://github.com/yourusername/youtube-data-analysis/issues)

---

⭐ **Star this repository if you found it helpful!**
