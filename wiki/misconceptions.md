# Misconceptions

{title candidates: Misconceptions, Rebuttals, Common criticism}

Misconceptions and common arguments against on-chain governance, coin voting and other aspects of Decred system.

## Coin voting is plutocracy
 
Counterarguments:

- Company shareholder governance is also plutocracy, but nobody complains about that.
- Voluntary: "plutocracy" is often used to mean non-voluntary (forced) participation, e.g. when you are born into a such society. You were not asked if you would like to participate. In public blockchains, on the opposite, no plutocracy happens to you until you voluntary join a given system.
- Switching cost: "plutocracy" is often used in context where the switching cost is high. On the opposite, switching from one public blockchain to another is low (sell token A, buy token B). Low cost doesn't mean small losses due to price dynamics. It means it is low effort to perform the switch - to exchange tokens.

Discussion:

- https://medium.com/@richardred/what-is-on-chain-cryptocurrency-governance-is-it-plutocratic-bfb407ef6f1
- https://medium.com/mosaic-network-blog/is-plutocratic-on-chain-governance-really-a-bad-thing-68132700205c

## Ticket voting is not inclusive enough, tickets are expensive

First, "expensive" for what? The amount of power one gets for a ticket is substantial. Ticket allows one to have a say in project's direction, voting on valid chain, consensus changes and budget decisions. This is not small. "Including" people with a few hundred bucks would be nice, but has lower priority than other things.

