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

- The most **important** link is the [Uniswap v3 contract maps](https://j1mmy.fi), which document the Pool Contract, Factory Contract, and Position Manager.
https://j1mmy.fi 

- [BitQuery](https://graphql.bitquery.io/ide) (to query data from blockchains)
https://graphql.bitquery.io/ide

- [Flipside Crypto](https://app.flipsidecrypto.com) (to query data from blockchains)
https://app.flipsidecrypto.com

- [GraphQL](https://medium.com/coinmonks/get-uniswap-data-using-the-graph-79d0c6f7b9f2) (to extract data from Uniswap)
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

- VISUALIZATION FOR FIRST THREE TABS

-- D3 Visualization Gallery (JavaScript library for manipulating documents based on data)
https://observablehq.com/@d3/gallery

-- Calendar (for slides 2-6)
https://observablehq.com/@d3/calendar

-- Timeline (for slides 2-6) 
https://observablehq.com/@mbostock/the-impact-of-vaccines

- CHARTS TAB

-- Timeline (for slide 7) (to see which are the cheapest hours or the day/week for each swap pair, where pairs are the rows, color is the gas fee)
https://observablehq.com/@tezzutezzu/world-history-timeline

-- Bubble chart (for slide 8) (showing volumes of all pairs, or coins in pools, size is volume, color can be volume/liquidity, red color tones if above median)
https://observablehq.com/@d3/bubble-chart

-- Arc diagram (for slide 9) (to see the pairs in the pools, color shows the main coin, such as ETH, USDT, USDC, DAI)
https://observablehq.com/@d3/arc-diagram

-- Animated scatter plot (for slide 10) (to see changes in multiple dimensions, as an animation)
https://observablehq.com/@mbostock/the-wealth-health-of-nations

-- Chord diagram (for slide 11) (to see volume & liquidity changes in pools, and in coins)
https://observablehq.com/@d3/chord-diagram

- OTHER POSSIBLE CHARTS

-- Realtime Horizon Chart (scrolling data, where time is x axis, pair is y axis, and color is the gas fee)
https://observablehq.com/@d3/realtime-horizon-chart

-- Treemap (showing volumes of all pairs)
https://observablehq.com/@d3/treemap

-- Stacked Area Chart (to see changes in volume and liquidity, color is pair)
https://observablehq.com/@d3/streamgraph

-- Sankey Diagram (changes in volume of pairs, color shows pair)
https://observablehq.com/@d3/sankey


## Suggested Technology Stack

- For the **backend**, the above data extraction tools can be tested, and the one that provides the fastest and most reliable results can be selected.
- For the **frontend**, the easiest thing to do would be to fork the Uniswap front-end code and do modifications on that. 
- For **visualizations**, as mentioned earlier, the most suitable library is thought to be [D3.js](https://d3js.org/). The [D3 Visualization Gallery](https://observablehq.com/@d3/gallery) at [Observable HQ](https://observablehq.com/@d3/) provides source codes for all the essential charts, that can be used in the SwapGasFees app.



