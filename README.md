# IPL Match Predictor

A sophisticated machine learning application that predicts Indian Premier League (IPL) cricket match outcomes in real-time, with detailed player statistics and visualization.

## About

This IPL Match Predictor uses the XGBoost machine learning algorithm to forecast match outcomes in the Indian Premier League. The application analyzes historical match data, team statistics, toss results, and venue factors to generate predictions, then displays them through an interactive UI along with live match data and player statistics.

## Features

- **Real-time match prediction** with win probability percentages for both teams
- **Live match status updates** including current scores and game state
- **Detailed player statistics**:
  - Batting stats (runs, balls, 4s, 6s, strike rate)
  - Bowling stats (overs, maidens, runs, wickets, economy)
- **Match information** including venue, toss details, and recent ball commentary
- **Visualization** of win probability with color-coded bar charts
- **Auto-refreshing data** with manual refresh option
- **Error handling** with informative status messages

## Technologies Used

- **Python** for the core application
- **pandas** for data manipulation and analysis
- **numpy** for numerical operations
- **XGBoost** for the machine learning model
- **scikit-learn** for model evaluation and preprocessing
- **tkinter** for the graphical user interface
- **matplotlib** for data visualization
- **requests** for API data fetching
- **PIL** for image handling
- **logging** for application diagnostics

## Data Sources

The prediction model uses:
- Historical IPL match data (from the matches.csv file)
- Live match data from Cricket API
- The application features both predictive analytics and real-time data integration

## Model Methodology

This project employs an XGBoost classifier with hyperparameter tuning via GridSearchCV to predict match outcomes. The model is evaluated using 5-fold cross-validation and includes the following features:
- Team identities
- Toss winner
- Season
- Home advantage

## How to Use

1. Clone this repository to your local machine
2. Ensure you have Python installed with the required packages
3. Make sure you have the `matches.csv` file in the same directory
4. Run the Python script
5. The application will automatically fetch current IPL match data
6. View real-time predictions, match status, and player statistics
7. Use the "Refresh Now" button to manually update data

## Installation

```
git clone https://github.com/[your-username]/IPL-Match-Predictor.git
cd IPL-Match-Predictor
pip install -r requirements.txt
python ipl_predictor.py
```

## API Integration

The application uses the Cricket API to fetch live match data. You'll need to:
1. Register for an API key at cricapi.com
2. Replace the API key in the code with your own key
3. Ensure you have an active internet connection while running the application

## UI Features

The application includes a user-friendly interface with:
- Match prediction display
- Live score updates
- Win probability visualization
- Tabbed interface for batting stats, bowling stats, and match information
- Status indicators for data freshness and errors
- Manual refresh button

## Future Enhancements

- Enhanced player performance analysis
- Historical head-to-head statistics
- Individual player impact on match outcomes
- Improved data visualization with trend analysis
- Mobile application version

## License

This project is licensed under the MIT License - see the LICENSE file for details.

## Contact

[Justin/Justin13-OSS] - [ramdevrathwa@gmail.com]

Project Link: https://github.com/[your-username]/IPL-Match-Predictor
