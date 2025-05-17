# 📺 YouTubeCommentHarvester

**YouTubeCommentHarvester** is a data pipeline that ingests **live YouTube comments** using the **YouTube Data API**, performs **text preprocessing and sentiment analysis**, and stores structured results in a **BigQuery data warehouse**. The system supports **scheduled batch jobs** and generates reports on **trending sentiments across video categories**.

This project demonstrates how to build a scalable, cloud-friendly NLP pipeline for real-time social media analysis.



## 📌 Features

- 🔄 **Live Comment Ingestion**:
  - Uses the YouTube Data API to fetch comments from videos, channels, or search queries
  - Supports configurable polling frequency and pagination

- 🧹 **Text Preprocessing**:
  - Removes emojis, links, and stop words
  - Normalizes text for model-ready input

- 💬 **Sentiment Analysis**:
  - Pre-trained models (e.g., TextBlob, Vader, or custom transformers)
  - Classifies comments into Positive / Negative / Neutral

- 🧠 **Categorical Aggregation**:
  - Groups results by video category (e.g., Music, Gaming, News)
  - Computes trending sentiment scores over time

- ⏰ **Batch Scheduling**:
  - Scheduled jobs using Cloud Composer (Airflow) or cron
  - Batches comment ingestion and sentiment scoring

- 🧾 **BigQuery Data Warehouse**:
  - Stores raw, processed, and scored comment data
  - Optimized schema for analytics and dashboarding



## 🛠️ Tech Stack

- **APIs**: YouTube Data API v3
- **Data Processing**: Python, Pandas
- **NLP & Sentiment Analysis**: TextBlob, Vader, or HuggingFace Transformers
- **Orchestration**: Apache Airflow (Cloud Composer optional)
- **Data Warehouse**: Google BigQuery
- **Visualization (optional)**: Google Data Studio / Looker Studio



## 🚀 Getting Started

### Prerequisites

- Python 3.8+
- Google Cloud account with BigQuery enabled
- YouTube API Key
- GCP SDK installed and authenticated

### Install Dependencies

```bash
git clone https://github.com/your-username/YouTubeCommentHarvester.git
cd YouTubeCommentHarvester
pip install -r requirements.txt
