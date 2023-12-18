# Smart Scalper SG

This code is a fully automated trading algorithm designed for trading the SBER symbol on the M5 timeframe. It uses impulse price changes and market depth to identify trading opportunities and execute buy or sell trades.

## Trading Parameters

- Symbol: SBER
- Timeframe: M5
- Lot Size: 0.1
- Stop Loss: 50 pips
- Take Profit: 100 pips

## Trading Algorithm

The trading algorithm is executed in the `OnTick` function. It starts by getting the current price of the symbol and calculating the price change since the previous tick. If the price change is positive, a buy trade is placed with a stop loss and take profit calculated based on the current price. If the price change is negative, a sell trade is placed with the corresponding stop loss and take profit levels.

Additionally, the algorithm checks the market depth using the `SymbolInfoBook` function. If the ask volume is higher than the bid volume, a buy trade is placed based on increased volumes. If the bid volume is higher than the ask volume, a sell trade is placed based on increased volumes.

## Program Execution

The program starts by enabling automated trading and setting the expert magic number. It subscribes to the specified symbol and timeframe. In the `OnStart` function, the trading algorithm is executed in a loop until the program is stopped. The algorithm is executed in the `OnTick` function, and then the program waits for the next tick using the `Sleep` function.

## Product Description

The Smart Scalper SG is a fully automated trading algorithm designed for trading the SBER symbol on the M5 timeframe. It utilizes impulse price changes and market depth to identify trading opportunities and execute buy or sell trades.

Key Features:
- Fully automated trading algorithm
- Designed for trading the SBER symbol on the M5 timeframe
- Uses impulse price changes and market depth to identify trading opportunities
- Adjustable lot size, stop loss, and take profit parameters

Please note that ForexRobotEasy is not the official developer of this product. We only provide sample code that can work as described in this product. For detailed reviews and trading results of this product, please visit [Forex Robot Easy - Smart Scalper SG](https://forexroboteasy.com/forex-robot-review/review-of-smart-scalper-sg-fully-automated-trading-algorithm-for-forts-futures-on-sberbank-and-gazprom-moscow-exchange/). To find the official developer of this product, please use MQL5.
