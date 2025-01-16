# Cars.com Web Scraper
![image](https://github.com/user-attachments/assets/82c7c439-5346-459b-b469-f21130b96dc4)

This project is a web scraper designed to collect car listings data from [Cars.com](https://www.cars.com/). It extracts information about cars such as make, model, price, location, mileage, and other relevant attributes to build a structured dataset for analysis or further processing.

---

## Features

- Scrapes detailed car listing information, including:
  - Make, model, year, and price
  - Mileage
  - Vehicle condition and other key attributes
- Paginated scraping, handling multiple pages of listings
- Saves scraped data to CSV format for easy analysis
- Configurable options for customizing the scraping process

---

## Folder Structure

```bash
├── code/               # Contains all scraping logic and utility functions
│   └─ scraper.py      # Main scraper script
├── data/               # Folder to store scraped data files
│   └─ cars_data.csv   # Sample CSV output file with car listings
├── README.md           # Project documentation
└── requirements.txt    # List of dependencies
```

---

## Prerequisites

Ensure you have the following installed:
- Python 3.x (preferably 3.7+)
- Required Python libraries (can be installed via `pip`)

---

## Installation

1. **Clone the repository**:

   ```bash
   git clone https://github.com/yourusername/cars.com-web-scraper.git
   cd cars-com-web-scraper
   ```

2. **Create a virtual environment** (optional but recommended):

   ```bash
   python -m venv venv
   source venv/bin/activate  # On Windows use `venv\Scripts\activate`
   ```

3. **Install required libraries**:

   ```bash
   pip install -r requirements.txt
   ```

---

## Usage

1. **Run the scraper**:
   - Navigate to the `code/` folder, then run the `scraper.py` script:
   
   ```bash
   python scraper.py
   ```

   The script will start scraping data from Cars.com, fetching car listings based on predefined parameters (e.g., price range, location, etc.).

2. **Output**:
   - The data will be saved in the `data/` folder in CSV and JSON formats, which can be used for further analysis or processing.

3. **Customization**:
   - Modify `scraper.py` to customize the parameters, such as:
     - **Location**
     - **Price range**
     - **Car make and model**
     - **Number of pages to scrape**
   
   For example, adjust the starting URL in the script to scrape listings from a different location or set of conditions.

---

## Dependencies

The following Python libraries are required:

- `requests`: For making HTTP requests to the Cars.com website
- `BeautifulSoup4`: For parsing HTML and extracting car listing information
- `pandas`: For saving data in CSV format (optional but recommended)
- `json`: For saving data in JSON format

You can install these dependencies using:

```bash
pip install -r requirements.txt
```

---

## Contributing

We welcome contributions to improve this project! Here's how you can get involved:

1. Fork the repository
2. Create a new branch (`git checkout -b feature-name`)
3. Commit your changes (`git commit -am 'Add new feature'`)
4. Push to the branch (`git push origin feature-name`)
5. Open a pull request with a description of your changes

---

## License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

---

## Acknowledgments

- [BeautifulSoup](https://www.crummy.com/software/BeautifulSoup/) for web scraping
- [Requests](https://requests.readthedocs.io/en/master/) for HTTP requests
- [Cars.com](https://www.cars.com) for the dataset

---

## Enhancing the Project

If you're looking to make this project even more useful, here are a few ideas:
- Add support for scraping more detailed attributes (e.g., car history reports, seller details)
- Introduce multi-threading to speed up scraping
- Provide a command-line interface (CLI) for easier customization and interaction
- Implement a database to store scraped data instead of flat files

---

## Example Output

Here’s a small preview of the kind of data you can expect from the scraper:

**CSV format:**

| Make & Model                              | Mileage    | Dealer Name                    | Rating | Review Count | Price   |
|-------------------------------------------|------------|---------------------------------|--------|--------------|---------|
| 2019 Mercedes-Benz AMG GLS 63 Base 4MATIC | 37,071 mi. | Mercedes-Benz of Pompano        | 4.5    | 607          | $89,998 |
| 2020 Mercedes-Benz GLE 350 Base 4MATIC    | 35,197 mi. | Mercedes-Benz of Rochester      | 2.5    | 3            | $59,987 |
| 2018 Mercedes-Benz GLE 350 Base 4MATIC    | 40,294 mi. | Mercedes-Benz of Rochester      | 4.7    | 101          | $43,940 |
| 2020 Mercedes-Benz GLE 350 Base 4MATIC    | 55,853 mi. | Mercedes-Benz of Des Moines    | 4.5    | 300          | $55,881 |
| 2016 Mercedes-Benz GLE-Class GLE 350 4MATIC| 51,375 mi. | Mercedes-Benz of Manchester    | 4.4    | 482          | $34,588 |

---
