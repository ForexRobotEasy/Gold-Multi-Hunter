# Gold Multi Hunter

## Overview
Gold Multi Hunter is an expert advisor (EA) designed to automate multi-currency XAU trading. It is developed by Forex Robot Easy Team and more information about this product can be found on their website [here](http://forexroboteasy.com).

The EA uses external parameters, global variables, and various functions to perform its trading operations. It is specifically designed to trade during evening quiet time and filter market volatility.

## External Parameters
- StopLoss: Stop Loss value in points

## Global Variables
- ticket: Trade ticket number
- virtualProfit: Virtual profit

## Functions
- OnInit(): Expert initialization function
- OnDeinit(const int reason): Expert deinitialization function
- OnTick(): Expert start function
- IsEveningQuietTime(): Check if it is evening quiet time
- IsVolatilityFilterPassed(const string symbol): Check if market volatility filter is passed
- IsTradeOpen(const string symbol): Check if there is an open trade for the given symbol
- OpenTrade(const string symbol): Open a new trade
- CloseAllTrades(): Close all open trades
- MagicNumber(): Get magic number

## How it Works
1. The EA starts by initializing and checking if it is evening quiet time.
2. If it is evening quiet time, the EA loops through each currency pair.
3. It checks if the market volatility filter is passed for each symbol.
4. If there is no open trade for the current symbol, a new trade is opened.
5. The trade opening logic is implemented in the OpenTrade() function. It sets entry and exit points, stop loss, and tracks virtual profit. It also calculates trade size and position risk.
6. The trade is placed using the OrderSend() function.
7. The EA also includes functions to close all open trades and get the magic number.

## Product Description
### Gold Multi Hunter - Automated Multi-Currency XAU Trading
Gold Multi Hunter is an expert advisor (EA) developed by Forex Robot Easy Team for automated multi-currency XAU trading. This EA is specifically designed to trade during evening quiet time and filter market volatility.

Key Features:
- Automated trading: The EA executes trades based on predefined rules and conditions, eliminating the need for manual trading.
- Multi-currency trading: It can trade multiple currency pairs simultaneously, providing diversification and potential profit opportunities.
- Evening quiet time trading: The EA is optimized to trade during evening quiet time, taking advantage of potentially favorable market conditions.
- Market volatility filter: The EA applies a volatility filter to ensure trades are executed during suitable market conditions.
- Stop Loss: It includes a customizable Stop Loss value to manage risk and protect against excessive losses.

Please note that ForexRobotEasy is not the official developer of this product. We only provide a sample code that can work as described in this product. For detailed reviews and trading results of Gold Multi Hunter, please visit the official developer's website [here](https://forexroboteasy.com/forex-robot-review/gold-multi-hunter-review-automated-multi-currency-xau-trading/). To find the official developer of this product, please refer to MQL5.
