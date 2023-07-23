# Company-Details-Web-Scraping-with-Scrapy and Saving Data to CSV and Excel
---
Overview
---
This Python script demonstrates web scraping using Scrapy, a popular web scraping framework, to extract data from a website containing information about companies. The scraped data is then saved to a CSV file and converted to an Excel file for further analysis and use.

# Prerequisites
Before running the script, ensure you have the following installed:

Python (version 3.6 or higher)
Scrapy (install using ```pip install scrapy```)
Pandas (install using ```pip install pandas```)

# Usage
Clone the repository or download the Python script file (Company Details -checkpoint.ipynb) to your local machine.

Install the required Python libraries using the commands mentioned in the "Prerequisites" section.

Open a terminal or command prompt and navigate to the directory where the Company Details -checkpoint.ipynb file is located.

Run the script using the following command:

Copy code
python ```Company Details -checkpoint.ipynb```

The script will initiate the web scraping process using Scrapy. It will extract company information from this [website](https://vdiv-bw.de/verwaltersuche/?no_cache=1&tx_browser_pi1%5Bradius%5D=50&page=1).

The scraped data will be saved to a CSV file named companies_output.csv, located in the same directory as the script.

Once the scraping process is completed, the script will convert the CSV data to an Excel file named companies_output.xlsx and save it to the specified output path (C:\Users\USER\Desktop\Data Extraction\Succesful Scraping\companies_output.xlsx).

# Customization

If you wish to scrape data from a different website, modify the start_url and allowed_domains variables in the CompanySpider class to target your desired website.

To adjust the time delay between requests, you can modify the DOWNLOAD_DELAY value in the settings dictionary. The current value is set to 3 seconds.

If you want to save the CSV or Excel file to a different directory or under a different name, you can change the corresponding file paths in the script.

# Notes
The website structure or layout might change over time, which can break the scraping process. In such cases, you may need to update the XPath selectors used in the CompanySpider class accordingly.

This script is intended for educational and demonstration purposes. Use it responsibly and avoid causing unnecessary load on the website servers by introducing additional delays between requests if needed.

License
This script is provided under the MIT License.
