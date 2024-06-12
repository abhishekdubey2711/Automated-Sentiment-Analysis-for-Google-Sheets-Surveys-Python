# Python Automation of Google Sheets and Sentimental Analysis

### About

###### This Python script automates sentiment analysis of feedback collected within a Google Sheet survey. It leverages the Google Sheets API and TextBlob library to analyze sentiment and populate a new column in the spreadsheet with the corresponding sentiment label ("Positive," "Negative," or "Neutral").

### Features

###### Automates repetitive sentiment analysis tasks.
Integrates seamlessly with Google Sheets.
Utilizes the popular TextBlob library for accurate analysis.
Provides clear feedback messages for successful execution.
Requirements

Python 3 (tested with 3.x)
TextBlob library (pip install textblob)
A Google Sheet with a survey form response sheet named "Form Responses 1" (configurable)
#Installation

##### Create a new Python project directory.
- Install the required library: pip install textblob
- Set up Google Sheets API credentials and save them as credentials.json following the instructions in the Google Sheets API quickstart guide (https://www.youtube.com/watch?v=BeIwYBfWPVs).
- (Optional) Update the script's variables (spreadsheet_id and feedback_column) to match your specific Google Sheet configuration.
#Usage

###### Place the Python script (named sentiment_analysis.py or any preferred name) in your project directory.
Ensure credentials.json is located within the same directory.
Run the script from your terminal using python sentiment_analysis.py.
Output

Upon successful execution, the script will print a confirmation message indicating that the sentiment analysis results have been updated in your Google Sheet.
The script also includes a print statement displaying the batch update response from the Google Sheets API for debugging purposes (optional to remove if desired).
Contributing

Feel free to submit pull requests or issues to improve this script. We appreciate your contributions!

## Disclaimer

This script is provided for educational purposes only. While TextBlob offers a decent level of accuracy, consider exploring more advanced sentiment analysis tools for production use cases.Note:

##### The script assumes the feedback column is located at index 15 (16th column) in the Google Sheet. Adjust the feedback_column variable if this differs.
Error handling can be further enhanced to provide more specific feedback in case of issues.
