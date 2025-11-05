# ai-assisted-stock-market-analyzer
A stock Market Analyzer with AI integration. It can take a stock type, and date range of interest, and analyzes the stock market for the period specified.

---
`Adedoyin Simeon Adeyemi` | [LinkedIn](https://www.linkedin.com/in/adedoyin-adeyemi-a7827b160/)

---

## Tools Used:

- Jupyter AI
- OpenAI API
- GPT4.1-mini
- Pandas (data analysis)
- yfinance (for relevant Stock data retrieval)
- Serper API (to extract stock market news data from the internet)
- Matplotlib (Stock trend plotting)

## Analysis Carried out:

- Downloaded relevant stock data for the given stock ticker of interest from internet to local storage using yfinance, given relevant ticker and period of interest.
- Carried out basic data exploration using descriptive statistics (pandas)
- Calculated total return in percentage
- Visualized closing trend for the given period (matplotlib), annotating, closing, low and peak prices and when.
- Loaded the Serper API key from the .env file
- Define a helper function to query Serper API, handling appropriate exceptions.
- Built the search queries using the peak and lowest dates
- Fetched and stored news snippets and metadata for peak and lowest dates
- Analyzed Signal volatility
    > - Calculated daily percentage changes
    > - Calculated volatility (standard deviation of daily returns) in percentage
    > - Analyzed daily percentage changes
    > - Analyzed 20-day rolling volatility (standard deviation)
    > - Identified volatility threshold and filtered for high volatility days
- Used OpenAI’s gpt-4.1-mini model to generate final report summary and insights.

## Analysis Results 

See [Generated results and visualizations here](outputs/results.md)

## Insights Generated (for AAPL ticker between 24/10/2024 - 23/10/2025):

    > Between October 24, 2024, and October 23, 2025, Apple Inc. (AAPL) delivered a total return of 12.61%, accompanied by a moderate overall volatility of 2.07%. The stock experienced its lowest point on April 8, 2025, closing at $172.00 amid broader market concerns over tariffs and rising investor anxiety. In the days surrounding this low, volatility peaked, with April 9 seeing an especially notable spike. Subsequently, AAPL recovered steadily to reach its peak price of $262.77 on October 21, 2025. This peak coincided with a market environment shaped by mixed earnings reports in the tech sector and cautious optimism as major indexes showed record-setting activity. On October 27, 2025, Apple traded near $265, reflecting its strong recovery and investor confidence despite sector headwinds. Overall, Apple demonstrated resilience and growth over the year amidst a fluctuating market landscape.
