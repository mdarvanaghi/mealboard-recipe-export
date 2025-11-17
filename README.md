# Mealboard Recipe Exporter
This script goes to your [Mealboard](http://mealboard.com) account and downloads all of the recipes. Mealboard has switched to storing and returning the recipes as JSON, so we're just leaving them as-is in that format for now.

## Usage
Create a `.env` file with the following environment variables:
- `MEALBOARD_EMAIL` - Your Mealboard email address
- `MEALBOARD_PASSWORD` - Your Mealboard password

These should match what you use for Mealboard to sync.

**Note:** The script uses `MEALBOARD_EMAIL` instead of `USERNAME` to avoid conflicts with the Windows system `USERNAME` environment variable.

Run the file:

`python3 mealboard.py`

This will download all of the recipes from Mealboard's website as json, leaving the converted files in the recipes folder.

### Warnings:
This doesn't well handle unexpected situations yet. Feel free to fix and make a PR for it, or I'll get to it eventually. For now:

* Supports Python 3 only