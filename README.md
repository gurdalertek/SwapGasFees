# SwapGasFees: Design of an Analytics Dashboard for Gas Fees on Uniswap 

**Gurdal Ertek**

This project proposes design of an analytics dashboard to interactively and dynamically display swap fees on [Uniswap](https://uniswap.org) and other analytics charts. 

The proposed SwapGasFees app is not implemented during the period of [UniCode Competition 2021](https://unicode.ethglobal.com/), due to lack of time and difficulties in finding team members. Yet, it outlines a blue print of how such a system can be implemented over an extended time period. In other words, the design provides a template, through which such a dashboard can be coded.

## Uniswap and Swap Fees

[Uniswap](https://uniswap.org) is the by far most popular decentralized exchange in the world, enabling swaps (exchanges) of many different tokens and coins on the Ethereum layer 1 blockchain network.

One of the fundamental issues in swaps is the "swap gas fee", which is in a way the fee paid to the blockchain network for evaluating and recording a swap transaction. The swap gas fees, or in short, swap fees, can change significantly over time, depending on the congestion of the Ethereum network, level of liquidity, trade volume, and many other factors. 

## Design Principles


## Data Extraction

The following libraries can be used for data extraction from Uniswap:

* Probably the most **important** link is the [Uniswap v3 contract maps](https://j1mmy.fi), which document the Pool Contract, Factory Contract, and Position Manager.
https://j1mmy.fi 

* [BitQuery](https://graphql.bitquery.io/ide) (to query data from blockchains)
https://graphql.bitquery.io/ide

* [Flipside Crypto](https://app.flipsidecrypto.com) (to query data from blockchains)
https://app.flipsidecrypto.com

* [GraphQL](https://medium.com/coinmonks/get-uniswap-data-using-the-graph-79d0c6f7b9f2) (to extract data from Uniswap)
https://medium.com/coinmonks/get-uniswap-data-using-the-graph-79d0c6f7b9f2

## UI Design 

This section describes the basic design of the user interface (UI) for the proposed SwapGasFees app. The detailed design and the details of how the app will work will be added as a separate tutorial later. 

There are two main screens/interfaces in the app:

- **Interface 1:** Analytics for gas fees for a selected swap pair  (under the `Swap`, `Pools`, and `Favorites` tabs) 
- **Interface 2:** Analytics for gas fees and Uniswap pools, in general (under the `Charts` tab)

Now let us look into both of these interfaces, and explain each.

- **Interface 1:** Swap Gas Fees

![](./figures/SwapGasFees_Design_03.png)

- ...
- ...

- **Interface 2:** Uniswap Analytics

![](./figures/SwapGasFees_Design_07.png)

- ...
- ...



## Visualizations


## Suggested Technology Stack

* For the **backend**, the above data extraction tools can be tested, and the one that provides the fastest and most reliable results can be selected.

* For the **frontend**, the easiest thing to do would be to fork the Uniswap front-end code and do modifications on that. 

* For **visualizations**, as mentioned earlier, the most suitable library is thought to be [D3.js](https://d3js.org/). The [D3 Visualization Gallery](https://observablehq.com/@d3/gallery) at [Observable HQ](https://observablehq.com/@d3/) provides source codes for all the essential charts, that can be used in the SwapGasFees app.



