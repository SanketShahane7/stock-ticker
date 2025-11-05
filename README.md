# Stock Predictions

A fun and interactive web application that provides "predictions" for stock market tickers. Built with vanilla JavaScript, this application allows users to input up to 3 stock tickers and generates a humorous report about their potential performance.

## Features

- Input up to 3 stock tickers
- Real-time stock data fetching from Polygon.io API
- Interactive UI with loading states
- Responsive design
- Humorous predictions and reports

## Prerequisites

- Node.js (for development)
- A Polygon.io API key

## Setup

1. Clone the repository:
```bash
git clone [repository-url]
cd stock-ticker
```

2. Create a `.env` file in the root directory and add your Polygon.io API key:
```
POLYGON_API_KEY=your_api_key_here
```

3. Open `index.html` in your browser or use a local development server.

## Running the Project

### Method 1: Using a Local Development Server (Recommended)

1. Install a local development server (if you don't have one):
```bash
npm install -g live-server
```

2. Start the development server:
```bash
live-server
```
The application will automatically open in your default browser at `http://localhost:8080`

### Method 2: Using Python's Built-in Server

If you have Python installed, you can use its built-in HTTP server:

For Python 3:
```bash
python -m http.server 8000
```

For Python 2:
```bash
python -m SimpleHTTPServer 8000
```

Then open `http://localhost:8000` in your browser.

### Method 3: Direct File Opening

You can also open the `index.html` file directly in your browser, but some features might not work due to CORS policies when making API requests.

## Project Structure

```
stock-ticker/
├── index.html          # Main HTML file
├── index.js           # Main JavaScript file
├── index.css          # Styles
├── utils/
│   └── dates.js       # Date utility functions
├── images/            # Project images and assets
└── .env              # Environment variables (not tracked in git)
```

## Usage

1. Enter a stock ticker (e.g., MSFT, AAPL, TSLA) in the input field
2. Click the add button to add the ticker
3. Add up to 3 tickers
4. Click "Generate Report" to get your prediction
5. View your humorous stock prediction report

## API Integration

The application uses the Polygon.io API to fetch real stock data. The API is called with the following parameters:
- Time range: Last 3 days of trading data
- Interval: Daily
- Ticker: User-provided stock symbols

## Development

The project uses vanilla JavaScript with ES6 modules. No build process is required to run the application.

## Disclaimer

This is a fun project and not meant to provide real financial advice. The tagline "Always correct 15% of the time!" should be taken as a joke.

## License

[Add your license here]

## Contributing

Feel free to submit issues and enhancement requests! 
