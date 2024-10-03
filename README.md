# Telegram Channel Scraper and Data Cleaner (Branch)

This branch extends the main project by adding functionality for scraping and cleaning Telegram channel data, with a focus on extracting and labeling entities like products, prices, and locations.

## Features
- Scrapes up to 10,000 messages from specified Telegram channels.
- Downloads attached media (e.g., photos) and stores them locally.
- Saves message metadata such as channel title, message text, date, and media file paths to a CSV file.
- Cleans message data by removing emojis, unwanted patterns, and specific Telegram handles.
- Replaces stylized number emojis with ordinary numbers.
- Labels entities like product names, prices, and locations in messages for downstream Named Entity Recognition (NER) tasks.

## Prerequisites
1. **Python 3.7+**
2. Telegram API account. [Create one here](https://my.telegram.org/auth).
3. Required libraries:
   - `telethon`
   - `python-dotenv`
   - `pandas`
   - `re`

You can install the dependencies with:
    ```bash
        pip install -r requirements.txt

## Data Cleaning and Labeling
- Removes emojis and specific patterns like @awasadmin1 and t.me/AwasMart.
- Replaces number emojis (e.g., 1⃣) with numeric characters (e.g., 1).
- Labels tokens in messages as B-PRODUCT, I-PRICE, or I-LOC for product names, prices, and locations, respectively.
### Output
The processed and labeled messages are saved in both CSV and CoNLL formats, ready for further analysis or model training.