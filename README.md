# Web Scraping Project: Fake Job Listings

## Overview
This project involves writing a Python script to scrape fake job listings from a sample website. We use the `requests` library to fetch webpage content and `BeautifulSoup` from `bs4` to parse and extract job listing information.

## Setup
- Python 3.x
- Libraries: `requests`, `beautifulsoup4`

## Usage
Run the script to scrape job listings from `https://realpython.github.io/fake-jobs/`. The script extracts titles, companies, and locations of the listings and prints them to the console.

## Code Snippet
```python
# Sample code snippet for fetching and parsing content
import requests
from bs4 import BeautifulSoup

URL = "https://realpython.github.io/fake-jobs/"
response = requests.get(URL)
soup = BeautifulSoup(response.content, 'html.parser')

