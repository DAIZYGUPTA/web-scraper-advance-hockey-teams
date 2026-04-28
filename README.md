
# Web Scraping Pipeline — Query-Based Data Extraction and Processing

## Overview
This project demonstrates a structured web scraping pipeline that extracts data from a paginated website, supports query-based filtering, and converts raw HTML into a clean, analysis-ready dataset.

The focus is on building a reusable and modular data pipeline rather than a one-time script.

## Features
- Pagination handling without hardcoding
- Query-based scraping using URL parameters
- Modular code structure (separate parsing and fetching logic)
- Safe data extraction (handling missing values)
- Raw HTML storage for reproducibility
- Structured dataset generation using Pandas
- Output in both CSV and Parquet formats

## Tech Stack
- Python
- requests
- BeautifulSoup (bs4)
- pandas

## Pipeline Architecture

### 1. Data Fetching
- Sends HTTP requests with headers
- Supports optional query filtering
- Detects total pages dynamically

### 2. Data Parsing
- Extracts structured data from HTML using CSS selectors
- Converts values into appropriate data types
- Handles missing values safely

### 3. Data Storage
- Saves raw HTML files locally
- Builds a structured dataset using Pandas

### 4. Output Generation
- Exports dataset as CSV (for compatibility)
- Exports dataset as Parquet (for efficiency and performance)

## Dataset
- Records: 500+
- Features:
  - Name
  - Year
  - Wins
  - Losses
  - Win %
  - Goals For
  - Goals Against
  - Goal Difference (+/-)

## Example Usage

```python
df = fetch_and_parse()
df = fetch_and_parse("Boston")
```

## Key Learning Outcomes
- Handling pagination dynamically
- Designing modular and reusable code
- Building a complete data pipeline (fetch → parse → store)
- Understanding the importance of structured data over raw scraping
- Working with efficient data storage formats like Parquet

## Output Files
- Raw HTML files for each page
- Clean dataset in CSV format
- Optimized dataset in Parquet format

## Future Improvements
- Add automated data pipeline execution
- Perform exploratory data analysis (EDA)
- Apply machine learning models on the dataset
- Build an interactive dashboard using Streamlit

## Contributing
Suggestions and improvements are welcome.

## Contact
Open to opportunities in data science, machine learning, and data engineering.
