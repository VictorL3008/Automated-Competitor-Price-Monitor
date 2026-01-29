# 🕵️‍♂️ Automated Competitor Price Monitor

### 🚀 Project Overview
In the competitive E-commerce landscape, pricing strategies must be dynamic. This project is an **automated web scraping tool** designed to extract, structure, and analyze product data from online retailers.

It simulates a real-world "Competitor Intelligence" scenario where a business needs to monitor pricing and stock availability across thousands of SKUs in real-time, eliminating the need for manual data entry.

### 🛠️ Key Features
* **Multi-Page Crawling:** Automated pagination logic to traverse through product catalogs (not just single pages).
* **Resilient Architecture:** Implemented `try/except` blocks to handle connection errors without crashing.
* **Ethical Scraping:** Integrated `time.sleep()` delays (Rate Limiting) to respect server load and prevent IP blocking.
* **Data Structuring:** Converts unstructured HTML data into a clean, analytical Dataset (Pandas DataFrame / CSV).

### 💻 Tech Stack
* **Python 3.12**
* **Requests:** For handling HTTP sessions.
* **BeautifulSoup4:** For HTML parsing and DOM traversal.
* **Pandas:** For data transformation and export.

### 📊 Sample Output
The script generates a structured dataset including:
| Title | Price (£) | Stock Status | Page Source |
| :--- | :--- | :--- | :--- |
| A Light in the Attic | 51.77 | In stock | 1 |
| Tipping the Velvet | 53.74 | In stock | 1 |
| Soumission | 50.10 | In stock | 1 |

*(Data extracted from the sandbox environment: books.toscrape.com)*

### 🔧 How to Run
1. Clone this repository.
2. Install dependencies:
   ```bash
   pip install requests beautifulsoup4 pandas