> How much say do you have about USD for a few grand? (@davecgh in [chat](https://matrix.to/#/!MgQoetFiyjrHAywokv:decred.org/$154949091135kyeGb:decred.org))

Second, there is wide agreement that lowering barrier to entry is a good thing. It is just not top priority.

Third, since ~May 2018 it is already possible to purchase a fraction of a ticket as low as 5 DCR. The process is documented in [Ticket Splitting](https://docs.decred.org/proof-of-stake/ticket-splitting/).

Fourth, several developers believe that the proper way to implement partial ticket purchases is not on-chain but off-chain via Lightning Network. A rough plan how to get there was [outlined](https://blog.decred.org/2019/11/11/LN-Multi-Owner-Tickets/) in Nov 2019.

## Coin holders cannot make good decisions

> I've said it on multiple occasions, but I've always found the arguments of that nature to, in the most charitable light, be ill-informed, or, in the more realistic light, incredibly narcissistic in nature. When you cut right to the heart of it, it is effective saying "Only I, or some person of my choosing, is smart enough to make these kinds of decisions. The rest of you plebs need not apply". (@davecgh in #general)

## Coin holder interests and user interest are not naturally aligned

[Source](https://medium.com/@Vlad_Zamfir/against-on-chain-governance-a4ceacd040ca). This requires defining "blockchain user". In case of "utility" tokens this argument can be true. For example, "users" of Ethereum blockchains willing to run smart contracts might have different interests from holders of ETH tokens. In case of "store of value" tokens the distinction between "users" and "holders" is less obvious and the sets have greater overlap than for "utility" tokens.

## Votes can be bought

- Buying votes in Decred is more expensive than buying hashpower.
- Votes can be bought in any voting system. You can't stop people from selling votes.

Discussion:

- Murad's opinion on gaming voting outcomes in Decred in Depth podcast ([43:32](https://www.youtube.com/watch?v=XkvcdjSH0c0&t=43m32s))

## Coin voting governance can be added later

It is hard to add coin voting if the system did not launch with it.

The challenges:

1. Will actors in power (miners or developers) give their power away?
2. How will people coordinate and maximize participation in the transition?
3. Will enough people vote after the transition?

Adding coin voting is more generally changing the governance model. For established projects it is essentially a transition of power from one group to another.

Existing direct holders of power either need to voluntarily give it up (e.g. miners approving blocks with new consensus rules where coin holders gain the voice, or developers shutting down their central "coordinator" server), or have their power forcibly revoked by groups with indirect power through a coordinated action (e.g. UASF-style move by a majority of economic nodes and users). The latter is kind of a revolt. In short, changing governance model will meet resistance. Posts against on-chain governance by Ethereum leaders with decision making power have demonstrated that it is easy for such projects.

Second issue is coordination. Decred community already has decent coordination tools and is building more. There is a process to [upgrade consensus](https://docs.decred.org/governance/consensus-rule-voting/overview/) and another to make [budget decisions](https://docs.decred.org/governance/politeia/overview/).

Finally, for coin voting to be strong it requires a substantial voter turnout. Decred community is constantly involved and keeps training to meke better decisions. Historical participation is above 50% for [consensus votes](https://docs.decred.org/governance/consensus-rule-voting/consensus-vote-archive/) and above 20% tickets (~10% coin supply) for budget and policy [decisions](https://explorer.dcrdata.org/proposals). A project looking to transfer power from miners to coin holders would need to (besides gaining miner support or pulling a revolt) engage many holders who didn't vote before, train them to participate and make them stay around for future votes.

Discussion:

- https://www.reddit.com/r/decred/comments/cirkvr/decreds_governance_model/

## Why doesn't Decred just use PoS only and checkpoint into Bitcoin?

That would mean Decred PoS layer follows whatever Bitcoin miners come up with. Having own PoW is necessary to have miners in check, and the only way to do it is to start the chain from scratch. (from [reddit](https://www.reddit.com/r/decred/comments/8o2h0q/andreas_talks_about_pos_and_pow_i_think_pos/))

## ASIC resistance, GPU-friendly algo is better

1. ASICs will appear sooner or later. It's a matter of time and financial incentive.
   - We have seen many examples throughout the history of cryptocurrencies: Litecoin's Scrypt, Ethereum's Dagger, Dash's X11, Zcash's Equihash, certain versions of Monero's algorithm, and several others - all started as "ASIC-resistant" but have seen ASICs developed for them that outperformed GPUs.
2. To "resist" ASICs you need to frequently change hashing algorithm. This is dangerous for network's security because it adds more complexity and more frequent changes to very sensitive code.
3. GPUs can mine a ton of other coins.
   - GPU owner is not incentivized to stay with certain network and work for its success.
   - GPU owner is not incentivized to not attack the network because he can easily switch to another after the attack.
   - There's a lot of GPU hashpower out there, and some of it can be easily rented to attack the network. To be safer, the network must be dominant in the GPU hashrate market.
4. Even if ASICs are never developed, if the coin gets big the GPU manufacturers can rig the game by using next gen cards themselves before selling them on the market.

Recommended:

- https://twitter.com/matt_odell/status/1067521417791582212
- https://blog.sia.tech/the-state-of-cryptocurrency-mining-538004a37f9b
- https://blog.sia.tech/fundamentals-of-proof-of-work-beaa68093d2b

## Decred is a fork of Bitcoin

Decred is not a fork of Bitcoin.

"Bitcoin fork" usually means Bitcoin Core codebase fork, Bitcoin chain fork, or new chain started from a snapshot of Bitcoin UTXO set. Decred is none of that.

1. Decred is not a fork of Bitcoin Core codebase. It is not a low effort fork that only changes a few parameters or &lt;1% of the codebase. All code was written from scratch in a different programming language. Hundreds of thousands lines of code written from scratch since 2013 would cost hundreds of thousands or even millions of USD.

2. Decred is not a fork of Bitcoin chain. Decred chain was started from scratch in Feb 2016.

3. Decred was not started from snapshot of Bitcoin UTXO set. The distribution started from a 8% premine split 50%/50% between developers and airdrop participants, and continued as 60%/30%/10% split between PoW miners, PoS voters and the Treasury.

Decred is a fork of btcsuite codebase, which is a from-scratch implementation of the Bitcoin protcol. So it can be arguably called a fork of Bitcoin protocol or Bitcoin concept. But nobody reads or says "fork" in that sense, so calling Decred "a fork of Bitcoin" undervalues thousands of high quality man hours put into building Decred.

lnd, one implementation of Lightning Network, is kind of a "fork" of btcsuite too. It saved lnd a lot of time and money, and thanks to it Bitcoin's Lightning Network is much more developed now than it would be without btcsuite.

Discussions:

- https://twitter.com/_Checkmatey_/status/1155901635257929728

## Decred's launch or premine was not fair

Docs page: [Premine](https://docs.decred.org/advanced/premine/).

> regarding the whole "fair launch"/premine scenario, I'm contuously amazed at the reasoning given. What is the supposed purpose of having a PoW-only launch? The reason given is that because it offers a "fair" distribution. This argument very quickly falls apart though if you spend just a tiny amount of time thinking about it. Fair for whom? Is it fair for the poor farmer who has never even heard of a GTX1080Ti? Is it fair if the people who launched it already have purpose-built hidden FPGAs and/or ASICs? Is it more fair that the Satoshi entity effectively premined _at least_ 1M BTC while an airdrop results in stronger decentralization out of the gate? etc
> 
> That is not to say that all premines are fair either, by any means, but the point is that things have to be examined individually and in context. The whole notion of one being more fair than the other in all cases is really not a defensible position. (@davecgh on [2019-02-03](https://matrix.to/#/!MgQoetFiyjrHAywokv:decred.org/$154915314826963wetJG:decred.org))

> even with pure PoW, how do we prove, with absolute certainty, that there wasn't a single actor with multiple GPU farms (or even throttled ASICs) that mined a lot of early coins? (@davecgh on [2019-01-06](https://matrix.to/#/!kdpEDksmOMNrlMqffD:decred.org/$15468080889396DbcMn:decred.org))

Discussion:

- https://twitter.com/NoahPierau/status/1086229612437356545
- https://twitter.com/NoahPierau/status/1086236361752039425
- https://twitter.com/NoahPierau/status/1103234103439171584
- Murad on Decred premine ([57:07](https://www.youtube.com/watch?v=XkvcdjSH0c0&t=57m07s))

## Decred's airdrop was not fair

Docs page: [Airdrop](https://docs.decred.org/advanced/premine/#airdrop).

> Also, the airdrop gets some bad press because the team “chose” who received it, but a big part of that was to remove the “unfairness” of people cheating by trying to get multiple airdrops. There is a lot of unfairness in the stock IPO model where certain people get the ability to purchase at the IPO price, some can buy more than others, and others can’t get anything at all. The airdrop was therefore more fair to the general public - it was just a light burden of proof that you had _something_ to do with technology/internet and _might_ be helpful to the project/community. (@snr01 on [2019-03-06](https://matrix.to/#/!MgQoetFiyjrHAywokv:decred.org/$155187615918225orXdP:decred.org))

> One of the downsides to transparency is that it also invites a lot of misinformation. (...) Another example is that Decred was completely transparent about its airdrop which resulted in it having one of the best Gini coefficients in the space while Bitcoin was effectively pre-mined to all hell in the early days by the Satoshi entity as detailed analysis has very strongly hinted at, but because it wasn't transparent, a ton of people attempt to act like it never happened. Anyway, the point is that transparency is great, but it's important to keep in mind that it also comes with a lot of negativity too. (@davecgh on [2019-08-10](https://matrix.to/#/!MIGqWXfLFBwhipPKYL:decred.org/$156545014313306LiRUf:decred.org))

## PoW uses too much energy, is bad for environment, etc

Energy use of cryptocurrencies must be compared to energy use of systems they are competing with. Why would you compare energy use of Bitcoin to power drawn by X households or Iceland, and not to energy use of the banking system? Same for carbon footprint and other metrics.

> Operating expenses for the entire banking industry may be $700B a year https://www.macrotrends.net/stocks/charts/BAC/bank-of-america/operating-expenses ([duganist](https://twitter.com/duganist/status/1167770570022408194))

> Bank Of America annual operating expenses for 2018 were $76B, a 6.97% increase from 2017. Bank Of America operating expenses for the twelve months ending September 30, 2019 were $82.137B, a 11.58% increase year-over-year. ([macrotrends.net](https://www.macrotrends.net/stocks/charts/BAC/bank-of-america/operating-expenses))

> One of the downsides to transparency is that it also invites a lot of misinformation. For example, consider the entire elecricity argument against cryptocurrencies that gets bandied about. The only reason anyone is even able to act like it's an issue is because it's transaparent enough to be calculated to a reasonable degress of accuracy. Meanwhile, the completely opaque massive banking infrastructure, cost of designing, printing, destroying, and transporting bills, and many, many more aspects allows them to get a pass. (@davecgh on [2019-08-10](https://matrix.to/#/!MIGqWXfLFBwhipPKYL:decred.org/$156544995913303PxYaD:decred.org))

Research:

- https://medium.com/@danhedl/pow-is-efficient-aa3d442754d3
- https://cbeci.org/
- https://digiconomist.net/bitcoin-energy-consumption
- https://digiconomist.net/bitcoin-electronic-waste-monitor/
- https://phys.org/news/2018-08-energy-bitcoin.html

## Decred gives passive income / returns / dividends / yield

Decred's voting reward is called "reward" for a reason. Its primary goal is to reward voters for locking coins and making decisions to advance the network. It is not fully "passive" - you have to do something and risk, and it is not "dividends".

## Decred is based on Proof of Activity paper

Decred is not _based on_ or _influenced by_ the [Proof-of-Activity](https://decred.org/research/bentov2014.pdf) paper.

This idea has likely originated from the first [announcement](https://blog.companyzero.com/2015/12/decred-rethink-digital-currency/) of Decred in 2015. It contained two statements about PoA:

> The project is a result of the theoretical proposals brought by proof-of-activity (PoA) and MC2 in 2013.

> This system is based on that of MC2, which is very similar to, but developed independently from, Proof-of-Activity (PoA) by Iddo Bentov, Charles Lee, Alex Mizrahi and Meni Rosenfeld.

Some people have likely incorrectly interpreted it.

> this was done more to give credit for proposing a system substantially similar to mc2's than to suggest PoA had a dominant role in the development of dcr (@jy-p on [2019-11-03](https://matrix.to/#/!kdpEDksmOMNrlMqffD:decred.org/$157280146131785QqYMu:decred.org))

A 2017 [tweet](https://twitter.com/SatoshiLite/status/825190721216933888) by Charlie Lee further supported the idea.

Decred is based on [Memcoin2](https://decred.org/research/mackenzie2013.pdf) paper.

PoA's contribution to Decred:

- spurred the founders to hurry up getting Decred into production
- stakepool concept
- provide a clear method for estimating the costs for performing majority attacks against the consensus system

Reading:

- https://docs.decred.org/research/overview/
- https://matrix.to/#/!kdpEDksmOMNrlMqffD:decred.org/$154465703641757josZI:decred.org
- https://matrix.to/#/!kdpEDksmOMNrlMqffD:decred.org/$157280114531777HJBxJ:decred.org
