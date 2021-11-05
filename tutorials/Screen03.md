## Screen 3: (Interface 1) Visualizing Swap Fees for the Selected Pair
1. After the `Show Swap Fees` button is clicked, the app extracts data from a database populated apriori, and displays two visualizations. 
2. The first visualization, on the upper right, is the swap gas fee for the selected fee, `by Hour` of the day. 
3. In the `by Hour` visualization, there are four rows, corresponding to the swap fees for `today`, `yesterday`, `this week`, and `this month`.
4. The black rectangle with the thick border shows the current time of the day.
5. The legend on the right hand side displays the fees with respect to the color scale.
6. The important text are shown in bold, including the text for `today`, current time, and fees for the current time and benchmark time points. 
7. The second visualization is on the lower right hand side, displaying swap gas fees `by Day`. 
8. The `by Day` visualization again displays the gas fees, but based on day of the year and month, enabling benchmark with previous months of the same year and the similar days of the past year.
9. In both visualizations, the unrealized future time periods are shown as blank (white color).
10. Using the two visualizations, a user can visually grasp whether now is a good time to swap or not.
11. Sample source code for implementing the first visualization can be found as ["World History Timeline"](https://observablehq.com/@tezzutezzu/world-history-timeline). Sample source code for the second calendar visualization can be found as ["Calendar"](https://observablehq.com/@d3/calendar), both under the [ObservableHQ Gallery](https://observablehq.com/@d3/gallery). The JavaScript visualization library used is [D3.js](https://d3js.org).
![](../figures/SwapGasFees_Design_03.png)

[Screen 1](Screen01.md) | **[Screen 2](Screen02.md) | Screen 3 | [Screen 4](Screen04.md)** | [Screen 5](Screen05.md) | [Screen 6](Screen06.md) | [Screen 7](Screen07.md) | [Screen 8](Screen08.md) | [Screen 9](Screen09.md) | [Screen 10](Screen10.md) | [Screen 11](Screen11.md) 

[Main Article](../README.md) | [Complete Tutorial](../Tutorial.md) 
