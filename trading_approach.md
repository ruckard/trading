These are the different approaches that I have made to trading.

# Gekko - Very early approach
[Gekko](https://gekko.wizb.it/) was a Bitcoin TA trading and backtesting platform. Its source code can be found in [Gekko Github repo](https://github.com/askmike/gekko/). It is currently [discontinued](https://medium.com/@gekkoplus/archiving-open-source-gekko-dba02e6efc7).

This Bitcoin BOT was based on Nodejs which I don't like too much (I'm more of a python guy). It worked but it was very hard to find a working strategy.
:Two important bits about this approach

  * The bot was designed in such a way that each time you decided a trade it put all of your 100% balance into it. Either you were 100% invested on BTC or you were 100% invested on USDT. Later on I discovered money management and thus I concluded that this was a flawed design. Back in the day I wasn't aware of it.
  * I did some backtesting and I was not very successful on getting good results. One thing I remember is deciding to use either 5m or 15m timeframe because this was not human based but computer based. So... If I was going to use a bot, I was going to win plenty of money and that should only happen with the smallest timeframes. Later on I learned that timeframes under 4 hours are mostly noise. It's rather more intelligent (on average) to work on 4h, 1d or 1w timeframes.

So the conclusions we can draw from this very early approach are two:

  * Despite a tool naming itself as a bot it doesn't mean it is well setup for its first usage (Putting 100% balance on each trade).
  * You cannot just a tool without knowing beforehand which strategy you want to use and which it's the most suitable timeframe for that strategy.

# TradingLatino - Copying a Youtuber strategy and discovering TradingView

## TradingLatino Broadcast

Jaime Merino is a trader from San Salvador country. He broadcasts his trading advice on his [TradingLatino Youtube channel](https://www.youtube.com/channel/UCLjSq1FapG5OgvHsDKinHdA). He also hosts a related webpage named [tradinlatino.net](https://tradinglatino.net/).

There are two special bits about his broadcasting. First of all he shares his bits of his strategy every day. Secondly you can check each day if his last day prediction was right or not because he usually repeats parts of his previous days with his predictions.

He claims that his strategy yields positive results 6 o 7 times of 10 times.

## TradingView discovery

Jaime uses [TradingView](https://tradingview.com/) webpage to make his predictions. He uses several indicators which you can replicate. So I opened a free TradingView account and tried to use his same indicators to see if I could replicated his setup. This turned out to be a difficult task because a free TradingView account has a limited set of indicators and some of the official TradingView indicators (as Volume Profile) are not available unless you have a paid account.

TradingView has a built-in scripting language that lets you to write your own indicators and strategies. So I managed to write replacements for the TradingView paid accounts only indicators. I also started to replicate TradingLatino strategy so that I could use the backtesting tool from TradingView to know if it was worth of using it or not.

I haven't fully replicated the TradingLatino strategy so I cannot answer that question yet.

Please check my [TradingView indicators and strategies page](tradingview-indicators.md) for more information about it.