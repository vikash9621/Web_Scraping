# Project Description

-> This project is a Python-based web scraper that extracts laptop listings from Amazon India.
->It uses Selenium to interact with dynamic content and BeautifulSoup to parse product details. 
  
  The extracted data includes:

- Laptop Name
- Price (in ₹)
- User Review (rating)
- Scraping Date

The data is saved into a CSV file, making it ideal for price trend analysis, dashboards (e.g., Power BI), and market comparison.

## Tools and Libraries Used

| Tool/Library        | Purpose                                                               |
| ------------------- | --------------------------------------------------------------------- |
|   selenium          | Automates browser to load dynamic content (JavaScript-rendered pages) |
|   webdriver-manager | Automatically installs the right ChromeDriver                         |
|   beautifulsoup4    | Parses HTML and extracts content using tags                           |
|   pandas            | Stores, cleans, and writes tabular data                               |
|   datetime          | Captures the date when scraping takes place                           |
|   time              | Adds delay to let JS content render                                   |


📋 Step-by-Step Process

1. Setup Headless Chrome
-> Launches a Chrome browser in headless mode using Selenium.

-> Simulates user visiting each Amazon page .

2. Scrape Product Data

For each page:

->Fetch product name

->Fetch price (if available)

->Fetch rating (e.g., "4.3 out of 5 stars")

->Save the current date

3. Save Raw Data
->All data is stored into a Pandas DataFrame.

->Output CSV: amazon_data61.csv

4. Data Cleaning Process
->Loads scraped CSV (amazon_laptop_data.csv)

->Extracts numeric rating using regex from review text

->Saves cleaned output to: cleaned_amazon_laptops.csv


🔮 Future Enhancements
->Add Flipkart support

->Schedule auto-scraping (daily)

->Email alerts for price drops

->Power BI / Tableau dashboard integration

->Add product URL and image





