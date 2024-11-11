# AE Bootcamp Capstone Project Proposal

## 1. Project Idea
   - **Overview**: Analyze stock market sentiment alongside real-time market data to gain insights into how news impacts stock performance.
   - **Problem Statement**: Investors and analysts need tools to understand the effects of news sentiment on stock trends for informed decisions.
   - **Project Scope**: Use Polygon’s market data and MarketAux's sentiment-tagged news data to model correlations between sentiment shifts and stock price changes.
   - **Target Audience / Stakeholders**: Traders, analysts, and investment managers looking to integrate sentiment data into decisions.

## 2. Tools and Technologies
   - **Data Collection**: Polygon API for real-time and historical stock data and MarketAux API for sentiment data.
   - **Data Transformation & Modeling**: ETL via dbt; Airflow for pipeline orchestration (using Astronomer).
   - **Data Storage**: Snowflake for efficient data handling.
   - **Visualization & Reporting**: Tableau for sentiment-stock price visualizations.
   - **Other Technologies**: Python (Pandas, SQL), potentially sentiment analysis libraries.

## 3. Conceptual Data Model
   - **Entities and Relationships**: Core entities include `Stocks`, `NewsArticles`, `Sentiments`, and `Prices`, linked through ticker symbols.
   - **Schema Diagram**: Show relationships where `Stocks` connect to `NewsArticles` via tickers, with `Sentiments` derived from articles.
   - **Data Flow**: Ingest data via APIs, transform, and store, then analyze and visualize.
   - **Example Queries**: E.g., average sentiment per ticker and impact of sentiment on price movement.

## 4. Project Milestones
   - **Milestones**:
      - **Part 1**: Data acquisition and API integrations.
      - **Part 2**: Data transformation, modeling, and storage setup.
      - **Part 3**: Visualization, reporting, and final adjustments.
   - **Expected Challenges**: Data quality, streaming data handling, API rate limits, and designing efficient ETL.

## 5. Success Criteria
   - **Key Metrics**: Sentiment-price correlation accuracy, processing efficiency, and dashboard usability.
   - **Outcomes**: A dashboard displaying real-time sentiment trends correlated with stock price changes, enabling actionable insights.
