# 🏉 Six Nations Championship Match Results Scraper

![License: MIT](https://img.shields.io/badge/License-MIT-green.svg)
![Python](https://img.shields.io/badge/Python-3.10-blue.svg)
[![View on Kaggle](https://img.shields.io/badge/View%20Dataset-Kaggle-blue?logo=kaggle)](https://www.kaggle.com/datasets/simfour/rugby-6-nations-results-2000-2024)

This project is a Python-based web scraping tool using **BeautifulSoup** to extract historical match results from the **Six Nations Championship**, the premier international rugby competition in Europe.

## 🧾 Description

This dataset compiles all match results from the beginning of the Six Nations Tournament up to the present. It includes detailed information such as team names, scores, bonus points, and stadiums.

**Participating Teams:** England, France, Ireland, Italy, Scotland, Wales

**📌 Bonus Points Notes:**

Bonus points were introduced in the **2017** edition. For matches before that year, bonus points are recorded as `0`, even though they were not officially awarded.

Bonus points can range from `0` to `5` and are awarded as follows:

- `+1` point for losing by 7 points or fewer  
- `+1` point for scoring 4 or more tries in one match  
- `+3` points for winning all matches in one edition (Grand Slam bonus)  

Bonus points are cumulative per match.

## 📦 Dataset

A cleaned and structured version of the dataset is available on Kaggle:

👉 [https://www.kaggle.com/datasets/simfour/rugby-6-nations-results-2000-2024](https://www.kaggle.com/datasets/simfour/rugby-6-nations-results-2000-2024)

## 🛠️ Technologies Used

- Python 3.10
- `BeautifulSoup4` – for HTML parsing  
- `requests` – for fetching web pages  
- `pandas` – for data handling 

## 📤 Output Format (CSV)

Each row in the dataset corresponds to a match and includes:

| Column        | Type   | Description |
|---------------|--------|-------------|
| `Year`        | int    | Year of the tournament edition |
| `Date`        | date   | Exact match date |
| `HomeTeam`    | str    | Home (host) team |
| `HomeBonus`   | int    | Bonus points earned by the home team |
| `AwayTeam`    | str    | Visiting team |
| `AwayBonus`   | int    | Bonus points earned by the visiting team |
| `HomeScore`   | int    | Points scored by the home team |
| `AwayScore`   | int    | Points scored by the away team |
| `Stadium`     | str    | Name of the stadium where the match was played |

## ▶️ How to Use

Open the notebook, update the cell with start and end year if needed and run the main cell to get the results. 

## 📄 License

This project is licensed under the MIT License.
Use responsibly and in accordance with the terms of service of the websites being scraped.
