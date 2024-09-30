# Portfolio-Analysis

Project Report: Portfolio Optimization and Sensitivity Analysis

1. Introduction
In the realm of investment management, optimizing portfolios to achieve superior risk-adjusted returns is crucial. This project leverages Python programming and financial data from Yahoo Finance to conduct portfolio optimization and sensitivity analysis. The primary goal is to construct an optimized portfolio that maximizes the Sharpe ratio while evaluating the impact of varying market conditions on portfolio performance through sensitivity analysis.

2. Methodology

Data Collection and Preprocessing
Financial data for selected stocks was retrieved from Yahoo Finance using Python's yfinance library. Daily adjusted closing prices ('Adj Close') were collected for the period from January 1, 2020, to January 1, 2023. The data underwent preprocessing to handle missing values and ensure uniform data formats, preparing it for subsequent analysis.

Calculating Returns and Volatility
Using the cleaned data, daily returns for each stock were computed as the percentage change in adjusted closing prices. Mean annualized returns and annualized volatility (standard deviation of returns) were then calculated based on daily returns, adjusted for 252 trading days per year.

Portfolio Optimization
Portfolio optimization aimed to maximize the Sharpe ratio, a measure of risk-adjusted return. The optimization process employed the minimize function from the scipy.optimize module, applying constraints to ensure the sum of portfolio weights equaled one. The resulting optimal portfolio weights were determined to allocate investments effectively across the selected stocks.

Sensitivity Analysis
Sensitivity analysis was conducted to assess how variations in expected returns and volatility levels influenced portfolio performance. By systematically adjusting expected returns and volatility within predefined ranges, the analysis provided insights into the robustness of the optimized portfolio under different market conditions.

3. Data Analysis

•	Annualized Volatility: The annualized volatility was previously calculated from historical data and can be referenced from the annual_volatility variable.

•	Sharpe Ratio: To calculate the Sharpe ratio, use the formula:


Sharpe Ratio=Expected Annual Return−Risk-Free RateAnnualized Volatility\text {Sharpe Ratio} = \frac{\text{Expected Annual Return} - \text{Risk-Free Rate}}{\text{Annualized Volatility}}Sharpe Ratio=Annualized VolatilityExpected Annual Return−Risk-Free Rate
Incorporating a risk-free rate (such as the yield on government bonds) would provide a comprehensive assessment of risk-adjusted returns compared to alternative investments.

Comparative Analysis
Comparative analysis against individual stock performances and a baseline portfolio highlighted the superior risk-adjusted returns achieved through optimization. The optimized portfolio's performance metrics surpassed those of individual stocks and demonstrated effective diversification and allocation strategies.

4. Visualization
Visual representations included scatter plots illustrating annual returns vs. volatility for individual stocks, contour plots depicting ROI (%) from sensitivity analysis, and cumulative returns of the optimized portfolio over the analysis period. These visuals facilitated the interpretation of data insights and supported the findings presented in the analysis.

5. Conclusion
In conclusion, this project exemplified the application of Python programming for advanced portfolio management and risk assessment. By employing quantitative techniques and utilizing financial data, an optimized portfolio was constructed to maximize risk-adjusted returns. The sensitivity analysis underscored the importance of considering varying market conditions in portfolio decision-making, offering valuable insights for investment strategies.

6. Recommendations
Looking ahead, future research could explore more sophisticated optimization models or incorporate additional factors such as sector-specific risks or investor preferences into the portfolio construction process. The methodologies and findings from this project provide a solid foundation for enhancing investment practices and achieving better risk-adjusted returns in real-world scenarios.

7. References
•	Yahoo Finance for financial data retrieval.
•	Python libraries: Pandas, NumPy, Scipy, Matplotlib for data manipulation, analysis, optimization, and visualization.
Appendices
•	Code snippets used for data preprocessing, portfolio optimization, sensitivity analysis, and visualization.
•	Additional charts, tables, and detailed analysis supporting the project's findings.
![image](https://github.com/user-attachments/assets/c019b8b1-1d85-45aa-b876-265a63905fb1)
