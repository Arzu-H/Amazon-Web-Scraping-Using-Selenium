# Amazon Product Web Scraper

A Python-based web scraping tool that extracts product information from Amazon's search results using Selenium WebDriver.

## Features

- Scrapes product details including titles, prices, and product links
- Headless browser operation for faster execution
- Data export to CSV format
- Built-in wait times and error handling for reliable scraping
- Configurable search terms and result limits

## Prerequisites

- Python 3.x
- Chrome browser
- ChromeDriver (compatible with your Chrome version)

## Required Libraries

```bash
pip install selenium
pip install pandas
```

## Setup

1. Install the required Python packages
2. Ensure Chrome browser is installed on your system
3. Download the appropriate ChromeDriver version for your Chrome browser
4. Place the ChromeDriver in your system PATH or specify its location in the code

## Usage

1. The script will:
   - Launch a headless Chrome browser
   - Navigate to Amazon.com
   - Search for the specified product (default: "laptop")
   - Extract details of the first 20 products
   - Save results to a CSV file

2. To modify the search term, update the `search_term` variable:
   ```python
   search_term = "your_search_term"
   ```

## Output

The script generates a CSV file named `amazon-web-scraping.csv` with the following columns:
- Title: Product name
- Price: Product price
- Link: Product URL

## Error Handling

- The script includes try-except blocks to handle common scraping issues
- Missing data fields are marked as "N/A"
- WebDriverWait is implemented to handle dynamic loading elements

## Limitations

- Results are limited to the first 20 products
- Scraping may be affected by Amazon's layout changes
- Rate limiting and captchas may affect functionality
- Price extraction assumes standard Amazon price format

## Legal Notice

Web scraping may be subject to legal restrictions and website terms of service. This tool is for educational purposes only.

## Best Practices

1. Implement appropriate delays between requests
2. Use the headless browser option for better performance
3. Regularly update ChromeDriver to match your Chrome version
4. Monitor for changes in Amazon's website structure
5. Handle your data collection responsibly


