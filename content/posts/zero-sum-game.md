---
title: "Zero-Sum Game"
date: 2023-06-24T09:56:34+09:00
draft: false
---

I'm just tired of doing MEV. It used to be fun, but not anymore. 
MEV is a zero-sum game, or perhaps a negative-sum game. 
After I realized that, I stopped talking about MEV on SNS. Sorry, but this is how it works and I hate to do it.
Now, I don't care about MEV anymore.

<!--more-->

### MEV in 2020
![MEV in 2020](https://www.tamagawa.ac.jp/SISETU/kyouken/jomon/katsuo.JPG)

### MEV in 2023
![MEV in 2023](https://www.msc.org/images/default-source/msc-english/content-banner/content-page-body-images-912-x-513/fishing-methods-(content-page)/pelagic-or-midwater-trawl-illustration.jpg?sfvrsn=7de237f_6)


## When someone is making, someone is losing 
Here is an example where someone lost a lot of money(not sure how much) and a MEV bot made $939 in a single tx.

trigger tx: https://polygonscan.com/tx/0xb5876bbba8339d7a22c6ef0125ec54d293b530430569a6088da651e35927e2f4

backrun tx: https://polygonscan.com/tx/0x8b81de6a081a1321d9e5aa56b8c888afcc354ae66b37a0d0fe9781c1feada1cf

Maybe the person who created this opportunity didn't realized that this swap would have a huge negative price impact and he/she would lose a lot of money. 
MEV searchers love this kind of swaps and actaully they are keeping the price impact low by taking the other side of the trade.
So, it is good for the market, but is it sustainable?


## The more searchers, the less profit
This is pretty obvious when you do arbitrage with the a backrun strategy. 
Here is the real world example from Arbitrum:

trigger: https://arbiscan.io/tx/0xf655ab9e4f21121476abc0c8b26c382e042c9b8fb1b18638fef839962301e076

backrun: https://arbiscan.io/tx/0xbcf2e46c15110cb8ca020e227493e56e695b4501cebb5111e12c53d8d266ead0

You can find many backrun txs in [the next block](https://arbiscan.io/txs?block=104254484) of the trigger tx. Notice only the first and the second arbitrage tx successfully made the arbitrage trades, but the rest didn't.
This kind of thing is happening all the time on all chains. Many of the top bots are now very sophisticated that they can detect pretty much all arbitrage opportunities, and they always win the latency game.
Like the conventional HFT, the only way to win this game is to be faster than others. How to be faster than these bots?

If there are few MEV searchers on the market, there would be many opportunities and you can make a lot of profit with a small cost.
However, if there are many MEV searchers, there would be few opportunities and you have to be faster than others to make a profit.
And the cost is getting higher and higher. The gas price will increase due to the congestion caused by the MEV txs. You might need more CPU cores, need to pay more gas fee to get your tx included faster, or even need to run more nodes.


## Future of MEV
I sometimes hear some people saying that there are still a lot of opportunities on some less crowded and newly launched chains.
But they're all gonna be the same. The more people join, the less profit you can make.

As time goes by, I have seen the following things happen in the MEV space:
- more gas price
- more sophisticated bots
- more server cost
- (maybe) less volatility

And probably the trend will continue. 
It's only gonna be like the conventional finance. It's more about who has more money and resources.
I miss those days when people are doing MEV with a free alchemy API. It was just about programming skills.
Of course, when threre is a huge market valatility, there will be a lot of opportunities and MEV bots make a lot regardless of the quality.
But we won't see the Luna crash every month. I cannot rely on the market volatility to make a profit.


## How to make it to the positive-sum game?
I don't know. Maybe during the bull trend, it could a positive-sum game, but it's not sustainable.
