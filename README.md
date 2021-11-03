# Design of SwapGasFees: an Analytics Dashboard for Gas Fees on Uniswap 

**Gurdal Ertek**

This project proposes design of an analytics dashboard to interactively and dynamically display swap fees and other analytical charts.

## Uniswap and Swap Fees

Uniswap is the by far most popular decentralized exchange in the world, enabling swaps (exchanges) of many different tokens and coins on the Ethereum layer 1 blockchain network.

One of the fundamental issues in swaps is the "swap gas fee", which is in a way the fee paid to the blockchain network for evaluating and recording a swap transaction. The swap gas fees, or in short, swap fees, can change significantly over time, depending on the congestion of the Ethereum network, level of liquidity, trade volume, and many other factors. 

## Design Principles


## Data Extraction

The following libraries can be used for data extraction from Uniswap:

* VERY IMPORTANT: Uniswap v3 contract maps (Pool Contract, Factory Contract, Position Manager)
https://j1mmy.fi 

* BitQuery (to query data from blockchains)
https://graphql.bitquery.io/ide

* Flipside Crypto (to query data from blockchains)
https://app.flipsidecrypto.com

* GraphQL (to extract data from Uniswap)
https://medium.com/coinmonks/get-uniswap-data-using-the-graph-79d0c6f7b9f2

## UI Design 


## Visualizations
