# 📊 Internship Market Intelligence Platform

An end-to-end internship data engineering platform developed as a Master's Challenge Hub project. 

The platform automates the collection of internship announcements from www.indeed.com, cleans and normalizes the data into a centralized cloud database, and exposes them through a searchable, user-friendly web portal.

---

## 🚀 Live Demo & Presentation

* **Web Portal:** [intern.mobilepul.com](https://intern.mobilepul.com) *(Note: If the live site is archived, please refer to the project artifacts below).*
* **Project Artifacts:** The core web-scraping pipelines and Jupyter Notebooks are available in this repository. 

<!-- Un-comment the line below and add your poster filename if you want to display your university poster -->
<!-- ![Project Poster](your-poster-filename.png) -->

---

## 🛠️ Technology Stack

![Python](https://img.shields.io/badge/python-3670A0?style=for-the-badge&logo=python&logoColor=ffdd54)
![Pandas](https://img.shields.io/badge/pandas-%23150458.svg?style=for-the-badge&logo=pandas&logoColor=white)
![MySQL](https://img.shields.io/badge/mysql-%2300f.svg?style=for-the-badge&logo=mysql&logoColor=white)
![PHP](https://img.shields.io/badge/php-%23777BB4.svg?style=for-the-badge&logo=php&logoColor=white)
![Linux](https://img.shields.io/badge/linux-%23FCC624.svg?style=for-the-badge&logo=linux&logoColor=black)
![HTML5](https://img.shields.io/badge/html5-%23E34F26.svg?style=for-the-badge&logo=html5&logoColor=white)
![CSS3](https://img.shields.io/badge/css3-%231572B6.svg?style=for-the-badge&logo=css3&logoColor=white)
![Jupyter Notebook](https://img.shields.io/badge/jupyter-%23FA4F01.svg?style=for-the-badge&logo=jupyter&logoColor=white)

* **Data Extraction:** BeautifulSoup4
* **Automation:** Linux Cron Jobs

---

## 🏗️ System Architecture

```text
  [ Indeed.com ]
        │
        ▼
 [ BeautifulSoup4 ] ──( HTML Parsing )
        │
        ▼
  [ Python/Pandas ] ──( Data Transformation & Deduplication )
        │
        ▼
[ MySQL Cloud DB ]  ──( Data Storage & Querying )
        │
        ▼
 [ PHP Web Portal ] ──( User Interface )
        │
        ▼
    [ Users ]
```

## 🌟 Key Features
Automated Data Collection: Continuous mining of targeted internship postings.

Robust Preprocessing: Automated data cleaning and data type normalization using Pandas.

Duplicate Detection: Smart filtering to ensure unique job postings and prevent database bloat.

Cloud Architecture: Structured storage in a cloud-hosted MySQL database.

Dynamic Search: Full-text search capability by city and specific industry keywords.

Scheduled Pipelines: Fully automated daily updates orchestrated via Linux Cron Jobs.

## 🔄 Project Workflow
Data Collection ➔ HTML Parsing ➔ Cleaning & Transformation ➔ Duplicate Detection ➔ MySQL Storage ➔ PHP Portal ➔ User Search

Extraction: Python scripts request and parse raw HTML content from target job boards.

ETL Pipeline: Data is fed into a Pandas pipeline where missing values are handled, strings are stripped, and duplicates are removed.

Ingestion: Cleaned records are securely pushed into the MySQL cloud database.

Delivery: The PHP frontend queries the database in real-time based on user search parameters (keywords, location) to serve active internship leads.

---
