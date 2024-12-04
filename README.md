# Telegram Channel Parser (Unofficial)

A Python application to parse Telegram channels using web version without official API.

## Features

- Parse public Telegram channels without API credentials
- Save messages to JSON files with timestamps
- Collect message ID, date, text, view count and post links
- Support for both channel usernames and full links

## Setup

1. Create a virtual environment and activate it:
```bash
python3 -m venv venv
source venv/bin/activate  # On Windows use: venv\Scripts\activate
```

2. Install dependencies:
```bash
pip install -r requirements.txt
```

## Usage

1. Run the application:
```bash
python app.py
```

2. Enter the Telegram channel username or link when prompted
   - You can use either @username format
   - Or full link format: https://t.me/username

3. The application will download all messages and save them to a JSON file
   - The filename will include the channel name and timestamp
   - Each message will contain: ID, date, text, and views count

4. You can parse multiple channels in one session

## Notes

- This parser uses the public web version of Telegram
- Only public channels are supported
- Rate limiting is implemented to avoid being blocked
- Some very old messages might not be accessible