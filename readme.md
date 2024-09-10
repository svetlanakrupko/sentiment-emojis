

# Telegram Message Sentiment Analyzer using emojis

## Overview
This script processes a JSON file containing Telegram messages to analyze sentiment and keyword occurrences over specified date ranges. It aggregates message counts, sentiment scores, and keyword frequencies, and formats the results for further use.

## Prerequisites
- Python 3.x

## Setup

1. **Install Dependencies**:
   - No additional libraries are required beyond the Python standard library.

2. **Input File**:
   - Ensure `pre-parsed_messages.json` is present in the same directory as the script. This file should contain the JSON data of messages.

3. **Keywords**:
   - Modify the `keywords` list to include any specific keywords you want to track.

4. **Date Ranges**:
   - Update the `periods_map` dictionary to define the date ranges and their corresponding week numbers.

## Script Workflow

1. **Read Data**:
   - Loads the JSON data from `pre-parsed_messages.json`.

2. **Initialize Analysis**:
   - Sets up dictionaries to store aggregated sentiment and keyword data for each channel.

3. **Analyze Messages**:
   - Processes each message to compute sentiment scores, emoticon counts, and keyword occurrences based on predefined criteria.

4. **Generate Results**:
   - Converts the analyzed data into a structured format, including channel details, for further analysis.

## Usage

Run the script using Python:

```bash
python your_script_name.py
```

## Output
- The script processes and analyzes the data, storing the results in the `result` variable. Modify the script as needed to save the output to a CSV or JSON file.

## Notes
- Ensure that the `pre-parsed_messages.json` file is correctly formatted with the required fields (`channel_url`, `date`, `message`, `reactions`, `city`, `region`).
- Adjust the `periods_map` and `keywords` according to your data analysis needs.

