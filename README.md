# Kenya Trade Chatbot

## Overview
The **Kenya Trade Chatbot** is an AI-powered tool that leverages **Retrieval-Augmented Generation (RAG)** to provide insights into Kenya's trade data. The chatbot interacts with a database to answer natural language questions, perform trade data analysis, and evaluate tariff impacts. Built using **Vanna AI**, this project is designed to streamline trade data exploration.

## Features
- **Natural Language Interaction**: Users can query the chatbot to retrieve trade-related insights.
- **Trade Data Analysis**: Executes SQL queries to provide trends, comparisons, and summaries.
- **Customizable Insights**: Generates results for exports, imports, trade balances, and tariff impacts.
- **Sector Focus**: Highlights Kenya's comparative advantage in key sectors.
- **Tariff Analysis**: Explores the influence of AHS and MFN tariffs on trade performance.

## Project Structure
```
/chatbot/TradeAnalysis
│
├── /data
│   ├── trade_data.db       # SQLite database with trade data
│
├── /models
│   ├── tradebot     # Trained Vanna model for RAG
│
├── /src
│   ├── app.py              # Main chatbot application
│   ├── analysis.ipynb      # Model training and Predefined SQL queries for RAG
│   ├── vanna_calls.py      # Preprocessing scripts for database setup
│
├── /utils
│   ├── logger.py           # Logging utilities
│   ├── config.py           # Configuration settings
│
├── .gitignore              # Git ignored files and directories
├── README.md               # Project documentation
└── requirements.txt        # Python dependencies
```

## Installation

### Prerequisites
- Python 3.8 or higher
- SQLite installed
- Virtual environment tools (e.g., `venv`)

### Setup Steps
1. **Clone the Repository**:
   ```bash
   git clone https://github.com/LubangaD/kenyatradechatbot.git
   cd kenyatradechatbot
   ```

2. **Set Up a Virtual Environment**:
   ```bash
   python -m venv venv
   source venv/Scripts/activate  # For Windows: venv\Scripts\activate
   ```

3. **Install Dependencies**:
   ```bash
   pip install -r requirements.txt
   ```

4. **Add Database**:
   - Ensure `trade_data.db` is located in the `/data` directory.

5. **Run the Chatbot**:
   ```bash
   streamlit run app.py
   ```

## Usage
### Example Queries
- "What are the top 5 export products from Kenya?"
- "What is the total trade balance for Europe & Central Asia?"
- "How do duty-free tariffs impact agricultural imports?"
- "What is the trend in vegetable exports over the years?"

### Key Functionalities
- **Insight Generation**: Ask natural language questions to receive SQL-driven insights.
- **Trend Analysis**: Get data visualizations or summaries for trade performance.
- **Comparative Advantage**: Learn which sectors offer Kenya the greatest potential for growth.

## Contributions
Contributions are welcome! Please create a branch, make your changes, and submit a pull request.

1. Fork the repository.
2. Create a feature branch:
   ```bash
   git checkout -b feature-name
   ```
3. Commit your changes:
   ```bash
   git commit -m "Description of changes"
   ```
4. Push to the branch:
   ```bash
   git push origin feature-name
   ```
5. Submit a pull request.

## License
This project is licensed under the MIT License. See `LICENSE` for more details.

## Acknowledgements
- Built using [Vanna AI](https://www.vanna.ai).
- Inspired by Kenya’s economic and trade data.

## Contact
For inquiries or support, please reach out via:
- **Email**: [derrick.lubanga@strathmore.edu](mailto:derrick.lubanga@strathmore.edu)
- **GitHub Issues**: [Submit an issue](https://github.com/LubangaD/kenyatradechatbot/issues)

