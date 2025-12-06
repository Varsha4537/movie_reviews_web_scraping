# 🎬 Movie Reviews Web Scraping & Neurodivergence Analysis

This repository contains code and workflows for **scraping, filtering, and analyzing user reviews** and online discussions of movies and TV shows that portray **neurodivergence**.

Data is collected from **news articles, Reddit, Twitter/X, and YouTube comments**, cleaned and merged for downstream analysis — including **sentiment**, **topic modeling**, and **representation studies**.

---

## 📂 Repository Structure

- **movie_reviews_web_scraping/**
  - **Guardian_API_extraction.ipynb** – Scrape articles from The Guardian API  
  - **NY_API_Extraction.ipynb** – NYTimes or other news source scraping  
  - **Reddit_API.ipynb** – Reddit submissions & comment scraper (Async PRAW)  
  - **Twitter_API.ipynb** – Twitter/X scraper using free API tier  
  - **YT_Reviews.ipynb** – YouTube comment downloader for selected videos  
  - **data_preprocessing_code.ipynb** – Text cleaning and normalization  
  - **final_code.ipynb** – Merges datasets + neurodivergence filtering  
  - **lda_topic_modeling_all.html** – Topic modeling visualization output  


---

## 🎯 Project Objective

The goal of this project is to build a unified dataset that consolidates:

- Public reviews  
- Viewer comments  
- Media coverage  
- Social conversations  

...about movies and TV shows depicting **autism, ADHD, dyslexia, Tourette syndrome, and other forms of neurodivergence**.

This enables researchers and analysts to perform:

- Representation analysis  
- Sentiment trend tracking  
- Topic modeling  
- Cross-platform perception studies  

---

## 🛠️ Features

- ✔ Scrapes **media coverage** using The Guardian API  
- ✔ Collects **Reddit posts & comments** (asynchronous PRAW)  
- ✔ Extracts **Twitter/X posts** with Tweepy (free API tier)  
- ✔ Downloads **YouTube comments** for selected videos  
- ✔ Filters all content using customizable **neurodivergence keyword lists**  
- ✔ Merges all platforms into one consolidated dataset per movie  
- ✔ Supports advanced NLP analysis (Sentiment, Keyword, LDA Topic Modeling)

---
## Dependencies
pandas
requests
tweepy
praw
asyncpraw
youtube_comment_downloader
beautifulsoup4
nltk
gensim
scikit-learn


---

## 🔑 API Keys Setup

You will need API keys for:

- The Guardian API  
- Reddit API  
- Twitter/X API  
- YouTube API (optional)

Store keys securely in **environment variables** or a local `.env` file.  
🚫 **Do NOT commit** these keys to the repository.

Example `.env`:

GUARDIAN_API_KEY=your_guardian_key
REDDIT_CLIENT_ID=your_reddit_client_id
REDDIT_CLIENT_SECRET=your_reddit_secret
TWITTER_BEARER_TOKEN=your_twitter_token
YOUTUBE_API_KEY=your_youtube_key

---

## 📑 Workflow

### 1️⃣ Scrape Data
- Run `Guardian_API_extraction.ipynb` → Media articles  
- Run `Reddit_API.ipynb` → Reddit discussions  
- Run `Twitter_API.ipynb` → Tweets  
- Run `YT_Reviews.ipynb` → YouTube comments  

### 2️⃣ Preprocess Data
Use `data_preprocessing_code.ipynb` to:
- Clean and normalize text  
- Deduplicate entries  
- Unify review formats  

### 3️⃣ Merge & Filter
Use `final_code.ipynb` to:
- Merge all platform datasets  
- Apply neurodivergence keyword filters  
- Export consolidated CSV/Excel outputs  

### 4️⃣ Analyze (Optional)
Perform:
- Sentiment analysis  
- Keyword frequency analysis  
- Topic modeling (example output: `lda_topic_modeling_all.html`)

---

## 🔧 Customization

### Change Movie List
Edit the list/dictionary of movie titles inside each scraping notebook.

### Modify Neurodivergence Keywords
Update the keyword list (e.g., *autism, ADHD, dyslexia, stimming, sensory issues, neurodivergent, neurodiversity*, etc.) inside preprocessing or scraping scripts.

---

## ⚠️ Ethical & Legal Notes

- Respect **API rate limits** and **Terms of Service** for each platform.  
- **Do not distribute raw scraped data** containing user-identifiable content.  
- Use datasets and analyses **for academic or research purposes only**.  

---

## 📊 Example Outputs

| Analysis | Description |
|-----------|-------------|
| Sentiment Analysis | Detect positive/negative tone in public perceptions. |
| Topic Modeling | Identify thematic clusters related to neurodivergent representation. |
| Keyword Frequency | Explore commonly used descriptors and sentiments. |

---

## 🧠 Research Applications

This repository supports **digital media sociology**, **AI/NLP-based representation studies**, and **neurodivergent discourse analysis** across diverse media platforms.

---

