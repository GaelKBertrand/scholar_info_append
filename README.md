# Google Scholar Profiles Scraping and Processing

## Overview

This Jupyter Notebook is designed to scrape data from Google Scholar profiles and process the data in batches. It handles the extraction of profile information, performs necessary data transformations, and saves the processed data to a CSV file. 

## Prerequisites

Before you can run this notebook, you need to have the following installed:
- Python 3.7 or later
- Jupyter Notebook or Google colab
- Required Python libraries can be found in the notebook

## Setup

1. **Google API Key and Custom Search Engine ID**:
   - Obtain a Google API Key from the [Google Cloud Console](https://console.cloud.google.com/).
   - Create a Custom Search Engine (CSE) and get the CSE ID from the [Custom Search JSON API](https://developers.google.com/custom-search/v1/overview).

2. **Credentials Configuration**:
   - Replace the placeholder `API_KEY` and `CSE_ID` in the notebook with your actual credentials.

## Notebook Structure

The notebook is divided into several sections:

1. **Library Imports**:
   - Necessary libraries are imported at the beginning.

2. **Constants and Configuration**:
   - API Key, CSE ID, and other constants are defined.

3. **Helper Functions**:
   - Functions to initialize the Custom Search API, scrape Google Scholar profiles, and handle data transformations are implemented.

4. **Data Processing**:
   - The main logic for scraping and processing data in batches.
   - Handles issues related to dtype compatibility and warnings related to setting values in a DataFrame.

5. **Output**:
   - Processed data is saved to a CSV file.

## Usage

1. **Initialization**:
   - Ensure that the `API_KEY` and `CSE_ID` are correctly set in the notebook.
   - Initialize the Custom Search API using the provided helper function.

2. **Scraping Profiles**:
   - Run the provided cells to scrape data from Google Scholar profiles.
   - Data is processed in batches to handle large datasets efficiently.

3. **Data Transformation**:
   - Additional transformations can be applied to the data as needed.
   - Optional code snippets are provided but should be ignored unless specifically required.

4. **Saving Results**:
   - The processed data is saved to a CSV file at the end of the notebook.

## Optional Code

Some optional code snippets are included in the notebook for extracting institution names and initializing the Custom Search API. These should not be run unless necessary for specific use cases. These sections are in the notebook with clear comments. 


## Issues and Troubleshooting

- **Warnings Related to DataFrame Operations**:
  - Ensure that you handle dtype compatibility issues properly when setting values in a DataFrame.
  - Use appropriate pandas methods to avoid SettingWithCopyWarning.

- **API Limits**:
  - Be aware of the rate limits imposed by the Google Custom Search API.
  - Implement necessary delays or batching to stay within the allowed limits.

## Contribution

Contributions to improve the notebook are welcome. Feel free to fork the repository and submit pull requests.

## License

This project is licensed under the MIT License.