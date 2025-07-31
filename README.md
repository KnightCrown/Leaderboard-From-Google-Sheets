# Fitness Leaderboard Generator
<img width="1579" height="815" alt="leaderboard-generator" src="https://github.com/user-attachments/assets/252667b0-bc1e-4623-8939-885205b8574a" />

A web-based leaderboard that Autogenerates fitness scores from Google Sheets.

## Setup Instructions

### 1. Configuration Setup

Before running the application, you need to set up your configuration:

1. Copy the template configuration file:
   ```bash
   cp config.template.js config.js
   ```

2. Edit `config.js` and replace the placeholder values with your actual credentials:
   - `apiKey`: Your Google Sheets API key
   - `spreadsheetId`: Your Google Sheets spreadsheet ID

### 2. Security Notes

- The `config.js` file contains sensitive information and is excluded from version control
- Never commit the `config.js` file to git
- The `config.template.js` file is safe to commit as it only contains placeholder values

### 3. Running the Application

Simply open `index.html` in a web browser. The application will:
- Load the configuration from `config.js`
- Fetch data from your Google Sheets
- Display weekly and monthly leaderboards

### 4. Google Sheets Setup

Ensure your Google Sheets:
- Has the correct structure with player names in column B
- Contains weekly scores in the specified columns (J, U, AF, AG, BB)
- Is publicly accessible or has proper API permissions

## File Structure

- `index.html` - Main application file
- `config.js` - Configuration file (not in version control)
- `config.template.js` - Configuration template
- `.gitignore` - Git ignore rules
- `README.md` - This documentation 
