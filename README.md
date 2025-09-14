# MultiAI_Hedge_Fund_Manager 🤖🤖

Multi AI agents for analyzing and managing your hedge fund portfolio . 📈💼

⚠️ This is a proof of concept for an AI-powered hedge fund.  The goal of this project is to explore the use of AI to make trading decisions.  This project is for **educational** purposes only and is not intended for real trading or investment.

This system employs several agents working together:

1. Aswath Damodaran Agent - The Dean of Valuation, focuses on story, numbers, and disciplined valuation
2. Ben Graham Agent - The godfather of value investing, only buys hidden gems with a margin of safety
3. Bill Ackman Agent - An activist investor, takes bold positions and pushes for change
4. Cathie Wood Agent - The queen of growth investing, believes in the power of innovation and disruption
5. Charlie Munger Agent - Warren Buffett's partner, only buys wonderful businesses at fair prices
6. Michael Burry Agent - The Big Short contrarian who hunts for deep value
7. Mohnish Pabrai Agent - The Dhandho investor, who looks for doubles at low risk
8. Peter Lynch Agent - Practical investor who seeks "ten-baggers" in everyday businesses
9. Phil Fisher Agent - Meticulous growth investor who uses deep "scuttlebutt" research 
10. Rakesh Jhunjhunwala Agent - The Big Bull of India
11. Stanley Druckenmiller Agent - Macro legend who hunts for asymmetric opportunities with growth potential
12. Warren Buffett Agent - The oracle of Omaha, seeks wonderful companies at a fair price
13. Valuation Agent - Calculates the intrinsic value of a stock and generates trading signals
14. Sentiment Agent - Analyzes market sentiment and generates trading signals
15. Fundamentals Agent - Analyzes fundamental data and generates trading signals
16. Technicals Agent - Analyzes technical indicators and generates trading signals
17. Risk Manager - Calculates risk metrics and sets position limits
18. Portfolio Manager - Makes final trading decisions and generates orders


#### Application Workflow Chart

<img width="1042" alt="Application workflow chart" src="images\Screenshot 2025-09-14 154752.png" />

Note: the system does not actually make any trades.





### 🚀 Test / Use the Product ?

#### 1. Clone the Repository

```bash
git clone https://github.com/KaustubhHari234/MultiAI_Hedge_Fund_Manager.git
cd MultiAI_Hedge_Fund_Manager
```

#### 2. Set up API keys

Create a `.env` file for your API keys:
```bash
# Create .env file for your API keys (in the root directory)
cp .env.example .env
```

Open and edit the `.env` file to add your API keys:
```bash
# For running LLMs hosted by openai (gpt-4o, gpt-4o-mini, etc.)
OPENAI_API_KEY=your-openai-api-key

# For getting financial data to power the hedge fund
FINANCIAL_DATASETS_API_KEY=your-financial-datasets-api-key
```

**Important**: You must set at least one LLM API key (e.g. `OPENAI_API_KEY`, `GROQ_API_KEY`, `ANTHROPIC_API_KEY`, or `DEEPSEEK_API_KEY`) for the hedge fund to work. 

## 3. Install dependencies and run the application
1. Install Poetry (if not already installed):
```bash
pip install poetry
```

2. Install dependencies:
```bash
poetry install
```

#### Run the AI Hedge Fund
```bash
poetry run python src/main.py --ticker AAPL,MSFT,NVDA
```

You can also specify a `--ollama` flag to run the AI hedge fund using local LLMs.

```bash
poetry run python src/main.py --ticker AAPL,MSFT,NVDA --ollama
```

You can optionally specify the start and end dates to make decisions over a specific time period.

```bash
poetry run python src/main.py --ticker AAPL,MSFT,NVDA --start-date 2024-01-01 --end-date 2024-03-01
```

#### Run the Backtester
```bash
poetry run python src/backtester.py --ticker AAPL,MSFT,NVDA
```

**Example Output:**

##### Sample Run for a Ticker

<img width="941" alt="Screenshot 2025-01-06 at 5 47 52 PM" src="images\Screenshot 2025-09-14 000444.png" />

<img width="941" alt="Screenshot 2025-01-06 at 5 47 52 PM" src="images\Screenshot 2025-09-14 000551.png" />

<img width="941" alt="Screenshot 2025-01-06 at 5 47 52 PM" src="images\Screenshot 2025-09-14 000614.png" />

##### Sample Run for BackTester - from 30 days ago to today

<img width="941" alt="Screenshot 2025-01-06 at 5 47 52 PM" src="images\Screenshot 2025-09-13 235804.png" />

<img width="941" alt="Screenshot 2025-01-06 at 5 47 52 PM" src="images\Screenshot 2025-09-13 235825.png" />

<img width="941" alt="Screenshot 2025-01-06 at 5 47 52 PM" src="images\Screenshot 2025-09-13 235741.png" />



### 🖥️ Web Application

The new way to run the AI Hedge Fund is through our web application that provides a user-friendly interface. This is recommended for users who prefer visual interfaces over command line tools.

Currently, The Web Application 🌐 is under development.


## ⚠️ Disclaimer

This project is for **educational and research purposes only**.

- Not intended for real trading or investment
- No investment advice or guarantees provided
- Creator assumes no liability for financial losses
- Consult a financial advisor for investment decisions
- Past performance does not indicate future results

By using this software, you agree to use it solely for learning purposes.

## 👤 About & Contact

This is a personal project by [Hari Kaustubh]
Crafted with ❤️ by Hari Kaustubh. 
🎉🎉


## License

This project is licensed under the MIT License. 