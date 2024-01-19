# WH Advanced Gartley Pattern MT5

This is a custom indicator for MetaTrader 5 (MT5) that identifies and plots Gartley patterns on the price chart. Gartley patterns are harmonic trading patterns that can provide potential entry and exit points in the market.

## Indicator Initialization

In the `OnInit()` function, the indicator buffers are initialized. Two buffers are used: `gartleyPatternBuffer` and `fibonacciBuffer`. The `gartleyPatternBuffer` is used to plot the Gartley pattern, while the `fibonacciBuffer` is used to plot the Fibonacci levels. The indicator style is set to draw arrows on the chart.

## Indicator Calculation

In the `OnCalculate()` function, the Gartley pattern is calculated based on the input price data. The function iterates over the available bars and checks if the given points form a Gartley pattern. If a Gartley pattern is detected, the `gartleyPatternBuffer` is updated with the third point of the pattern, and the `fibonacciBuffer` is cleared. If a Gartley pattern is not detected, the `gartleyPatternBuffer` is cleared, and the `fibonacciBuffer` is updated with the fourth point of the pattern.

## Gartley Pattern Detection

The `CheckGartleyPattern()` function is responsible for checking if the given points form a Gartley pattern. The specific logic for detecting Gartley patterns should be implemented in this function. Currently, the function returns false, indicating that no Gartley pattern is detected. Traders can customize this function to implement their own Gartley pattern detection logic.

## Product Description

This code provides a sample implementation of an advanced Gartley pattern indicator for MetaTrader 5 (MT5). The indicator identifies and plots Gartley patterns on the price chart, helping traders to spot potential trading opportunities.

Please note that Forex Robot Easy is not the official developer of this product. We are providing a sample code that can work as described in the product. To find the official developer of this product, please refer to MQL5.

For detailed reviews and trading results of this product, please visit [Forex Robot Easy - WH Advanced Gartley MT5 Unbiased Review and Results](https://forexroboteasy.com/forex-robot-review/wh-advanced-gartley-mt5-unbiased-review-and-results/).
