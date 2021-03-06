# Misconceptions

This page collects and addresses misconceptions and common arguments against on-chain governance, coin voting and other Decred systems.

- [Coin voting is plutocracy](#coin-voting-is-plutocracy)
- [Ticket voting is not inclusive enough, tickets are expensive](#ticket-voting-is-not-inclusive-enough-tickets-are-expensive)
- [Coin holders cannot make good decisions](#coin-holders-cannot-make-good-decisions)
- [Voting on policies is inefficient compared to electing representatives](#voting-on-policies-is-inefficient-compared-to-electing-representatives)
- [Dev tax is bad](#dev-tax-is-bad)
- [The interests of coin holders and users are not aligned](#the-interests-of-coin-holders-and-users-are-not-aligned)
- [Votes can be bought](#votes-can-be-bought)
- [Coin voting governance can be added later](#coin-voting-governance-can-be-added-later)
- [Why doesn't Decred just use PoS alone and checkpoint into Bitcoin?](#why-doesnt-decred-just-use-pos-alone-and-checkpoint-into-bitcoin)
- [ASIC resistance, GPU-friendly algo is better](#asic-resistance-gpu-friendly-algo-is-better)
- [Decred is a fork of Bitcoin](#decred-is-a-fork-of-bitcoin)
- [Decred's launch or premine was not fair](#decreds-launch-or-premine-was-not-fair)
- [Decred's airdrop was not fair](#decreds-airdrop-was-not-fair)
- [Proof-of-Work uses too much energy, is bad for environment, etc](#proof-of-work-uses-too-much-energy-is-bad-for-environment-etc)
- [Decred gives passive income (returns, dividends, yield)](#decred-gives-passive-income-returns-dividends-yield)
- [Decred is based on Proof of Activity paper](#decred-is-based-on-proof-of-activity-paper)
- [Staking hurts market liquidity](#staking-hurts-market-liquidity)

## Coin voting is plutocracy
 
Counterarguments:

- Definition: ["plutocracy"](https://en.wikipedia.org/wiki/Plutocracy) has historically only been used to refer to the dominant power in a particular geographical location, the monarchy/empire/state.
- Voluntary: "plutocracy" is often used to mean non-voluntary (forced) participation, e.g. when you are born into a such society. You were not asked if you would like to participate. In public blockchains, on the other hand, no plutocracy happens to you until you voluntary join a given system.
- Switching cost: "plutocracy" is often used in context where the switching cost is high, i.e. it is hard to "opt-out" of the economic system adopted in your society. On the other hand, switching cost from one public blockchain to another is low (sell token A, buy token B). Low cost doesn't mean small losses due to price dynamics. It means it is low effort to perform the switch - to exchange tokens. Because blockchains are purely digital, switching between them does not require physical relocation, learning a new language, getting a new job, etc.
- Scope: the voting power you gain for having (more) DCR is limited to controlling how Decred works and how its Treasury is spent. Decred is not a full [society](https://en.wikipedia.org/wiki/Society) or nation state and it lacks many elements that could be subject to plutocracy: territory, military, police, healthcare, religion, etc. Decred's [mission](https://docs.decred.org/governance/decred-constitution/) is limited to building technology for the public benefit with a focus on cryptocurrency technology. Outside of Decred, the DCR currency can be used like any other form of wealth to pursue the ideas of plutocracy in full-blown societies.
- Strict rules: even if we imagine that DCR is adopted in some society and plutocracy is established, it will be a very different game because printing wealth out of thin air is not allowed.
- The concept of governance by the people who share a stake in a common enterprise is familiar from the governance of corporations, although it works in a different way in that context.

To summarize, plutocracy is a problem when you are born into it, it is hard to escape and it is hard to join a better society. In contrast, you choose whether to join a public blockchain and it is easy to leave it and join another one.

Discussion:

- https://medium.com/@richardred/what-is-on-chain-cryptocurrency-governance-is-it-plutocratic-bfb407ef6f1
- https://medium.com/mosaic-network-blog/is-plutocratic-on-chain-governance-really-a-bad-thing-68132700205c

## Ticket voting is not inclusive enough, tickets are expensive

First, "expensive" for what? The amount of power one gets for a ticket is substantial. Specifically, one ticket grants ~1/40,960th of the decision-making power. Tickets allow one to have a say in project's direction, voting on valid chain, consensus changes and budget decisions. This is not small. "Including" people with a few hundred bucks would be nice, but has lower priority than other tasks.

> How much say do you have about USD for a few grand? (@davecgh in [chat](https://matrix.to/#/!MgQoetFiyjrHAywokv:decred.org/$154949091135kyeGb:decred.org))

Second, there is wide agreement that lowering the barrier to entry is a good thing. It is just not top priority.

Third, since ~May 2018 it is already possible to purchase a fraction of a ticket as low as 5 DCR in a process called [Ticket Splitting](https://docs.decred.org/proof-of-stake/ticket-splitting/).

Fourth, several developers believe that the proper way to implement partial ticket purchases is not on-chain but off-chain via Lightning Network. A rough plan how to get there was [outlined](https://blog.decred.org/2019/11/11/LN-Multi-Owner-Tickets/) in Nov 2019.

## Coin holders cannot make good decisions

Decred decouples _sovereignty_ (decision making power) from _expertise_. Like all people, experts have their own agendas. To make better decisions, coin holders are incentivized consider experts' advice. But coin holders have the final say because they will be the ones to face _consequences_ of their decisions.

A few metaphors:

- Shareholders in a company hire experts, pay them and follow their advice, but still have the final say.
- When you are building or buying a house, you don't know everything and consult with experts. But you are the one choosing which experts to consult and what advice to follow, because you are the one who will live in the house.
- When choosing a car, you may have no expertise but you will use it (and risk your life).
- When visiting doctors, you use (and pay for) their expertise to learn about diseases and cure, but you will be the one to have consequences and you can choose which advice to follow. If the doctor prescribes wrong medicine or ignores the root cause, it will be _your_ problem.

> I've said it on multiple occasions, but I've always found the arguments of that nature to, in the most charitable light, be ill-informed, or, in the more realistic light, incredibly narcissistic in nature. When you cut right to the heart of it, it is effective saying "Only I, or some person of my choosing, is smart enough to make these kinds of decisions. The rest of you plebs need not apply". (@davecgh in #general)

Discussion:

- @jy-p on experts vs decision making power in Off the Chain podcast ([player.fm](https://player.fm/series/off-the-chain-2428336/jake-yocom-piatt-project-lead-for-decred-crypto-ego-management))

## Voting on policies is inefficient compared to electing representatives

- Delegating decision making power to elected representatives can indeed be more efficient. They can do it full time, they can be experts in relevant domains and they can know much more current information than an average voter. The problem is that their interests are often not aligned with interests of voters who will feel the consequences.
- Electing representatives was the only way for large groups to make collective decisions throughout most of the history. What has changed recently is the introduction of computers, the Internet, instant communication across any distance, and the development of consensus algorithms that allow multiple parties to agree on something without a central point of control. All this technology allows to create systems for collective decision making where the need of elected representatives is minimized or removed.
- Although it is rare, direct voting exists in nation state politics as [direct democracy](https://en.wikipedia.org/wiki/Direct_democracy) where people decide on policy initiatives directly. Switzerland is a notable example:

> Most western countries have representative systems. Switzerland is a rare example of a country with instruments of direct democracy (at the levels of the municipalities, cantons, and federal state). Citizens have more power than in a representative democracy. On any political level citizens can propose changes to the constitution (popular initiative), or ask for an optional referendum to be held on any law voted by the federal, cantonal parliament and/or municipal legislative body.

The price for having more power is it requires to pay more attention and actively participate:

> The list for mandatory or optional referendums on each political level are generally much longer in Switzerland than in any other country; for example any amendment to the constitution must automatically be voted on by the Swiss electorate and cantons, on cantonal/communal levels often any financial decision of a certain substantial amount decreed by legislative and/or executive bodies as well.
> 
> Swiss citizens vote regularly on any kind of issue on every political level, such as financial approvals of a school house or the building of a new street, or the change of the policy regarding sexual work, or on constitutional changes, or on the foreign policy of Switzerland, four times a year. Between January 1995 and June 2005, Swiss citizens voted 31 times, on 103 federal questions besides many more cantonal and municipal questions. During the same period, French citizens participated in only two referendums.

Decred has similar demand for attention and participation in return for much greater sovereignty the individual can get than in many competing cryptocurrency systems. During the [first year](https://blockcommons.red/publication/politeia-at-1/) of Decred's off-chain decision making platform (Politeia), 38 proposals have been voted on with an average turnout of 31% of eligible voting tickets (representing ~15% of the circulating DCR supply).

## Dev tax is bad

The 10% of [block rewards](https://docs.decred.org/advanced/issuance/) are going to the [Treasury](https://dcrdata.decred.org/address/Dcur2mcGjmENx4DhNqDctW5wJCVyT3Qeqkx?txntype=merged_debit).

- It is not "tax" because Decred is an opt-in system. Term ["tax"](https://en.wikipedia.org/wiki/Tax) refers to nation state law that uses force to make individuals pay and that is very hard to opt-out. If dilution from Decred Treasury is "tax", then emission of fiat currency is also "tax" but much worse because neither the emission nor distribution is voted on by holders of the currency (who are affected by the dilution).
- It is not "_dev_ tax" because the Treasury can also fund design, outreach, events, integrations, partnerships, and virtually anything that stakeholders approve.
- The alternative to having no common Treasury is to depend on altruism, venture capital and other external help that is unreliable and comes with its own interests.

## The interests of coin holders and users are not aligned

This used to be a commont argument from [Ethereum folks](https://medium.com/@Vlad_Zamfir/against-on-chain-governance-a4ceacd040ca), but somewhere in 2019 they pivoted to pitch ETH as [store of value](https://docs.ethhub.io/ethereum-basics/what-is-ether/#store-of-value) and this argument became less used. In case it will be made again in the future, Decred's approach is below.

To address the "users vs holders" we need to define who is the "user". In the case of "utility" tokens this argument can be true. For example, "users" of Ethereum blockchain willing to run smart contracts might have different interests from holders of ETH tokens. In case of "store of value" tokens the distinction between "users" and "holders" is less obvious and these groups have greater overlap than for "utility" tokens.

If coin holders are not given power because their interest are not aligned with users, some other group will have this power and not necessarily serve in users' best interests as well:

- developers' decisions might get steered by their investors or their desire to stay in power
- miners' decisions might get steered by their profits
- decisions of economic nodes like exchanges might get steered by their profits or their legal environments

Giving power to users themselves fixes the incentives but introduces the problem how to distribute that power. If there is no voting with main coin, other ways to assign power must be explored like auxiliary voting tokens, identity systems, user-based Proof-of-Work or something else. The challenge is to align incentives without making the system centralized, permissioned, or relying on external oracles.

## Votes can be bought

Votes can be bought in any voting system. You can't stop people from selling votes. In Decred, there are certain disincentives:

- Buying votes is more expensive than buying hashpower.
- Voters might lose in value of their locked coins if something bad is voted in.

Discussion:

- Murad's opinion on gaming voting outcomes in Decred in Depth podcast ([43:32](https://www.youtube.com/watch?v=XkvcdjSH0c0&t=43m32s))

## Coin voting governance can be added later

In theory it is possible. But it is hard to add coin voting if the system did not launch with it.

The challenges:

1. Will actors in power (miners or developers) give their power away to holders?
2. How will people coordinate and maximize participation during the transition?
3. Will enough people vote after the transition?

Transition to coin voting is a radical change to the governance model. For established projects it is essentially a transition of power from one group to another.

Existing direct holders of power either need to voluntarily give it up (e.g. miners approving blocks with new consensus rules where coin holders gain the voice, or developers shutting down their central "coordinator" server), or have their power forcibly revoked by groups with indirect power through a coordinated action (e.g. UASF-style move by a majority of economic nodes and users). The latter is sort of a revolt. Any change of governance model will meet resistance.

Second issue is coordination of upgrades. Decred community already has decent coordination tools and is building more. There is a process to [upgrade consensus](https://docs.decred.org/governance/consensus-rule-voting/overview/) and another to make [budget decisions](https://docs.decred.org/governance/politeia/overview/).

Finally, for coin voting to be strong it requires a substantial voter turnout. It takes time and many voting rounds to grow the culture where people care and participate. Decred community is constantly involved and keeps learning to make better decisions. Historical participation is above 50% for [consensus votes](https://docs.decred.org/governance/consensus-rule-voting/consensus-vote-archive/) and above 20% tickets (~10% coin supply) for budget and policy [decisions](https://explorer.dcrdata.org/proposals). A project looking to transfer power from miners to coin holders would need to (besides gaining miner support or pulling a revolt) engage many holders who didn't vote before, train them to participate and make them stay around for future votes. If people in power are willing to give it away but there are too few voters, the power will transition from one small group to another.

Discussion:

- https://www.reddit.com/r/decred/comments/cirkvr/decreds_governance_model/

## Why doesn't Decred just use PoS alone and checkpoint into Bitcoin?

That would mean Decred PoS layer follows whatever Bitcoin miners come up with. Having own PoW is necessary to have miners in check. (from [reddit](https://www.reddit.com/r/decred/comments/8o2h0q/andreas_talks_about_pos_and_pow_i_think_pos/))

## ASIC resistance, GPU-friendly algo is better

1. ASICs will appear sooner or later. It's a matter of time and financial incentive.
   - We have seen many examples throughout the history of cryptocurrencies: Litecoin's Scrypt, Ethereum's Dagger, Dash's X11, Zcash's Equihash, multiple Monero's past algorithms, etc - all started as "ASIC-resistant" but have seen ASICs developed for them that outperformed GPUs.
2. To "resist" ASICs the network needs to keep changing hashing algorithms. This is dangerous for network's security because it adds more complexity and more frequent changes to very sensitive code.
3. GPUs can mine a ton of other coins.
   - GPU owner is not incentivized to stay with certain network and work for its success.
   - GPU owner is not incentivized to not attack the network because he can easily switch to another after the attack.
   - There's a lot of GPU hashpower out there, and some of it can be easily rented to attack the network. To be safer, the network must be dominant in the GPU hashrate market.
4. Even if ASICs are never developed, if the coin gets big the _GPU manufacturers_ can rig the game by using next gen cards themselves before selling them on the market.

Reading:

- https://twitter.com/matt_odell/status/1067521417791582212
- https://blog.sia.tech/the-state-of-cryptocurrency-mining-538004a37f9b
- https://blog.sia.tech/fundamentals-of-proof-of-work-beaa68093d2b

## Decred is a fork of Bitcoin

Decred is not a fork of Bitcoin in any useful sense.

"Bitcoin fork" usually means Bitcoin Core codebase fork, Bitcoin chain fork, or new chain started from a snapshot of Bitcoin UTXO set. Decred is neither of that.

1. Decred is not a fork of Bitcoin Core codebase. It is not a low effort fork that only changes a few parameters or &lt;1% of the codebase. All code was written from scratch in a different programming language. Hundreds of thousands lines of code written from scratch since 2013 cost hundreds of thousands or even millions of USD.

2. Decred is not a fork of Bitcoin chain. Decred chain was started from scratch in Feb 2016.

3. Decred was not started from snapshot of Bitcoin UTXO set. Distribution of DCR was started with a 8% [premine](https://docs.decred.org/advanced/premine/) split 50%/50% between the developers (to compensate for past work) and open airdrop participants, and continued as 60%/30%/10% split between PoW miners, PoS voters and the Treasury.

Decred is a fork of [btcsuite](https://github.com/btcsuite) codebase, which is a from-scratch implementation of the Bitcoin protcol. Arguably it can be called a "fork of Bitcoin protocol" or a "fork of Bitcoin concept". But nobody means "fork" in that sense, so calling Decred "a fork of Bitcoin" is misleading and devalues thousands of high quality man hours put into building Decred.

It is worth noting that [lnd](https://github.com/lightningnetwork/lnd), one implementation of Lightning Network, is kind of a "fork" of btcsuite too. btcsuite saved lnd a lot of time and money, and thanks to it Bitcoin's LN is much more developed now than it would be without btcsuite.

Discussions:

- https://twitter.com/_Checkmatey_/status/1155901635257929728

## Decred's launch or premine was not fair

See [Premine](https://docs.decred.org/advanced/premine/) page for details.

> regarding the whole "fair launch"/premine scenario, I'm contuously amazed at the reasoning given. What is the supposed purpose of having a PoW-only launch? The reason given is that because it offers a "fair" distribution. This argument very quickly falls apart though if you spend just a tiny amount of time thinking about it. Fair for whom? Is it fair for the poor farmer who has never even heard of a GTX1080Ti? Is it fair if the people who launched it already have purpose-built hidden FPGAs and/or ASICs? Is it more fair that the Satoshi entity effectively premined _at least_ 1M BTC while an airdrop results in stronger decentralization out of the gate? etc
> 
> That is not to say that all premines are fair either, by any means, but the point is that things have to be examined individually and in context. The whole notion of one being more fair than the other in all cases is really not a defensible position. (@davecgh on [2019-02-03](https://matrix.to/#/!MgQoetFiyjrHAywokv:decred.org/$154915314826963wetJG:decred.org))

> even with pure PoW, how do we prove, with absolute certainty, that there wasn't a single actor with multiple GPU farms (or even throttled ASICs) that mined a lot of early coins? (@davecgh on [2019-01-06](https://matrix.to/#/!kdpEDksmOMNrlMqffD:decred.org/$15468080889396DbcMn:decred.org))

Discussion:

- https://twitter.com/NoahPierau/status/1086229612437356545
- https://twitter.com/NoahPierau/status/1086236361752039425
- https://twitter.com/NoahPierau/status/1103234103439171584
- Murad on Decred's premine ([57:07](https://www.youtube.com/watch?v=XkvcdjSH0c0&t=57m07s))

## Decred's airdrop was not fair

See [Airdrop](https://docs.decred.org/advanced/premine/#airdrop) page for details.

> Also, the airdrop gets some bad press because the team "chose" who received it, but a big part of that was to remove the "unfairness" of people cheating by trying to get multiple airdrops. There is a lot of unfairness in the stock IPO model where certain people get the ability to purchase at the IPO price, some can buy more than others, and others can't get anything at all. The airdrop was therefore more fair to the general public - it was just a light burden of proof that you had _something_ to do with technology/internet and _might_ be helpful to the project/community. (@snr01 on [2019-03-06](https://matrix.to/#/!MgQoetFiyjrHAywokv:decred.org/$155187615918225orXdP:decred.org))

> One of the downsides to transparency is that it also invites a lot of misinformation. (...) Another example is that Decred was completely transparent about its airdrop which resulted in it having one of the best Gini coefficients in the space while Bitcoin was effectively pre-mined to all hell in the early days by the Satoshi entity as detailed analysis has very strongly hinted at, but because it wasn't transparent, a ton of people attempt to act like it never happened. Anyway, the point is that transparency is great, but it's important to keep in mind that it also comes with a lot of negativity too. (@davecgh on [2019-08-10](https://matrix.to/#/!MIGqWXfLFBwhipPKYL:decred.org/$156545014313306LiRUf:decred.org))

## Proof-of-Work uses too much energy, is bad for environment, etc

Energy use of cryptocurrencies must be compared to energy use of systems they are competing with. Why would anyone compare energy use of Bitcoin to power drawn by Iceland? How is it a useful comparison? It must be compared to energy used by the banking system. Same for carbon footprint and other metrics.

> Operating expenses for the entire banking industry may be $700B a year https://www.macrotrends.net/stocks/charts/BAC/bank-of-america/operating-expenses ([duganist](https://twitter.com/duganist/status/1167770570022408194))

> Bank Of America annual operating expenses for 2018 were $76B, a 6.97% increase from 2017. Bank Of America operating expenses for the twelve months ending September 30, 2019 were $82.137B, a 11.58% increase year-over-year. ([macrotrends.net](https://www.macrotrends.net/stocks/charts/BAC/bank-of-america/operating-expenses))

> One of the downsides to transparency is that it also invites a lot of misinformation. For example, consider the entire elecricity argument against cryptocurrencies that gets bandied about. The only reason anyone is even able to act like it's an issue is because it's transaparent enough to be calculated to a reasonable degress of accuracy. Meanwhile, the completely opaque massive banking infrastructure, cost of designing, printing, destroying, and transporting bills, and many, many more aspects allows them to get a pass. (@davecgh on [2019-08-10](https://matrix.to/#/!MIGqWXfLFBwhipPKYL:decred.org/$156544995913303PxYaD:decred.org))

Research:

- https://medium.com/@danhedl/pow-is-efficient-aa3d442754d3
- https://cbeci.org/
- https://digiconomist.net/bitcoin-energy-consumption
- https://digiconomist.net/bitcoin-electronic-waste-monitor/
- https://phys.org/news/2018-08-energy-bitcoin.html

## Decred gives passive income (returns, dividends, yield)

Decred's voting reward is called "reward" for a reason. Its primary goal is to reward voters for locking coins and making decisions to advance the network. It is not fully "passive" - you have to do something and risk, and it is not "dividends".

## Decred is based on Proof of Activity paper

Decred is not _based on_ or _influenced by_ the [Proof-of-Activity](https://decred.org/research/bentov2014.pdf) paper.

This idea has likely originated from the first [announcement](https://blog.companyzero.com/2015/12/decred-rethink-digital-currency/) of Decred in 2015. It contained two statements about PoA:

> The project is a result of the theoretical proposals brought by proof-of-activity (PoA) and MC2 in 2013.

> This system is based on that of MC2, which is very similar to, but developed independently from, Proof-of-Activity (PoA) by Iddo Bentov, Charles Lee, Alex Mizrahi and Meni Rosenfeld.

Some people have likely incorrectly interpreted it.

> this was done more to give credit for proposing a system substantially similar to mc2's than to suggest PoA had a dominant role in the development of dcr (@jy-p on [2019-11-03](https://matrix.to/#/!kdpEDksmOMNrlMqffD:decred.org/$157280146131785QqYMu:decred.org))

A 2017 [tweet](https://twitter.com/SatoshiLite/status/825190721216933888) by Charlie Lee further enforced this myth.

Decred is based on [Memcoin2](https://decred.org/research/mackenzie2013.pdf) paper.

PoA's actual contributions to Decred:

- spurred the founders to hurry up getting Decred into production
- stakepool concept
- provide a clear method for estimating the costs for performing majority attacks against the consensus system

Reading:

- https://docs.decred.org/research/overview/
- https://matrix.to/#/!kdpEDksmOMNrlMqffD:decred.org/$154465703641757josZI:decred.org
- https://matrix.to/#/!kdpEDksmOMNrlMqffD:decred.org/$157280114531777HJBxJ:decred.org

## Staking hurts market liquidity

Background: DCR holders can lock their coins in the PoS system to gain decision making power and receive voting rewards. Such locked DCR become non-liquid (cannot move) for up to 142 days. This naturally limits the total amount of DCR that can move at any given moment. As of writing (March 2020), roughly half of the 11.2M mined coins is locked in PoS, which means that only 5.6M DCR is liquid (it's even less due to other factors that we ignore here).

Some people argue that the PoS system significantly hurts _exchange liquidity_ specifically, i.e. the amount of DCR that people are _willing_ to trade. Such DCR is held on exchanges and placed in the order books or is ready to go there once the market reaches some desired state. Other tradeable DCR is curated by OTC desks or is simply idle in the wallets waiting to be traded.

In other words, the argument is that the PoS system makes it harder to buy and sell DCR, which in turn makes DCR a less attractive asset for investors.

On the one hand:

- Staking is an extra incentive to not trade your DCR since it offers a risk-free DCR yield (about 7%/year as of writing, latest estimate is [here](https://dcrdata.decred.org/)). It is plausible that some people would trade or loan their DCR if there was no staking.
- If your DCR is locked and you suddenly need to trade it, you can't.

On the other hand:

- Staking is strictly opt-in. You can use fiat in trade or you can buy stock in a company and take part in governance. Same for DCR, you can trade it or you can buy tickets. Staking may pull some money away from exchanges, but if you want to trade your DCR nothing stops you from doing so (unless you have locked the coins, then you need to wait).
- It is not a binary choice between staking and trading. If there was no PoS system some would just hold and still not trade.
- The way DCR is locked in PoS can be compared to a loan market where it is not allowed to revoke the loan before the agreed upon date. Such loan market may develop in any cryptocurrency and also restrict liquidity.
- Staking yield [declines](https://docs.decred.org/advanced/issuance/) over time due to decreasing PoS rewards and increasing ticket price.
- Every block (5 minutes), on average 5 tickets worth of DCR are entering the PoS system, but also the same amount is exiting it. Should the DCR market price rise significantly, some holders will direct their unlocked DCR to the market instead of re-staking it. This will increase liquidity in response to demand.

Discussion:

- https://www.reddit.com/r/decred/comments/6r9yd8/competition_between_liquidity_and_participation/
- https://www.reddit.com/r/decred/comments/7tx4rm/pos_vs_liquidity_can_we_have_both/
