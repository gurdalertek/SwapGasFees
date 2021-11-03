## Screen 7: (Interface 2) Timeline Visualization under `Charts` Tab
1. The second main function of the SwapGasFees app is the display of various charts, under the `Charts` tab, to enable a deeper understanding of the Uniswap ecosystem.
2. The `Charts` tab implements a different interface than the earlier three tabs: There is a display (possibly with a legend) and two navigation buttons, namely `Previous Chart` and `Next Chart`. This interface design again is targeted to minimize the cognitive load on the user, allowing the user to digest the reported results one at a time.
3. The first screen has the `Previous Chart` button disabled, yet still in display, to provide a hint of what is to come.
4. The first screen of the `Charts` tab immediately provides the most important information, off the bat: _"What are the best times for swaps of top pairs?"_
5. The visualization shows time on the x axis and top pairs on the y axis (as rows). 
6. Each bar displays the favorable times for each swap pair. There has to be a consistent rule for all pairs, to identify the best times, such as _"Select the times where the price is at the lower 30% quartile"_.
7. While the presented visualization shows bars as a single color, each bar can potentially be drawn to allow a color spectrum.
8. Sample source code for implementing this visualization can be found as ["World timeline visualization"](https://observablehq.com/@tezzutezzu/world-history-timeline), under [ObservableHQ Gallery](https://observablehq.com/@d3/gallery). The JavaScript visualization library used is [D3.js](https://d3js.org).
![](../figures/SwapGasFees_Design_07.png)

[Screen 1](Screen01.md) | [Screen 2](Screen02.md) | [Screen 3](Screen03.md) | [Screen 4](Screen04.md) | [Screen 5](Screen05.md) | **[Screen 6](Screen06.md) | Screen 7 | [Screen 8](Screen08.md)** | [Screen 9](Screen09.md) | [Screen 10](Screen10.md) | [Screen 11](Screen11.md) 

[Main Article](../README.md) | [Complete Tutorial](../Tutorial.md) 
