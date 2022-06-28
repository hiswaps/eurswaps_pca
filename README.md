# PCA Analysis of Swap Rates (EUR ESTR)

The following notebook serves as a documentation for the PCA analysis on ESTR swap rates. For the purpose of PCA, only the time series of swap rates across different tenors (1-50Y) was used.

View the interactive notebook here: https://colab.research.google.com/drive/12Ux8dqAIqRHZ3IAzkmL7IeoXvNJh275n?usp=sharing 

For the development of the application, similar procedure was used with two datasets: EUR ESTR swap rates and EUR 6M EURIBOR swap rates

## Table of Contents

1. Importing External Libraries
2. Fetching Swap Rates From the CSV files
3. Calculating the Daily Swap Rate Change (in bps)
4. Computing the Covariance Matrix + PCA
5. Plotting the PCs across Tenors
6. Calculating the actual values of the Principal Components
7. Calculating the Expected Daily Change in Swap Rates (change implied by our PCA)
8. Calculating the PCA residuals and identifying Relative Value opportunities


## Sources/References:


### Textbooks & Research Papers

- Fixed Income Relative Value Analysis: A Practitioners Guide to the Theory, Tools, and Trades by Doug Huggins
- Introduction to Fixed Income Analytics: Relative Value Analysis, Risk Measures, and Valuation by Frank J. Fabozzi and Steven V. Mann
- Market Risk Analysis Volume-I: Quantitative Methods in Finance
- Credit Suisse Research: https://research-doc.credit-suisse.com/docView?language=ENG&format=PDF&source_id=csplusresearchcp&document_id=1001969281&serialid=EVplkK6oNi2Oum067aSBs%2Bp%2F04%2F3pgbDBc%2B1pGHrQ0U%3D&cspId=null
- Salomon Smith Barney FI Research: http://quantlabs.net/academy/download/free_quant_instituitional_books_/%5BSalomon%20Smith%20Barney%5D%20Principles%20of%20Principal%20Components%20-%20A%20Fresh%20Look%20at%20Risk,%20Hedging%20and%20Relative%20Value.pdf 
- https://www.moodysanalytics.com/-/media/whitepaper/2014/2014-29-08-PCA-for-Yield-Curve-Modelling.pdf


### Websites and Other Resources

- https://linanqiu.github.io/2015/12/03/pca-irs/
- https://www.clarusft.com/mechanics-and-definitions-of-spread-and-butterfly-swap-packages/
- https://towardsdatascience.com/principal-component-analysis-pca-explained-visually-with-zero-math-1cbf392b9e7d
- https://www.clarusft.com/principal-component-analysis-of-the-swap-curve-an-introduction/
- https://medium.com/@lextheoracle/decomposing-the-aud-swap-market-with-pca-ea272a0ba42
- https://towardsdatascience.com/decomposing-predicting-the-euro-yield-curve-b3ad1670fdbb
- https://asmquantmacro.com/2015/06/29/principal-component-analysis-part-ii/
