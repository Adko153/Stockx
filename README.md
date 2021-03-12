# Stockx

/__pycache__
sales.csv
*.png
*.csv




v0.0.1
-Getting specific size product page via the Network tab
-Parsing the JSON file to retrieve last prices

v0.1.0
-Rewrite of the code
-Product pages from which data is retrieved is less of a hassle to find

v1.0.0
-CLI interface (using input()) -Drastic change of UX -Product pages fetched via keywords -Improvements of README.md file

v1.0.1
-CLI interface rewrite (using argparse) -Major improvements (code readility, comments, code structure) -Possibility to save info to a file

v1.0.2
-csv implementation -graphs creation

v1.0.3
-code readability improvements -UX improvements



Simple requests CLI based program to get last sales of a product from StockX

Requirements
Python 3

pip3 install -r requirements.txt
Commands
git clone
cd stockx-sneakers-prices
python3 src/scraper.py --keywords your keywords
Example

python3 src/scraper.py jordan 1 mocha
This will look for the 250 last sales of the Jordan 1 Mocha.

By default, it will retrieve the last 250 sales but can be less if there has not been that many.

Current features
 Ask for keywords (argparse)
 Retrieving last sales
 Saving data as a csv file
 Dataframes creation (pandas)
 Charts creations (matplotlib)
Upcoming features
 machine learning models implementation (sklearn)
 deep learning implementation to predict prices (tensorflow)
CLI UX (argparse)
It asks the user for the keywords.

Retrieving last sales
Getting data using Requests python module

Saving them to a file
Simple .csv format saving

Plots creation
Plots creation will be created grouping sales by periods (7-day or 1-month for instance) and saved as a .png file


  
requests==2.24.0
numpy==1.19.2
pandas==1.1.3
matplotlib==3.3.2
