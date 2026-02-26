# API Integrations in Python

A collection of small Python examples that show how to integrate with popular external APIs.

## Included Integrations

1. **Oxford Dictionary API**
   - Search related words for a query.
   - Fetch definitions for a selected word.
2. **OpenWeatherMap Forecast API**
   - Retrieve 5-day forecast data for a city.
   - Print weather details such as temperature, humidity, pressure, and description.
3. **YouTube Data API v3**
   - Search YouTube content by keyword.
   - Group and print results by videos, channels, and playlists.

## Project Structure

```text
API-Integrations-Python/
|- Oxford_Dictionary/
|  |- main.py
|  |- readme.md
|  \- oxford_search.png
|- Weather_forecast/
|  |- main.py
|  |- readme.md
|  |- weather.png
|  \- file_log.png
|- Youtube/
|  |- main.py
|  |- readme.md
|  \- youtube_search.png
\- README.md
```

## Prerequisites

- Python 3.8+
- Internet connection
- API credentials for each service you want to use

## Install Dependencies

From the repository root:

```bash
pip install requests google-api-python-client
```

## API Credentials

Each script uses placeholders in `main.py`. Replace them with your own keys:

- `Oxford_Dictionary/main.py`
  - `app_id`
  - `app_key`
- `Weather_forecast/main.py`
  - `app_id`
- `Youtube/main.py`
  - `DEVELOPER_KEY`

## Run the Scripts

### 1) Oxford Dictionary

```bash
cd Oxford_Dictionary
python main.py
```

Before running, update `word_id` in `main.py` with the word you want to search.

### 2) Weather Forecast

```bash
cd Weather_forecast
python main.py
```

The script prompts for:

- city name
- country code (for example: `US`, `IN`, `GB`)

### 3) YouTube Search

```bash
cd Youtube
python main.py --q "python api" --max-results 10
```

## API Documentation

- Oxford Dictionary: https://developer.oxforddictionaries.com/
- OpenWeatherMap Forecast: https://openweathermap.org/forecast5
- YouTube Data API v3: https://developers.google.com/youtube/v3

## Notes

- These are educational examples focused on basic request/response flow.
- Credentials are currently read from source code placeholders. For production, move keys to environment variables or a secure secrets manager.
- Check each subfolder's `readme.md` for script-specific details.
