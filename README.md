# 🎬 Movie Reviews Web Scraping & Neurodivergence Analysis

This repository contains code and workflows for scraping, filtering, and analyzing user reviews and online discussions of movies and TV shows that portray neurodivergence.  
Data is collected from **news articles, Reddit, Twitter, and YouTube comments**, and then cleaned and merged for downstream analysis (e.g., sentiment, topic modeling, representation studies).

---

## 📁 Repository Structure



movie_reviews_web_scraping/
├── Guardian_API_extraction.ipynb # Scrape articles from The Guardian API
├── NY_API_Extraction.ipynb # NYTimes or other news source scraping
├── Reddit_API.ipynb # Reddit submissions & comment scraper (Async PRAW)
├── Twitter_API.ipynb # Twitter/X scraper using free API tier
├── YT_Reviews.ipynb # YouTube comment downloader for selected videos
├── data_preprocessing_code.ipynb # Text cleaning and normalization
├── final_code.ipynb # Merges datasets + neurodivergence filtering
└── lda_topic_modeling_all.html # Topic modeling visualization output


---

## 🎯 Project Objective

The goal of this project is to build a unified dataset covering:

- Public reviews  
- Viewer comments  
- Media coverage  
- Social conversations  

…about movies and TV shows that depict **autism, ADHD, dyslexia, Tourette syndrome, and other forms of neurodivergence**.

This enables:

- Representation analysis  
- Sentiment tracking  
- Topic modeling  
- Cross-platform comparison of user perceptions  

---

## 🛠️ Features

- ✔ Scrapes media coverage using **The Guardian API**
- ✔ Collects **Reddit posts & comments** using asynchronous API calls  
- ✔ Extracts **Twitter/X posts** using Tweepy and the free API tier  
- ✔ Downloads **YouTube comments** from selected videos  
- ✔ Filters all content using customizable **neurodivergence keyword lists**  
- ✔ Merges all platforms into a single dataset per movie  
- ✔ Supports advanced NLP analysis (sentiment, LDA topic modeling)

---

If a requirements file is not provided, install dependencies manually based on notebooks:

pandas

requests

tweepy

praw / asyncpraw

youtube_comment_downloader

beautifulsoup4 (if additional scraping)

nltk, gensim, sklearn (optional NLP tasks)

3️⃣ Insert API Keys

You will need keys for:

The Guardian API

Reddit API

Twitter/X API

YouTube (optional)

Store keys in environment variables or local config files (DO NOT commit them).

📑 Workflow
1. Scrape Data

Run Guardian_API_extraction.ipynb for media articles

Run Reddit_API.ipynb for Reddit discussions

Run Twitter_API.ipynb for tweets

Run YT_Reviews.ipynb for YouTube comments

2. Preprocess Data

Use data_preprocessing_code.ipynb to:

Clean all text

Deduplicate

Normalize review formats

3. Merge & Filter

Use final_code.ipynb to:

Merge all platform datasets

Apply neurodivergence keyword filters

Export consolidated CSV/Excel outputs

4. Analyze (Optional)

Sentiment analysis

Keyword frequency analysis

LDA topic modeling (example output in lda_topic_modeling_all.html)

🔑 Customization
Change Movie List

Edit the list/dictionary inside each scraping notebook.

Change Neurodivergence Keywords

Modify the list (e.g., autism, ADHD, dyslexia, stimming, sensory issues, neurodivergent, etc.) in preprocessing or scraping files.

⚠️ Ethical & Legal Notes

Respect the rate limits and Terms of Service of each API.

Do not distribute raw scraped user data without proper anonymization.

Use this repository for academic or research purposes only.

📜 License

This project is intended for research and educational use.
Feel free to fork, modify, or build upon it — with attribution.
