## Automated eBay Web Scraping and Price Monitoring Script Documentation

### Overview:
This script enables automated web scraping of eBay product pages to monitor prices. It also provides email notifications if the price of a specific product falls below a defined threshold. The script is written in Python and utilizes various libraries such as BeautifulSoup, requests, pandas, and smtplib.

### Prerequisites:
Before running the script, ensure that the following prerequisites are met:
- Python is installed on your system.
- Required libraries are installed. You can install them using pip: `pip install beautifulsoup4 requests pandas`

### Code Description:

1. **Importing Libraries**:
   - The script begins by importing necessary libraries such as BeautifulSoup, requests, pandas, csv, and smtplib for web scraping, data manipulation, CSV operations, and email functionality.

2. **Connect to eBay Website**:
   - The script specifies the URL of the eBay product page and sends a request to fetch the page content using the requests library.

3. **Parse HTML Content**:
   - BeautifulSoup is used to parse the HTML content of the eBay product page, making it easier to navigate and extract desired information.

4. **Extract Product Title and Price**:
   - The script extracts the title and price of the product from the parsed HTML content of the eBay page.

5. **Clean Data**:
   - The extracted title and price are cleaned by removing unnecessary characters and whitespace.

6. **Write Data to CSV File**:
   - The cleaned data along with the current date are written to a CSV file named "EbayWebScraping.csv" for further analysis and monitoring.

7. **Read Data from CSV**:
   - The script reads the data from the CSV file to verify that the information is stored correctly.

8. **Send Email Notification**:
   - An email notification is sent if the price of the product falls below a certain threshold. Email configuration details are fetched from environment variables using the dotenv library.

9. **Monitor Price Function**:
   - A function named `monitor_price` is defined to automate the process of monitoring the product price. It performs web scraping to extract the latest price and updates the CSV file accordingly. If the price is below a specified threshold, it triggers an email notification.

10. **Automate Price Monitoring**:
    - The `monitor_price` function is executed in a loop with a delay of 24 hours (86400 seconds) between each iteration to continuously monitor the price changes.

### Usage:
1. **Setup Environment Variables**:
   - Set up environment variables for sender email, receiver email, and sender password to enable email notifications. These variables can be stored in a `.env` file in the script directory.

2. **Run the Script**:
   - Execute the script using Python: `python ebay_price_monitor.py`
   - The script will continuously monitor the price of the specified eBay product and send email notifications if the price drops below the defined threshold.

3. **Modify Threshold**:
   - Modify the price threshold in the `monitor_price` function according to your preferences.

### Conclusion:
This script provides a robust solution for automating eBay price monitoring and receiving email notifications for price changes. It can be further customized and integrated into other applications as needed.
