 Social Profile Scraper

This Python script automates extracting profile information—such as names, social media links (Instagram, LinkedIn), phone numbers, emails, and websites—from a target webpage. It uses Playwright to load the page with automatic scrolling, dynamically loads all content, extracts profile links, visits each profile for detailed data, and saves everything into a timestamped Excel file.

**Key features:**
- Automatic scrolling to load all dynamic content
- Extracts profile URLs and detailed info from each profile
- Gathers social links, contact info, and websites
- Saves results in Excel format for easy analysis

**Requirements:**
- Python 3.7+
- Playwright (`pip install playwright`) & run `playwright install`
- BeautifulSoup4 (`pip install beautifulsoup4`)
- pandas (`pip install pandas`)

**Usage:**
1. Set the target URL inside the `main()` function.
2. Run the script: `python scraper.py`
3. Find the results saved as `output_YYYY-MM-DD_HH-MM-SS.xlsx`.

**Notes:**
- Supports session cookies with `cookies.json` if available.
- Scrolling behavior can be customized in the `auto_scroll` function.
- Update CSS selectors if the page structure changes.

Created by Moiz
