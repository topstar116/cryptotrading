# cryptotrading
Real-time crypto price data with Macrometa
Macrometa is a Global Data Network that offers a decentralized, distributed database, stream processing engine and compute platform that runs across 175 global edge regions. Apps, APIs and web services written on Macrometa are automatically deployed globally and handle requests from the closest edge location relative to the request with local read-write latencies (i.e. very low latencies).

Macrometa offers a range of ready-made capabilities that enable an application like a crypto trading bot to be built quickly and easily. We will use the following features of Macrometa in this tutorial:

Macrometa's serverless, decentralized and geo distributed developer platform that provides a database, a stream engine and stream processor and a function/container runtime.
We will use the global document database for storing trade data and sharing all trade related metadata and state between the decentralized, stateless bots and components
We will use geo distributed streams for publishing real-time price data from each exchange. Each bot subscribes to the stream and makes a decision on whether to buy or sell

#Crypto trading strategy
lets use a simple trend trading strategy:

Buy → When current price crosses above 10 bar simple moving average
Sell → When current price crosses below 10 bar simple moving average
The trading bot will run this strategy with:

BTC/USD pair on Coinbase Pro exchange
BTC/EUR pair on Bitstamp exchange
BTC/JPY pair on BitFlyer exchange
Please note that the trading strategy is a hypothetical example and does not take into account slippage, spreads, position sizing, account balances etc. Feel free to enhance the strategy and let me know what the results look like. The code for this trading bot is open source.





