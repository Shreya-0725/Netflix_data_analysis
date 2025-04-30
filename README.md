# 📊 Netflix Movie Data Analysis 

## 📌 Project Overview

This project analyzes Netflix's movie catalog to uncover trends in genres, popularity, ratings, and release timelines. The objective was to generate actionable insights that can guide Netflix or similar streaming platforms in content planning, acquisition, and audience targeting strategies.

---

## 🎯 Goal of the Dashboard

The goal of this dashboard is to provide strategic insights into Netflix's movie content by analyzing patterns in:

- **Movie Genres**: Understanding which genres dominate Netflix’s library to guide future investments.
- **Audience Preferences**: Identifying highest and lowest-rated movies and most voted content to analyze viewer sentiment.
- **Popularity Trends**: Examining which movies gained the most/least attention and their associated genres.
- **Release Timeline**: Discovering which years saw the most movie releases to understand content volume strategies.

These insights help stakeholders make informed decisions around production, content curation, and platform optimization.

---

## 🧩 Business Problem

Netflix constantly invests in diverse content, but understanding **what performs well** (by genre, rating, and popularity) is critical for maximizing viewer engagement and retention. The challenge is to find which types of content resonate the most with audiences — and when.

---

## 🧪 Dataset Overview

- **Source**: Internal Netflix data (simulated for this project)
- **Rows**: 9,827
- **Columns**: 9
- **Key Columns**: `Title`, `Release_Date`, `Genre`, `Vote_Average`, `Popularity`, `Vote_Count`

---

## 🛠️ Data Cleaning Steps

- Converted `Release_Date` to datetime and extracted **release year**.
- Cleaned the `Genre` column (split comma-separated values and exploded them into individual rows).
- Categorized `Vote_Average` into bins: `not_popular`, `below_avg`, `average`, `popular`.
- Dropped unnecessary columns like `Overview` and `Original_Language` for analysis clarity.

---

## 📊 Key Visuals & Interview-Worthy Insights

### 1. Genre Distribution

- **Visualization**: Count plot of `Genre`
- **Insight**: Drama is the most frequent genre on Netflix, indicating a strong platform preference for emotional, narrative-driven content.

---

### 2. Highest Voted Genre Distribution

- **Visualization**: Count plot of `Vote_Average` bins
- **Insight**: Most movies fall under the `average` to `below_avg` rating categories, signaling room for improvement in overall content quality.

---

### 3. Most Popular Movie & Its Genre

- **Movie**: *Spider-Man: No Way Home*
- **Genres**: Action, Adventure, Science Fiction
- **Insight**: High popularity correlates with high-action, franchise-driven content. Netflix could benefit by acquiring or producing similar blockbuster-style content.

---

### 4. Least Popular Movie & Its Genre

- **Movie**: *The United States, Thread*
- **Genres**: Music, Drama, War, Sci-Fi, History
- **Insight**: Niche or complex genre blends tend to be less popular, suggesting Netflix should re-evaluate investment in such content.

---

### 5. Movie Releases by Year

- **Visualization**: Histogram of `Release_Date`
- **Insight**: A spike in movie releases occurred in recent years, indicating aggressive content expansion — which may align with user acquisition or retention strategies.

---

## ✅ Conclusion

This dashboard provides a clear view into Netflix’s movie catalog strategy:

- **Drama** is the most dominant genre.
- **Audience ratings** mostly fall between average to below average — an area to improve.
- **Blockbusters** like Spider-Man have the highest popularity, suggesting that action-packed or franchise movies drive high engagement.
- **Release year trends** show a significant push in recent years, highlighting Netflix's strategy to expand its movie library rapidly.

These insights can assist Netflix in making data-driven decisions about **what content to promote, produce, or retire** from its platform.

---

## 🧰 Tools Used

- **Python** (Pandas, NumPy)
- **Visualization**: Matplotlib, Seaborn
- **Jupyter Notebook** for development
