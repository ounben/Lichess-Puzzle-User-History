# Lichess Puzzle Activity Downloader

This Python script retrieves puzzle activity data from Lichess using the Lichess API, processes it, and saves it to a CSV file. It's designed to be used in a Google Colab environment for easy data retrieval and download.

## Features

* Fetches puzzle activity data from Lichess.
* Uses the `python-lichess` library for efficient API interaction.
* Handles API errors gracefully.
* Converts timestamps to datetime objects.
* Saves data to a CSV file named with the current date (YYYYMMDD_puzzle_activity_clean.csv).
* Automatically downloads the CSV file in Google Colab.

## Requirements

* Python 3
* `python-lichess` library: Install with `pip install python-lichess`
* `pandas` library: Install with `pip install pandas`
* Google Colab (recommended for easy execution and download)

## Usage


Open in Google Colab: The easiest way to use this script is within Google Colab. Create a new Colab notebook and copy the Python code into a cell.

## Install dependencies: In a local machine, run:
pip install lichess
pip install requests
pip install pandas

## Install dependencies: In a Colab cell, run:

Bash

!pip install python-lichess pandas

Replace API Token: IMPORTANT: Replace the placeholder API token ("lip_...") in the Python code with your actual Lichess API token. You can obtain your token from your Lichess account settings (https://lichess.org/account/oauth/authorize). Never commit your API token directly to your repository.

Run the script: Execute the Colab cell containing the Python code.

Download the CSV: The script will automatically download the generated CSV file to your local machine.

## Code Explanation
The Python script uses the lichess.Client to interact with the Lichess API. It retrieves puzzle activity, parses the JSON response, converts timestamps to datetime objects, and saves the data to a CSV file. The filename includes the current date for easy tracking. Error handling is included to catch potential issues with the API request.

Example


token = "YOUR_LICHESS_API_TOKEN"  # Replace with your actual token!

Contributing
Contributions are welcome! Please open an issue or submit a pull request if you have any suggestions or improvements.

License
This project is licensed under the GNU General Public License v3.0. See the LICENSE file for details.
