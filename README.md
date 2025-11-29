# Cryptocurrency-Price-Tracker

Cryptocurrency Price Tracker
Automated Real-Time Market Data Extraction Tool
Overview:

The Cryptocurrency Price Tracker is a robust Python-based tool designed to extract and log real-time cryptocurrency market data from CoinMarketCap. It uses Selenium WebDriver to automate browser interaction, effectively handling dynamic, JavaScript-rendered content to ensure the collection of accurate, live market metrics.
This project is ideal for analysts, investors, and developers seeking consistent, structured data for trend forecasting, dashboard visualization, and custom portfolio monitoring.

Key Features:

 * Live Price Scraping: Dynamically fetches current price, 24-hour change, and market capitalization for leading cryptocurrencies.
 * Dynamic Page Handling: Leverages Selenium to reliably scrape data from modern, JavaScript-heavy web pages.
 * Top 10 Coins Focus: Structured to collect essential metrics for the top 10 cryptocurrencies (easily configurable for more).
 * Historical Logging: Appends timestamped data to a CSV file, enabling powerful trend tracking and comparative analysis over time.
 * CSV Export Ready: Outputs clean, structured data directly into a CSV file, ready for integration with visualization tools.
 * Headless Support: Supports running the script in the background using headless browser mode, perfect for server deployment or scheduled tasks.

Technologies Used:
| Category | Technology | Purpose |
|---|---|---|
| Core Language | Python 3.x | Primary language for automation and logic. |
| Web Scraping | Selenium | Automates browser control and handles dynamic content rendering. |
| Data Processing | Pandas | Structures, manipulates, and exports data to CSV. |
| Driver Management | webdriver_manager | Automatically manages and installs the correct ChromeDriver version. |
| Browser | Google Chrome | Controlled via ChromeDriver for scraping. |

Getting Started:

Prerequisites
 * Python 3.x installed.
 * Google Chrome installed (for Selenium to control).
Installation
 * Clone the repository:
   git clone https://github.com/your-username/crypto-price-tracker.git
cd crypto-price-tracker

 * Install the required Python libraries:
   pip install selenium pandas webdriver-manager

Running the Script:

 * Open your terminal or command prompt.
 * Execute the main Python script:
   python tracker.py

 * The script will initialize the Chrome browser (or run in headless mode if configured), scrape the data, and generate/update the output file.

Output:

The script generates a file named crypto_prices.csv. Each row is timestamped and includes the following columns:
| Column Name | Description |
|---|---|
| Timestamp | The date and time the data was collected. |
| Coin Name | The full name of the cryptocurrency (e.g., Bitcoin). |
| Price | The current price in USD. |
| 24h Change (%) | The percentage change in the last 24 hours. |
| Market Cap | The current total market capitalization. |

Future Enhancements:

 * Multi-Platform Aggregation: Add support for scraping prices from multiple exchanges (e.g., Binance, Coinbase).
 * Database Integration: Replace CSV export with integration into a relational (e.g., PostgreSQL) or NoSQL (e.g., MongoDB) database for better data management.
 * Email/SMS Alerts: Implement custom logic to send notifications when a coin hits a certain price threshold or experiences a rapid change.
