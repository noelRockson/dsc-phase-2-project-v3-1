# 🎬 Film Industry Data Analysis  
![Film Banner](https://upload.wikimedia.org/wikipedia/commons/thumb/1/15/Clap_cinema_icon.png/640px-Clap_cinema_icon.png)

# Project Title  
**Data-Driven Strategy for a New Film Studio**

## 🧭 Overview  
This project analyzes film data to help a new studio make informed decisions about what types of films to produce. Using data from IMDb, TMDb, and box office sources, we identify the genres, runtimes, and formats that receive the highest audience ratings and engagement.

## 💼 Business Understanding  
A new film studio with no production history wants to invest in movies that are likely to succeed with both critics and audiences.

This project aims to:
- Recommend the most popular and well-rated genres  
- Determine the ideal film length based on success metrics  
- Highlight language and format choices for global appeal

## 📊 Data Understanding  
This analysis uses merged data from multiple industry-standard sources:

- **IMDb**: User ratings, votes, runtime, genre, language  
- **TMDb**: Popularity score and metadata  
- **Box Office Mojo & The Numbers**: Budget and revenue insights  

Key variables include:
- `primary_title`, `genres`, `runtime_minutes`  
- `averageRating`, `numVotes`, `language`, `popularity`  

Time Range: Mostly 2000s–2020s  
Total Films Analyzed: Thousands

## 🛠️ Data Preparation  
The data was cleaned and processed as follows:
- Filtered for films with **above-average ratings**
- Dropped rows with missing runtime or genre information  
- Split multi-genre films into individual genres  
- Created visualizations grouped by rating, runtime, and genre  
- Converted and standardized runtime, language, and genre fields

## 📈 Analysis and Results

### 🔹 Top Genres by Popularity  
![Top Genres](Images/output.png)

### 🔹 Runtime Distribution of High-Rated Films  
![Runtime Histogram](Images/output2.png)

## ✅ Final Recommendations

### 🎭 1. **Invest in High-Performing Genres**
- Focus on **Drama**, **Comedy**, **Action**, and **Documentary**  
- These genres have the most consistent high ratings and vote counts

### ⏱ 2. **Target the Ideal Runtime**
- Aim for films between **90–120 minutes**  
- This range dominates among high-rated and high-vote films

### 🌐 3. **Maximize Global Appeal**
- English and Hindi films lead in popularity  
- Consider themes that resonate internationally

### 🧪 4. **Experiment with Genre Hybrids**
- Action-Comedy and Drama-Thriller mixes show strong engagement  
- Can expand audience while managing risk

## ✅ Conclusion and Next Steps  
This analysis equips the studio with insights to make strategic production choices.

**Next Steps:**
- Analyze financial ROI by genre and runtime  
- Run deeper analysis using cast, director, and release year  
- Build an internal dashboard to update and monitor trends

## 📁 Repository Structure

```
├── Images/
│   ├── movie_data_erd.jpeg
│   ├── output.png
│   ├── output2.png
├── zippedData
|   ├── bom.movie_gross.csv
│   ├── im.db.zip
│   ├── tmdb.movies.csv
│   └── tn.movie_budgets.csv
├── .gitignore
├── CONTRIBUTING.md
├── index.ipynb
├── presentation.pdf
├── README.md
├── student.ipynb
└── ...
```