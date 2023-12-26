# Nadaraya Watson Envelope LUX EA

This code represents the implementation of the Nadaraya Watson Envelope LUX EA trading robot. It is developed by the Forex Robot Easy Team and can be found on their website [forexroboteasy.com](https://forexroboteasy.com).

## Description

The Nadaraya Watson Envelope LUX EA is a trading robot that uses the Nadaraya Watson Envelope indicator to identify potential trading opportunities in the forex market. The indicator calculates upper and lower envelopes based on a specified period and price close. The robot opens sell trades when the current price is above the upper envelope and buy trades when the current price is below the lower envelope.

## How it Works

The code starts by including the necessary libraries, Trade.mqh and Envelopes.mqh. It then defines constant variables such as the symbol to trade (SYMBOL), lot size (LOT_SIZE), and magic number (MAGIC_NUMBER).

The global variables are initialized, including the CTrade object for trade operations and the CEnvelopes object for envelope calculations.

The OnTick function is defined to handle market movements. It retrieves the current price using SymbolInfoDouble and calculates the upper and lower envelope values using the iEnvelopes function from the CEnvelopes object.

If the current price is above the upper envelope, a sell trade is opened using the Sell function from the CTrade object. If the current price is below the lower envelope, a buy trade is opened using the Buy function.

The OnDeinit function is defined to clean up resources when the program is stopped. It closes any open trades and deinitializes the trade and envelopes objects.

The OnInit function is defined to initialize the trade and envelopes objects when the program starts.

The OnStart function is defined to subscribe to the market and set the magic number for the robot.

The OnCalculate function is the main entry point of the program. It calculates any necessary bars and returns the number of calculated bars.

## Product Description

The Nadaraya Watson Envelope LUX EA is an innovative forex trading robot that utilizes the Nadaraya Watson Envelope indicator to identify potential trading opportunities. It is developed by the Forex Robot Easy Team and can be found on their website [forexroboteasy.com](https://forexroboteasy.com).

This trading robot is designed to automatically open sell trades when the current price is above the upper envelope and buy trades when the current price is below the lower envelope. It uses the Envelopes.mqh library to calculate the envelope values and the Trade.mqh library to execute the trades.

Please note that ForexRobotEasy is not the official developer of this product. This code is provided as a sample that can work as described in the product. To find the official developer of this product, please refer to MQL5.

For detailed reviews and trading results of this product, please visit [forexroboteasy.com](https://forexroboteasy.com/forex-robot-review/nadaraya-watson-lux-ea-review-mql5s-innovative-forex-robot/).
