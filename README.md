# Gold-Stocks-Mean-Reversion-Trading-Strategy
Implementing various trading strategies primarily centered around mean-reversion on the GDXJ with linear/non-linear, ALSTM and rules-based approaches. WIP

## Project Thesis:

The dominant narrative around gold stocks remains rooted in outdated assumptions. Investors — particularly institutions — have historically treated gold producers as a leveraged proxy for physical gold, but mostly for the purposes of hedging and diversification. As a result, most capital allocated to gold equities is passive, buy-and-hold, and arguably valuation-agnostic. But this line of thinking ignores the fundamental reality: these are companies, not commodities. Their prices are shaped not just by macro trends, but also by operating costs, hedging activity, firm-specific catalysts, and behavioral flows. Yet almost no one trades these stocks actively.

This project was born from the observation that gold stocks lag spot gold in performance, even during bullish gold cycles — an outcome that frustrates traditional gold bugs like Peter Schiff, who expect gold equities to outperform or atleast track with the metal during inflationary environments. They haven’t. But what if that disconnect isn’t a reason to stay away — what if it’s exactly an inefficiency that we can exploit?

Digging into the research, I made some fascinating observations: investor timing in gold ETFs has consistently underperformed even passive benchmarks by over 1.5% annually. ​Studies also show that gold mining stocks demonstrate a time-varying and non-linear sensitivity to spot gold — the so-called gold beta is not constant and has declined in recent years. More importantly, they behave differently under different interest rate regimes, with real interest rates being one of the most influential variables in determining returns on gold. Add to that the decline in hedging among miners and the rise of alternative inflation hedges like Bitcoin, and you have a structural shift in how gold stocks behave — a shift that most investors are ignoring.

So I asked: if the old logic no longer works, what does? This project explores whether active long/short trading strategies using ML models can capitalize on these mispricings. I backtested multiple ML and statistical models (Random Forest, Lasso, LightGBM, Linear Regression) across decades of gold equity data. Our strategies incorporate not just predicted return magnitude but also confidence weighting, volatility scaling, and filtering based on signal strength — with performance compared against benchmarks like GLD, GDX, and SPY. I am also working on implementing ALSTM and rules-based trading strategies.

The results so far show clear differences across models and regimes. Some models outperform benchmarks over longer windows but struggle post-2020 — a period marked by stimulus-driven macro shifts and strong spot gold performance that wasn’t mirrored in equities. This divergence reinforces our core thesis: gold equity pricing is no longer just a function of gold prices. By layering behavioral analysis, timing signals, and dynamic position sizing, I aim to construct trading strategies that outperform a long-term buy-and-hold approach with the GDXJ and GLD.

## Results

### Models Accuracy and Cross Validation:

![image](https://github.com/user-attachments/assets/33df6fc8-aeaf-4519-93e8-0c1155978a62)

![image](https://github.com/user-attachments/assets/1036cc4b-2c0a-48b2-aa5d-88dc263c57e0)

### Historical Backtest Results:

![image](https://github.com/user-attachments/assets/6e9f9db7-4e61-4be8-a54f-9340b853f9aa)



