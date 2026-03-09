# 🏏 IPL Data Analysis (EDA)

## 📌 Project Overview
This project performs **Exploratory Data Analysis (EDA)** on the IPL dataset using Python to explore match data, player performances, team results, and venue statistics.

---

## 🛠️ Libraries Used
- 🐼 **pandas**
- 🔢 **numpy**
- 📊 **matplotlib**
- 🎨 **seaborn**

---

## 📂 Data Loading
- Imported the required Python libraries.
- Loaded the dataset using `pd.read_csv("ipl.csv")`.
- Displayed the first few rows of the dataset using `df.head()`.

---

## 🔍 Dataset Overview
- Used `df.describe()` to check the statistical summary of numerical columns.
- Used `df.info()` to examine:
  - Total number of rows and columns
  - Data types of each column
  - Non-null values present in the dataset.

---

## 🧹 Data Cleaning
- Checked for duplicate rows using `df.duplicated().sum()`.
- Checked missing values using `df.isna().sum()`.
- Dropped the **umpire3** column due to a large number of missing values.

---

## 📊 Exploratory Data Analysis

### 📅 Matches Played Per Season
- Calculated the number of matches played in each season using `value_counts()`.
- Sorted seasons using `sort_index()`.
- Visualized the result using a **line plot**.

---

### 🏅 Top 10 Player of the Match
- Counted `player_of_match` awards using `value_counts()`.
- Selected the **top 10 players** with the most awards.
- Visualized the results using a **bar chart**.

---

### 🏆 Maximum Winning Margins
- Calculated:
  - Maximum value of `win_by_runs`
  - Maximum value of `win_by_wickets`.

---

### 🎲 Toss Winner and Match Winner
- Calculated the number of matches where the **toss winner also won the match**.

---

### 🥇 Top 10 Teams by Wins
- Calculated team wins using `winner.value_counts()`.
- Selected the **top 10 teams** with the highest wins.
- Visualized the distribution using a **pie chart**.

---

### 📉 Teams With Least Wins
- Sorted teams by number of wins in ascending order.
- Selected the **5 teams with the least wins**.
- Visualized the results using a **bar chart**.

---

### 🪙 Toss Decision Analysis
- Counted toss decisions using `toss_decision.value_counts()` to see how many times teams chose:
  - `bat`
  - `field`.

---

### ⚔️ Toss Decision vs Match Result
- Calculated matches where:
  - Toss winner chose **bat** and won the match.
  - Toss winner chose **field** and won the match.

---

### 🔴 RCB Wins at Chinnaswamy Stadium
- Filtered matches where:
  - `winner = Royal Challengers Bangalore`
  - `venue = M Chinnaswamy Stadium`.
- Calculated the total number of wins.

---

### 📊 Distribution of Wins by Runs
- Created a **histogram** showing the distribution of win margins by runs.

---

### 🏟️ Top Venues Hosting IPL Matches
- Calculated venues with the highest number of matches using `value_counts()`.
- Selected the **top 10 venues**.
- Visualized the distribution using a **pie chart**.

---

### 🌆 Cities Hosting IPL Matches
- Calculated cities that hosted the most IPL matches using `value_counts()`.
- Selected the **top 10 cities**.
- Visualized the distribution using a **pie chart**.

---

## 📑 Dataset Columns
- `id`
- `season`
- `city`
- `date`
- `team1`
- `team2`
- `toss_winner`
- `toss_decision`
- `result`
- `dl_applied`
- `winner`
- `win_by_runs`
- `win_by_wickets`
- `player_of_match`
- `venue`
- `umpire1`
- `umpire2`

---

⭐ *Aspiring Data Analyst exploring data using Python, data cleaning, and exploratory data analysis techniques.*
