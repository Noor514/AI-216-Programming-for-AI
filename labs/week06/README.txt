# 📌 Quotes Scraping & SQLite Pipeline Project

## Project Overview

This project demonstrates a complete **data pipeline** using Python. It includes:

* Web scraping quotes from a public website
* Storing data in a SQLite database
* Performing database queries and generating reports
* Practicing ethical scraping using `robots.txt`

---

## Features

* Scrapes quotes and authors from multiple web pages
* Stores structured data in SQLite (`quotes.db`)
* Performs SQL-based analysis
* Generates summary reports
* Follows ethical scraping guidelines

---

## 🛠️ Technologies Used

* Python 3
* Requests
* BeautifulSoup4
* SQLite3

---

## 📂 Project Structure

```
project/
│
├── scrape.py              # Web scraping script
├── database.py            # Database creation
├── insert_data.py         # Store scraped data
├── queries.py             # Database queries
├── pipeline.py            # Full end-to-end pipeline
├── robots_check.py        # Ethical scraping check
├── quotes.db              # SQLite database file
└── README.md              # Project documentation
```

---

## 🔄 Data Pipeline Flow

1. **Scraping**

   * Extract quotes and authors from website

2. **Storage**

   * Save data into SQLite database (`quotes.db`)

3. **Processing**

   * Run SQL queries for insights

4. **Reporting**

   * Display results like total quotes and top authors

---

## 🧾 Database Schema

### Table: `quotes`

| Column | Type    | Description |
| ------ | ------- | ----------- |
| id     | INTEGER | Primary Key |
| quote  | TEXT    | Quote text  |
| author | TEXT    | Author name |

---

## 📊 Sample Outputs

### ✔ Total Quotes Stored

```
30 quotes stored
```

### ✔ Unique Authors

```
10 unique authors
```

### ✔ Top Author

```
Albert Einstein (3 quotes)
```

---

## ⚖️ Ethical Scraping

Before scraping any website, always check `robots.txt`.

Example:

```
https://github.com/robots.txt
```

### 🔍 Example Disallowed Paths

* /search
* /marketplace

👉 These paths should NOT be accessed by bots.

---

## 📌 Key Concepts Learned

* HTTP requests & web scraping
* HTML parsing using BeautifulSoup
* SQLite database operations
* SQL queries (SELECT, INSERT, UPDATE, DELETE)
* Data aggregation and reporting
* Ethical scraping practices

---

##  How to Run

1. Install dependencies:

```bash
pip install requests beautifulsoup4
```

2. Run pipeline:

```bash
python pipeline.py
```

---

##  Author

This project is developed for learning purposes to understand **web scraping, databases, and data pipelines in Python**.
