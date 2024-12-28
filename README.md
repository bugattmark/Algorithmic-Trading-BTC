# Live Algorithmic Trading BTC in Python 📈
## Automated BTC/USDT pair trading with a predefined strategy on Binance
<a href="url"><img src="https://github.com/bugattmark/Algorithmic-Trading-BTC/assets/76730347/879d0eba-4a3c-4e57-8e69-8d330edd7233" align="middle" height="274" width="500" ></a>
---
I started researching and working on this project in early 2022.
I deployed the project live in June 2022. The project is completed on March 22, 2023.

I automated the CDC Actionzone V2 Strategy with the BTC/USDT pair and deployed the strategy on Binance. The project is completed in python.
To fine-tune the strategy, I coded a historical backtester to test the strategy, given parameters on historical BTC/USDT data. The backtester is completed in python.

---

### 1. Trading automation:
I used the ccxt library to simplify the process of creating/deleting limit orders. Pandas, MatPlotlib libraries are used. Deployed on AWS EC2.
After studying long-term investment strategies, I chose a trading strategy called "CDC Actionzone" to trade the BTC/USDT pair in the market. I fetched live OHLCV(Open,High,Low,Close,Volume) data of the BTC/USDT pair. Using the OHLCV data, I calculated the values for the "CDC Actionzone" indicator. When the conditions are met (Moving average crossovers and closing price is below/above the long moving average) for creating/deleting orders, a request is sent to Binance via API to create or delete the order. I deployed the code on AWS EC2.
In the strategy, stop losses are used.

---

### 2. Backtesting:
I coded the backtesting program in python. Pandas, Matplotlib libraries are used.
I imported Historical Bitcoin OHLCV since 2020. I indexed through every candle since 2020 until 2023 and calculated indicator values with initially set parameters. If the indicator indicates buy/sell, the virtual portfolio is updated to replicate real-life trading. At the end, the profit is calculated, along with W/L ratio, Biggest loss, completed trades etc.

I used this backtesting program for both my personal trading and my algorithmic trading.

I took into account gas fees, spot trading fees, stop losses, market slippage and uncertainties. Using the parameters which return the highest profits, I automated that given strategy.

Example in action:
<br>
<br>
![image](https://github.com/bugattmark/Algorithmic-Trading-BTC/assets/76730347/0e206981-9509-4a39-bf5e-97b43f1b3c8b)


---

### Improvements that I will implement in later projects: <br>
- Optimisation algorithm for finding optimal strategy parameter values. <br>
- Deep Neural network for trading due to the very complex nature of markets <br>
- Record and document the step-by-step process of projects for evaluation. <br>

🎉🎉

![image](https://github.com/bugattmark/Algorithmic-Trading-BTC/assets/76730347/c64dcc1d-0959-4b49-875a-8071f007b43c)
