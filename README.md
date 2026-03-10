# 🎧 Spotify Artist & Track Analysis

## 📌 Project Overview

This project performs an **Exploratory Data Analysis (EDA)** on Spotify datasets containing information about artists and tracks.

The goal of this analysis is to understand patterns in music data such as:

- Artist popularity
- Track popularity
- Audio features of songs
- Release trends
- Duration patterns
- Relationships between music characteristics

The analysis helps uncover insights about how different music features influence song popularity on Spotify.

---

## 📂 Dataset Information

The project uses two datasets:

### 1️⃣ Artists Dataset
Contains information about Spotify artists.

Main columns include:

- `id` – Unique artist identifier  
- `name` – Artist name  
- `followers` – Number of followers  
- `popularity` – Popularity score of the artist  
- `genres` – Music genres associated with the artist  

---

### 2️⃣ Tracks Dataset
Contains detailed information about songs.

Main columns include:

- `id` – Unique track identifier  
- `name` – Track name  
- `popularity` – Popularity score of the track  
- `duration_ms` – Track duration in milliseconds  
- `release_date` – Song release date  
- `danceability` – How suitable the track is for dancing  
- `energy` – Intensity and activity of the track  
- `loudness` – Overall loudness of the track  
- `valence` – Positivity of the track  
- `tempo` – Speed of the song  
- `acousticness` – Probability that the track is acoustic  

---

## ⚙️ Data Processing Steps

The following steps were performed in the analysis:

1. **Data Loading**

   Both datasets were loaded using Pandas.

2. **Column Renaming**

   To avoid column conflicts during merging:
   
   - `id` in artists → renamed to **artist_id**
   - `id` in tracks → renamed to **track_id**

3. **Data Cleaning**

   - Removed duplicate records
   - Handled missing values
   - Converted track duration from milliseconds to minutes

4. **Artist Column Processing**

   The `id_artists` column contained multiple artist IDs in list format.

   This column was cleaned and exploded so that each row represents a single artist.

5. **Dataset Merging**

   The datasets were merged using the **artist_id** column to create a combined dataset for deeper analysis.

---

## 📊 Analysis Performed

### 1️⃣ Artist Analysis

- Top artists with the most tracks
- Artists with the highest popularity
- Distribution of artist popularity

---

### 2️⃣ Track Analysis

- Top 10 most popular tracks
- Distribution of track popularity
- Average track popularity

---

### 3️⃣ Audio Feature Analysis

The following music features were analyzed:

- Danceability
- Energy
- Loudness
- Valence
- Tempo
- Acousticness

Scatter plots were used to explore relationships between these features and track popularity.

---

### 4️⃣ Track Duration Analysis

- Distribution of song durations
- Average length of tracks

Duration was converted from milliseconds to minutes for better interpretation.

---

### 5️⃣ Release Trend Analysis

- Number of tracks released per year
- Popularity trends over time

This analysis helps understand how music production changes over time.

---

### 6️⃣ Correlation Analysis

A **correlation heatmap** was created to understand relationships between numerical variables such as:

- Energy
- Loudness
- Danceability
- Tempo
- Popularity

---

## 📈 Key Insights

Some important insights from the analysis include:

- A small number of artists contribute a large number of tracks.
- Track popularity varies widely across songs.
- High energy tracks often have higher loudness values.
- Most songs fall within a similar duration range.
- Audio features like danceability and energy influence listener engagement.

---

## 🛠 Tools & Technologies Used

- **Python**
- **Pandas**
- **Matplotlib**
- **Seaborn**
- **Jupyter Notebook / Google Colab**

---

## 📁 Project Structure
Spotify-Analysis  
│  
├── Spotify_Analysis.ipynb  
├── artists.csv  
├── tracks.csv  
└── README.md  


---

## 🎯 Project Objective

The objective of this project is to demonstrate **data cleaning, dataset merging, exploratory data analysis, and data visualization skills** using real-world Spotify data.

This project helps understand how data analysis can uncover meaningful insights from music streaming platforms.

---

## 🚀 Future Improvements

Possible improvements for this project include:

- Building a **machine learning model to predict track popularity**
- Creating an **interactive dashboard using Power BI or Tableau**
- Performing deeper **genre-based analysis**

---

## 📬 Author

**Aman K**

Data Analyst | Data Visualization | Python | SQL
