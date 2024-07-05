# Analysing Bias in 2024 UK Election News Articles

## Table of Contents

- [Project Overview](#project-overview)
- [Features](#features)
- [Installation](#installation)
- [Usage](#usage)
- [Data Collection](#data-collection)
- [Data Cleaning and Preparation](#data-cleaning-and-preparation)
- [Topic Handling Process](#topic-handling-process)
- [Sentiment Analysis](#sentiment-analysis)
- [Visualisation](#visualisation)
- [Contributing](#contributing)
- [License](#license)
- [Contact](#contact)

## Project Overview

This project focuses on detecting and visualising potential bias in news articles related to the 2024 UK election. By employing data scraping, cleaning, sentiment analysis, and visualization techniques, we aim to develop a comprehensive dataset and analysis that highlight bias trends across various news sources.

## Features

- **Data Scraping:** Extracts news articles from various sources.
- **Data Cleaning:** Processes and cleans text data for analysis.
- **Topic Modeling:** Identifies key topics in the news articles.
- **Sentiment Analysis:** Evaluates the sentiment of the articles.
- **Data Visualization:** Prepares data for visualization in Tableau.
- **Bias Detection:** Highlights potential biases in news coverage.

## Installation

To run this project locally, follow these steps:

1. **Clone the Repository:**
    ```bash
    git clone https://github.com/yourusername/uk-election-bias-analysis.git
    cd uk-election-bias-analysis
    ```

2. **Create a Virtual Environment:**
    ```bash
    python -m venv venv
    source venv/bin/activate  # On Windows use `venv\Scripts\activate`
    ```

3. **Install Dependencies:**
    ```bash
    pip install -r requirements.txt
    ```

4. **Download Required Data:**
    Ensure you have the necessary data files or run the data scraping script to collect data.

## Usage

### Running Jupyter Notebooks

To explore the data processing steps and analysis, open and run the Jupyter notebooks:

1. **Start Jupyter Notebook:**
    ```bash
    jupyter notebook
    ```

2. **Open the Notebooks:**
    - `capstone_get_data.ipynb` - Data scraping and cleaning.
    - `capstone_sentiment_analysis.ipynb` - Sentiment analysis.
    - `capstone_table_check.ipynb` - Data preparation for visualization.

### Scripts

- **Data Scraping:** 
    ```bash
    python scripts/data_scraping.py
    ```
- **Data Cleaning:** 
    ```bash
    python scripts/data_cleaning.py
    ```
- **Sentiment Analysis:**
    ```bash
    python scripts/sentiment_analysis.py
    ```

## Data Collection

A combination of web scraping techniques was used to collect news articles from various sources. The key steps include:

- **Scrape Links:** Extract news article links from specified websites.
- **Scrape Article Data:** Gather article content, titles, authors, and publication dates.

## Data Cleaning and Preparation

Data cleaning process involves:

- **Text Cleaning:** Removing URLs, email addresses, and other unwanted elements.
- **Tokenization:** Splitting text into individual words and removing stopwords.
- **Date Formatting:** Converting publication dates into a standard format.

## Topic Handling Process

Identify and manage topics using the following steps:

1. **Topic Modeling:** Utilize LDA to uncover topics in articles.
2. **Topic Extraction:** Extract key topics and words.
3. **Topic Classification:** Classify articles based on predominant topics.
4. **Topic Frequency Analysis:** Analyse the frequency of each topic.

## Sentiment Analysis

Sentiment analysis workflow includes:

- **Methods:** Using rule-based and machine learning-based approaches (e.g., VADER, TextBlob, BERT).
- **Sentiment Labeling:** Assigning positive, negative, or neutral labels to articles.
- **Quality Checks:** Ensuring accuracy through random checks and validations.

## Visualisation

Data prepared for visualization is saved in CSV files and imported into Tableau for detailed bias analysis. Visualisations include topic frequencies, sentiment distribution, and source bias.

The visualisation can be seen through Tableau Public here : [Bias Presentation](https://public.tableau.com/shared/H2XQ2YXFM?:display_count=n&:origin=viz_share_link)

## Contributing

We welcome contributions to improve this project! Here’s how you can help:

1. Fork the repository.
2. Create a new branch (`git checkout -b feature/YourFeature`).
3. Commit your changes (`git commit -m 'Add YourFeature'`).
4. Push to the branch (`git push origin feature/YourFeature`).
5. Open a Pull Request.

---

Feel free to contribute and improve this project. Together, we can create a valuable resource for analyzing bias in news articles!

