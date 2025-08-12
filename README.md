 Social Profile Scraper

This Python script uses Playwright and BeautifulSoup to scrape profile information (like names, social media links, phone numbers, emails, and websites) from a given URL. It automatically scrolls the page to load more content, extracts relevant profile links, fetches detailed data from each profile, and saves everything into an Excel file.

---

## Features

- Automatic page scrolling to load dynamic content
- Extraction of profile links from the main page
- Parsing individual profiles for social media links (Instagram, LinkedIn), phone numbers, emails, and websites
- Saves extracted data into a timestamped Excel file
- Uses Playwright for browser automation (Chromium)
- Uses BeautifulSoup for HTML parsing

---

## Requirements

- Python 3.7+
- Playwright (`pip install playwright`)
- BeautifulSoup4 (`pip install beautifulsoup4`)
- pandas (`pip install pandas`)

Also, make sure to install the Playwright browsers by running:
playwright install

yaml
Copy
Edit

---

## How to Use

1. Set your target URL in the `main()` function inside the `url` variable.
2. Run the script:
python scraper.py

yaml
Copy
Edit
3. The script will scroll through the page, extract profile data, and save it into an Excel file named like `output_YYYY-MM-DD_HH-MM-SS.xlsx`.

---

## Notes

- The script supports loading cookies from `cookies.json` to handle logged-in sessions if needed.
- Adjust the scroll behavior in the `auto_scroll` function if you want to limit or extend scrolling.
- Make sure the target site structure matches the selectors used in the script, otherwise you might need to update them.

---

## License

This project is open-source and free to use.

---

## Author

Moiz (your name or GitHub handle)
