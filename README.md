# Football Match Data Scraper

This project is a Python-based web scraper that extracts football match data, including date, home team, goals, and away team, from the [Adam Choi Football Stats](https://www.adamchoi.co.uk/overs/detailed) website. The scraper allows users to select a country, league, and season, then saves the extracted match data in a CSV file.

## Features

- Interact with a website using **Selenium WebDriver** to navigate and select specific football matches.
- Extract match data such as date, home team, goals, and away team.
- Save the scraped data in a structured **Pandas DataFrame**.
- Export the match data to a **CSV** file for further analysis.

## Project Setup

### Prerequisites

Ensure you have the following installed before running the project:

1. **Python** (version 3.x)
2. **Google Chrome** and **ChromeDriver** (Ensure the version of ChromeDriver matches your Chrome browser version)
3. Python packages: 

   - **Selenium**
   - **Pandas**

To install the required packages, run:

```bash
pip install selenium pandas
```

### Running the Scraper
  - Run the script in your terminal or IDE.
  - Input a Country name (e.g., Spain, Saudi Arabia) when prompted.
  - Select the League and Season based on the displayed options.
  - The script will scrape match data and output it as a CSV file named in the format Country_League_Season.csv.

### Sample Usage
```
  Enter a football Country Name: Spain
  Spain League's -
  La Liga
  Segunda Division
  
  Spain Season's -
  2022/2023
  2021/2022
  
  Enter a Football League: La Liga
  Enter a Football Season: 2022/2023
```
The scraper will collect the football match data for the selected country, league, and season, then store the data in a CSV file like **Spain_La_Liga_2022_2023.csv**.


### Error Handling
  - The script handles invalid inputs (e.g., incorrect league or season names) by providing prompts for the correct input.
  - If a CSV file cannot be created due to a naming issue, the script prompts for a different name.

