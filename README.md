# Telegram Channel Scraper

This branch extends the functionality of the main project by adding the ability to scrape data from Telegram channels and download media files, using the `Telethon` library. The scraped data is stored in a CSV file, including any attached media (e.g., photos).

## Features
- Scrapes up to 10,000 messages from specified Telegram channels.
- Downloads media (photos) from messages and saves them locally.
- Stores message metadata such as channel title, message text, date, and media file path in a CSV file.
- Easily configurable via environment variables for `api_id`, `api_hash`, and `phone`.

## Prerequisites
1. **Python 3.7+**
2. A Telegram API account. [Create one here](https://my.telegram.org/auth).
3. Required libraries:
   - `telethon`
   - `python-dotenv`

You can install the dependencies with:

```bash
pip install -r requirements.txt
