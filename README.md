# PCA Analysis of Swap Rates (EUR ESTR)

The following notebook serves as a documentation for the PCA analysis on ESTR swap rates. For the purpose of PCA, only the time series of swap rates across different tenors (1-50Y) was used.

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
