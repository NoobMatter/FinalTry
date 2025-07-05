# iPhone Price Tool

A web application that provides real-time iPhone pricing information by combining Swappa market data with live eBay sold listings analysis.

## Features

- **Swappa Price Lookup**: Get current market prices from Swappa for various iPhone models and conditions
- **Live eBay Analysis**: Real-time scraping of eBay sold listings with intelligent filtering
- **Price Recommendations**: Suggested eBay listing prices based on market data
- **Comprehensive Coverage**: Supports iPhone 12 through iPhone 15 series
- **Mobile-Optimized**: Clean, responsive interface designed for mobile use

## How It Works

1. Select your iPhone model, condition, and storage capacity
2. Get instant Swappa pricing data
3. View average eBay sold prices (excluding broken/parts listings)
4. See recommended eBay listing prices
5. Direct links to filtered eBay sold listings

## eBay Filtering

The app uses advanced eBay filters to provide accurate pricing:
- **Condition Filters**: Excludes broken, parts-only, and heavily damaged listings
- **Network Filter**: Shows only unlocked devices for consistent pricing
- **Sold Listings Only**: Uses actual sold prices, not asking prices

## Tech Stack

- **Backend**: Python Flask with requests and BeautifulSoup4
- **Frontend**: Vanilla JavaScript with modern CSS
- **Data Processing**: Statistical analysis with outlier detection
- **Deployment**: Designed for easy hosting on platforms like Vercel, Heroku, or Railway

## Installation

1. Clone the repository:
```bash
git clone https://github.com/yourusername/iphone-price-tool.git
cd iphone-price-tool
```

2. Install dependencies:
```bash
pip install -r requirements.txt
```

3. Run the application:
```bash
python app.py
```

4. Open your browser to `http://localhost:5000`

## API Endpoints

- `GET /` - Main application interface
- `POST /api/ebay-average` - Get average eBay price for a specific URL
- `GET /health` - Health check endpoint

## Configuration

The app includes sample Swappa pricing data in `swappaData.json`. Update this file with current market prices as needed.

## Deployment

The app is configured for easy deployment:
- **Vercel**: Use the included `vercel.json` configuration
- **Heroku**: Includes `Procfile` for Heroku deployment
- **Railway/Render**: Compatible with standard Python hosting

## License

MIT License - feel free to use and modify as needed.

## Contributing

Pull requests welcome! Please ensure any changes maintain the mobile-first design and filtering accuracy.