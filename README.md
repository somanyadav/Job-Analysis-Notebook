# Job Analysis Notebook

Welcome to the README for the Job Analysis Notebook. This Jupyter Notebook is an innovative tool designed to automate the process of job searching and analysis. It's tailored for professionals seeking opportunities at Thomson Reuters, but with a bit of tweaking, it can adapt to any career page.

## Introduction

The Job Analysis Notebook is a powerful blend of web scraping and AI analysis. It scrapes job listings from Thomson Reuters' career page and then uses an AI model to evaluate these opportunities against your resume. The focus is on matching job requirements, especially years of experience, with your professional profile.

## Getting Started

### Prerequisites

- Jupyter Notebook or JupyterLab environment.
- Python 3.x installed within the Jupyter environment.
- Libraries: Selenium, BeautifulSoup4, OpenAI.
- Chromium WebDriver for Selenium.

### Installation

1. **Setting Up Jupyter Notebook**:
   If you don't have Jupyter Notebook installed, you can install it via Anaconda or using pip:

   ```bash
   pip install notebook
   ```

2. **Install Required Libraries**:
   Open your Jupyter Notebook and install the necessary Python libraries:

   ```python
   !pip install selenium beautifulsoup4 openai
   ```

3. **Chromium WebDriver Setup**:
   The script requires ChromeDriver for Selenium. Install it as follows:

   ```python
   !apt-get update
   !apt install chromium-chromedriver
   ```

   Add ChromeDriver to your PATH in the notebook:

   ```python
   import sys
   sys.path.insert(0,'/usr/lib/chromium-browser/chromedriver')
   ```

## How to Use

1. **Launch the Notebook**:
   Open the Job Analysis Notebook in your Jupyter environment.

2. **Enter Your Resume Details**:
   Modify the `resume` and `yoe` (years of experience) variables with your information.

3. **Run the Notebook**:
   Execute each cell sequentially. The notebook performs the following actions:
   - Scrapes job listings from Thomson Reuters.
   - Analyzes each job's suitability based on your resume.

4. **Interpreting Results**:
   The notebook outputs:
   - Scraped job titles and URLs.
   - A detailed analysis for each job, indicating suitability.

## Notebook Highlights

- **Interactive and User-Friendly**: Jupyter Notebook allows for an interactive experience, where you can tweak parameters and instantly see the results.
- **Visualization**: The notebook can be extended to include data visualizations for a more engaging analysis.
- **Customization**: Easily adaptable for different job portals or criteria.

## Customization Tips

- **Adapting to Different Job Portals**: Change the scraping logic to adapt to different websites.
- **Enhancing Analysis**: Modify the AI analysis section to include more resume parameters.

## Example Code Snippets

- **Initial Setup**:

  ```python
  from selenium import webdriver
  from selenium.webdriver.chrome.options import Options
  # Selenium setup code
  ```

- **Web Scraping Logic**:

  ```python
  driver.get("https://careers.thomsonreuters.com/")
  # Code to scrape job listings
  ```

- **AI Analysis**:

  ```python
  for job_url, job_description in job_details.items():
      # Analysis code using OpenAI
  ```

---
