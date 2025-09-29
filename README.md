# Video Ranking & Recommendation System

## **Overview**

This project implements a video ranking and content-based recommendation system using a real-world **YouTube trending videos dataset**. The system ranks videos based on engagement metrics and recommends similar videos using textual metadata (title, description, tags).

---

## **Features**

* **Video Ranking:** Videos are ranked using a weighted score combining normalized views, likes, and comments.
* **Visualization:** Top videos are visualized using a bar chart.
* **Content-Based Recommendations:** TF-IDF vectorization on video metadata is used to compute cosine similarity and recommend similar videos.
* **Automatic Dataset Loading:** The dataset is fetched directly from a public GitHub repository, requiring no manual download.

---

## **Dataset**

* Source: [YouTube Trending Videos (US)](https://github.com/ZhaoyiW/YouTube-Trending-Video-Analysis)
* File used: `USvideos.csv`

---

## **Installation**

1. Clone or download this repository.
2. Open the `.ipynb` notebook in **Google Colab** or **Jupyter Notebook**.
3. All required Python libraries: `pandas`, `numpy`, `scikit-learn`, `matplotlib`, `seaborn` (install via `pip` if needed).

```bash
pip install pandas numpy scikit-learn matplotlib seaborn
```

---

## **Usage**

1. Run the notebook cells sequentially.

2. The notebook will:

   * Load the dataset automatically.
   * Compute and display top-ranked videos.
   * Visualize the top 10 videos by ranking score.
   * Recommend top 5 similar videos for a selected video.

3. Modify `top_video_id` to test recommendations for other videos.

---

## **Methodology**

1. Normalize video engagement metrics (views, likes, comments).
2. Compute a weighted ranking score: `Ranking = 0.5*views + 0.3*likes + 0.2*comments`.
3. Use TF-IDF on video title, description, and tags to create feature vectors.
4. Compute cosine similarity between videos for recommendations.

---

## **Conclusion**

This project demonstrates how to:

* Rank videos based on engagement metrics.
* Recommend similar videos using content-based filtering.
* Provide a simple and interactive way for users to explore trending and related content efficiently.

---
