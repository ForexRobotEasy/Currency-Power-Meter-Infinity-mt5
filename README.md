# Currency Power Meter Infinity MT5

This code is a sample implementation of the Currency Power Meter Infinity MT5 indicator. It calculates the strength of different currency pairs based on a specified period and price type. The indicator is developed by Forex Robot Easy Team and more information about this product can be found on their website [here](https://forexroboteasy.com/forex-robot-review/currency-power-meter-infinity-mt5-review-strength-analysis-for-traders/).

## Input Parameters

- **Period**: The period used for calculating currency strength. Default value is 14.
- **Price**: The price type used for calculations. Default value is PRICE_CLOSE.

## Variables

- **currencyStrength[]**: An array to store the calculated currency strength values.
- **currencyPairs[]**: An array to store the names of the currency pairs.

## Initialization

In the `OnInit()` function, the currency pair names are initialized in the `currencyPairs` array. The currency strength for each currency pair is then calculated using the `iCustom()` function.

## OnTick()

In the `OnTick()` function, it checks if the current chart is a currency pair chart using `ChartIsSymbol()`. If it is, it gets the index of the current currency pair using `ArrayIndex()` and checks if it is valid. If it is, it adds a line chart for the current currency pair using `ChartIndicatorAdd()`.

## OnChartEvent()

In the `OnChartEvent()` function, it checks if the event is related to a mouse click using `CHARTEVENT_CLICK`. If the click position is within the mobile panel area (0-100 for both parameters), it switches to the next currency pair using `ChartOpen()`.

Please note that ForexRobotEasy is not the official developer of this product. This code is only a sample implementation that can work as described in the product. To find the official developer of this product, please use MQL5.

For detailed reviews and trading results of this product, visit [here](https://forexroboteasy.com/forex-robot-review/currency-power-meter-infinity-mt5-review-strength-analysis-for-traders/).
