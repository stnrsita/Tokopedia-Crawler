# Tokopedia Crawler

## Overview

Welcome to the **Tokopedia Crawler**! This project contains two scripts to extract product links from Tokopedia for the keyword "flat shoes" using different methods: **Selenium** and **Requests**.

### Key Features

- **Selenium Scraper**: Utilizes a web browser to scroll through the pages and extract more product links. This method allows for comprehensive data collection as it loads all items on the page dynamically.
- **Requests Scraper**: Makes HTTP requests to retrieve only the visible items on the screen, resulting in a limited number of product links.

## Installation

### Prerequisites

Ensure you have the following installed on your machine:

- Python 3.x
- Pip (Python package installer)
- Chrome WebDriver (for Selenium)

### Setup

1. Clone this repository:
   ```bash
   git clone https://github.com/yourusername/tokopedia-crawler.git
   cd tokopedia-crawler
   ```

2. Install the required packages:
   ```bash
   pip install requests beautifulsoup4 selenium pandas
   ```

3. Ensure the `chromedriver` executable is in your project directory and matches your Google Chrome version.

## Usage

### Running the Crawlers

To run the crawlers, use the following commands in your terminal:

1. **Using Selenium:**
   ```bash
   python selenium_crawler.py
   ```

2. **Using Requests:**
   ```bash
   python requests_crawler.py
   ```

After executing each script, the product links will be saved in CSV files named:
- `result_crawling_tokped_with_selenium.csv`
- `result_crawling_tokped_with_requests.csv`

### Data Comparison

The data obtained from the **Selenium** scraper is generally more extensive because it employs scrolling to load all products on the page, so it requires a relatively long execution time. In contrast, the **Requests** method captures only those products that are visible at the time of the request, leading to fewer results but relatively fast execution time..

## Results

The structure of the results generated by both scrapers is as follows:

| Product Links                                |
|----------------------------------------------|
| https://www.tokopedia.com/product1          |
| https://www.tokopedia.com/product2          |
| https://www.tokopedia.com/product3          |
| ...                                          |

> Note: The above table is a sample representation of the links you can expect in the CSV files.

## Conclusion

This project demonstrates the effectiveness of web scraping for data collection from e-commerce sites like Tokopedia. By utilizing both Selenium and Requests, you can gather comprehensive data tailored to your needs.

---

Happy Crawling!
