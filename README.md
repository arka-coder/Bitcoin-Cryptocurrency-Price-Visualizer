# Bitcoin-Cryptocurrency-Price-Visualizer
### Bitcoin Price Visualizer
This project visualizes Bitcoin (BTC) to US Dollar (USD) exchange rate data from various exchanges using Python. It retrieves historical data from the Quandl API, processes it using the pandas library, and creates interactive plots with Plotly.

### Project Overview
The primary goal of this project is to fetch, analyze, and display historical Bitcoin price data. It uses several major exchanges as data sources to provide a comprehensive view of the market. To optimize performance and avoid redundant API calls, the data is cached locally in .pkl files after the first retrieval.

### Features
- Multi-Exchange Data: Fetches data from Bitstamp, Coinbase, itBit, and Kraken.

- Data Caching: Saves downloaded data to local pickle files (.pkl) to speed up subsequent runs.
 
- Interactive Visualizations: Uses Plotly to generate interactive charts, allowing for zoom, pan, and data inspection on hover.
 
- Cloud Publishing (Optional): Includes functionality to publish generated plots to Plotly's Chart Studio for easy sharing.

### Data Sources
This visualizer uses the following datasets from the Quandl API:

BCHARTS/BITSTAMPUSD: Bitstamp USD

BCHARTS/COINBASEUSD: Coinbase USD

BCHARTS/ITBITUSD: itBit USD

BCHARTS/KRAKENUSD: Kraken USD


### Install dependencies:
- Run the following command in your terminal to install the required Python libraries.
  
- pip install numpy pandas pickle5 quandl plotly chart-studio ipywidgets
  
- Configure API Keys:
  
- Quandl API Key: You will need a free API key from Quandl. Once you have your key, open the BTC-Visualizer.ipynb notebook and replace the placeholder in the following line:
  
- quandl.ApiConfig.api_key = 'YOUR_API_KEY'
  
- Chart Studio Credentials (Optional): If you want to save your plots to the cloud, sign up for a free account at Chart Studio to get your username and API key. Then, update the following lines in the notebook:
  
- import chart_studio
- chart_studio.tools.set_credentials_file(username='YourUserName', api_key='YourAPIKey')

### Usage

Create and display interactive plots of the Bitcoin prices.

File Descriptions
BTC-Visualizer.ipynb: The main Jupyter Notebook for visualizing the data.

Untitled.ipynb: A scratchpad notebook, likely used for initial exploration.

BCHARTS-*.pkl: Pickle files containing cached data for each Bitcoin exchange.

Contributing
Contributions are welcome! If you have suggestions for improvements, please feel free to fork the repository and submit a pull request. You can also open an issue with the tag "enhancement".

Fork the Project

Create your Feature Branch (git checkout -b feature/AmazingFeature)

Commit your Changes (git commit -m 'Add some AmazingFeature')

Push to the Branch (git push origin feature/AmazingFeature)

Open a Pull Request
