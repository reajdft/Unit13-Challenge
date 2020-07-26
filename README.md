
# Cryptocurrency Market Analysis via PCA & K Means Clustering
## Project Summary & Notes:
**Data Source** - CryptoCompare using this endpoint: https://min-api.cryptocompare.com/data/all/coinlist

**Purpose:**
To provide a summary overview of currently tradeable cryptocurrencies, grouped by K Means to understand shared traits across over the 500 cryptos currently traded
* Notebook contents: 
* 1. Pre-processing/cleaning/standardizing
* 2. PCA development
* 3. K Means Clustering
* 4. Summary stats and visualization

## Pre-processing/cleaning/standardizing:
* The source data in the accompanying CSV file removed stale cryptos & and those with zero coins mined to filter down to active cryptos. 
* The crypto's Algorithm type and ProofType contained in the raw data were then converted to dummies, with the entire feature set scaled using SKLearn's Standard Scaler function

### PCAs:
* The feature set was reduced from 100 to 3

### K-Means:
* Clustering the 3 principal components yielded and optimal cluster grouping of 4 (see Elbow Curve in attached notebook)

### Tables & Visuals:
* See notebook for visuals