# 📺 YouTube Trending Video Analysis  

A full-stack data analytics project by **Prajwal Shelar**, designed to uncover hidden patterns behind YouTube’s global trending videos.  
This project explores **100,000+ videos** to analyze audience engagement, channel behavior, and content performance — empowering creators, analysts, and strategists with predictive insights and interactive dashboards for smarter publishing decisions.  

---

---

## 🧠 Project Overview  

Understanding what makes a video trend is crucial for maximizing reach and engagement.  
This project delivers a complete analytics workflow — from data cleaning to model deployment — enabling:  

- 📊 Performance forecasting using video metadata  
- 👍 Engagement-driven content strategy optimization  
- 🌍 Country-wise trend comparison and analysis  
- 📈 Dashboard insights for creators and media planners  

---

## 🎯 Key Objectives  

- Clean and preprocess multi-country YouTube datasets  
- Engineer features for view prediction and dashboard visualization  
- Build and evaluate regression models for performance forecasting  
- Deploy an interactive Streamlit dashboard for real-time insights  

---

## 📁 Project Structure  

| File Name | Description |
|------------|--------------|
| `youtube.csv` | Raw dataset of trending video records |
| `cleaned_youtube.csv` | Processed data after cleaning and feature engineering |
| `youtube.sql` | SQL queries for extraction and filtering |
| `sqlconnect.py` | Python script for SQL database connection |
| `youtube analysis.ipynb` | Jupyter notebook with EDA, ML modeling, and insights |
| `trending_model.pkl` | Trained regression model for predicting video views |
| `trending_features.pkl` | Saved feature set used during training |
| `channel_encoder.pkl` | Encoder for channel names |
| `country_encoder.pkl` | Encoder for country names |
| `app.py` | Streamlit app for dashboard deployment |
| `YOUTUBE ANALYSIS DASHBOARD.accdb` | MS Access dashboard for engagement and performance trends |

---

## 🧹 Data Preprocessing  

- Encoded categorical features (`channel_title`, `country`, `category_id`)  
- Extracted publish-time features (`hour`, `day`, `month`)  
- Engineered engagement metrics (`likes`, `dislikes`, `comment_count`)  
- Removed duplicates and handled missing values  
- Normalized continuous variables for consistent model training  

---

## 📈 Exploratory Data Analysis  

- View distribution across countries and categories  
- Engagement metrics variation over time  
- Channel behavior and consistency in uploads  
- Correlation matrix of engagement features vs. views  
- Time-of-day impact on video performance  

---

## 🤖 Modeling Approach  

- **Target Variable:** `views`  
- **Algorithms:** Linear Regression, Random Forest Regressor, XGBoost Regressor  
- **Evaluation Metrics:** MAE, RMSE, R² Score  
- **Key Features:** `likes`, `comment_count`, `publish_hour`, `channel_title`, `country`  

---

## 📊 Dashboard Overview  

### 🔷 MS Access Dashboard  
Provides visual insights into engagement and performance trends:  

- 🌍 View distribution by country and category  
- 📈 Growth of engagement metrics over time  
- 📊 KPIs: Average views, likes, and comments  

![Power BI Preview](https://image2url.com/images/1755870126425-f0cdee17-78bc-4837-b2a0-01f85a494821.png)  
![Power BI Preview](https://image2url.com/images/1755870155361-9d759e81-1d66-473b-958e-f7ecafdb3da6.png)  

---

### 🟢 Streamlit App  
An interactive dashboard for real-time predictions and insights:  

- 📺 Input video metadata to forecast views  
- 📊 Visualize feature importance  
- 🌍 Filter by country or category  
- 📈 Compare engagement-driven predictions  

![Streamlit Preview](https://image2url.com/images/1755870229701-78175c47-feb6-4b48-9619-b2411a14f029.png)  

---

## 🚀 Deployment  

- Model serialized using **Pickle (`.pkl`)** for persistence  
- Deployed on **Streamlit Cloud** for live demo  
- SQL integration for dynamic video filtering  
- Git LFS used for managing large files  

---

## 🧠 Business Impact  

- Forecasts future video performance for better planning  
- Identifies high-engagement formats and regions  
- Helps optimize publishing schedules by country and category  
- Supports content creators with data-driven strategy  

---

## 🛠️ Tech Stack  

- **Languages & Libraries:** Python (Pandas, NumPy, Scikit-learn, Streamlit)  
- **Database:** SQL for filtering and extraction  
- **Visualization Tools:** MS Access, Matplotlib, Seaborn, Plotly  
- **Deployment:** Streamlit Cloud, GitHub, Git LFS  

---

## 📌 Future Enhancements  

- Add **NLP analysis** on video titles and descriptions for sentiment detection  
- Introduce **clustering** to group channels by performance behavior  
- Allow **user uploads** for instant view prediction  
- Expand dashboard for **subscriber growth forecasting**  
