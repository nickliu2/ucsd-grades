# UCSD SET Project

## Overview
This project involves scraping, cleaning, and analyzing course evaluation data from the newly introduced Student Evaluation of Teaching website (SET). The goal is to create a comprehensive dataset that can be used for various analyses, such as understanding instructor performance, course difficulty, and student satisfaction. **Data from SET from S123 to WI24** is in `SET_WI24.csv`.

## Features
- Scraping detailed course evaluation data from the UCSD SET.
- Cleaning and preprocessing the dataset to ensure accuracy and consistency.
- Documenting the process and maintaining a structured approach to data collection and cleaning.
- Collecting approximately 5000 course evaluations from several hundred tables (one table per course).

## Installation

### Prerequisites
- Python 3.7 or higher
- Google Chrome
- Anaconda or Miniconda
- Required Python packages: `selenium`, `pandas`, `beautifulsoup4`, `notebook`
- Cookies from a SET session. Export a cookie json file while logged into SET page and create a json file called `academicaffairs.ucsd.edu.cookies.json` copy and paste cookie information into json file. Extension I used here: ([link](https://chromewebstore.google.com/detail/export-cookie-json-file-f/nmckokihipjgplolmcmjakknndddifde?pli=1))

### Setup
1. **Clone the repository:**
    ```
    git clone git@github.com:nickliu2/ucsd-grades.git
    ```

2. **Create and activate a Conda environment:**
- Access the directory and run:
    ```
    conda env create -f environment.yml
    ```

3. **Activate the environment:**
    ```
    conda activate ucsd-grades
    ```

## Process Documentation
- **Data Scraping:** Used Selenium and BeautifulSoup to automate the extraction of course evaluation data from the UCSD SET website. This involved navigating through multiple pages, handling cookies, and extracting data from tables.
- **Data Cleaning:** Processed the raw data to handle missing values, convert data types, and ensure consistency. This step ensures that the data is ready for analysis.
- **Data Collection:** Successfully collected approximately 5000 course evaluations from several hundred tables, with each table corresponding to a different course.

## Contributing
If you wish to contribute to this project, please fork the repository and submit a pull request. For major changes, please open an issue to discuss what you would like to change.

## Thanks to ...
[This reddit post](https://www.reddit.com/r/UCSD/comments/14uh5q5/since_capes_is_being_retired_i_scraped_all_its/) about scraping CAPEs to inspire me to scrape SET.
