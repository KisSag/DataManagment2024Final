
# Movie Review Analysis Project

## Project Overview
This project scrapes movie reviews from Rotten Tomatoes and performs sentiment analysis on the collected data. The analysis includes both positive and negative reviews, data preprocessing, and storage in a SQLite database. I use movie reviews and ratings to train and evaluate the model.

## Requirements
Required packages:
- pandas
- numpy
- requests
- pyquery
- sqlite3
- scikit-learn
- beautifulsoup4


## Database
- SQLite3 (included in Python standard library)


## Project Structure
project/
│
├── assign.ipynb # Main Jupyter notebook
├── movie_reviews.db # SQLite database
├── requirements.txt # Project dependencies
└── README.md # This file

## Features
1. **Web Scraping**
   - Scrapes movie reviews from Rotten Tomatoes
   - Collects reviewer name, source, review text, and date
   - Handles both positive and negative reviews

2. **Data Processing**
   - Text preprocessing
   - Sentiment analysis
   - Feature extraction

3. **Data Storage**
   - SQLite database integration
   - Three main tables:
     - positive_reviews
     - negative_reviews
     - final_reviews

## Usage

1. **Setup Environment**
   ```bash
   # Install dependencies
   pip install -r requirements.txt
   ```

2. **Run the Notebook**
   ```bash
   jupyter notebook assign.ipynb
   ```

3. **Database Operations**
   - Data is automatically saved to `movie_reviews.db`
   - To query the database directly:
   ```python
   import sqlite3
   conn = sqlite3.connect('movie_reviews.db')
   # Run your SQL queries
   conn.close()
   ```

## Notes
- Ensure proper internet connection for web scraping
- The database file will be created in the project root directory

