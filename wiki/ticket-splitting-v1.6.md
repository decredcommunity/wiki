---
author: bee
updated_utc: 2021-03-16
---

# Ticket Splitting in v1.6

## What is the short status?

> We absolutely agree ticket splitting is worthwhile. Supporting it correctly moving forward is a lot of work that touches the entire stack, which is going to take some time. See this [blog post](https://blog.decred.org/2019/11/11/LN-Multi-Owner-Tickets/). Meanwhile you can still split tickets using the legacy tools, see [here](https://decredvoting.com/ticketsplitting).

Thanks to u/Inaccurate- for [writing](https://www.reddit.com/r/decred/comments/m547to/not_focusing_on_split_tickets_will_affect_us/gr1iruu/) it so well.

## Does it still work?

Yes, as of writing (March 2021) buying partial tickets is still possible.

## How do I split tickets now?

It is currently possible if the following conditions are met:

- Decrediton (GUI) or dcrwallet (command-line) must be of v1.5 series
- the VSP must be of "legacy" type
- the VSP must support ticket splitting

In other words, it will _not_ work with v1.6 software, and it will _not_ work with VSPs of the new "vspd" type.

You can get the latest v1.5.2 software [here](https://github.com/decred/decred-binaries/releases/tag/v1.5.2).

And then you need a compatible VSP. Three are known to support ticket splitting:

- [99split.com](https://99split.com/)
- [decredvoting.com](https://decredvoting.com/)
- [stake.decredbrasil.com](https://stake.decredbrasil.com/)

BUT you also need to join other people to buy a full ticket, you need _active sessions_ on that VSP. Of the three above, only decredvoting.com is having those recently. You can monitor all three on [this page](https://mainnet-split-tickets.matheusd.com/) (slightly outdated text).

This text intends to clarify most recent status but not copy the docs - see [this page](https://decredvoting.com/ticketsplitting) for a good entry point with all instructions linked, and then you can connect with other users in [@dcrtktsplit](https://t.me/dcrtktsplit) Telegram or [##ticketsplitting]({}) on Matrix.

Note: Here we only talk about _VSP staking_, because users who can [solo](https://docs.decred.org/advanced/solo-proof-of-stake-voting/) stake likely don't need ticket splitting.

## Can I downgrade from v1.6?

No. If you have upgraded to v1.6, the only way to use ticket splitting again is to install v1.5, re-download the blockchain and re-create the wallet from seed.

{ can multiple versions of Decrediton be installed on Windows and macOS via our recommended install paths? }

Decrediton relies on dcrd to handle the chain and dcrwallet to handle the wallet.

Release notes for [dcrd v1.6](https://github.com/decred/decred-binaries/releases/tag/v1.6.0#dcrd-v160) warn: once blockchain data is migrated to new version there is no going back without re-downloading it with v1.5

dcrwallet v1.6 also does a one-way migration of the wallet file and older versions will not work with it. { correct? }

## Will it break? When?

Yes. The software stack that currently supports ticket splitting will stop working around **May 7, 2021** when v1.5 will stop syncing.

{ what will happen to tickets bought too late, when is too late? }

## What is ticket splitting again?

Ticket splitting allows to buy a part of the ticket. At least 5 DCR is required to participate. Participants get:

- a _chance_ to cast a consensus vote, proportional to one's input (e.g. funding 60% of a ticket gives a 60% chance to vote with it)
- a _fraction_ of the voting reward, proportional to one's input
- Politeia voting rights are granted to the biggest contributor

See more in the [tutorials](https://decredvoting.com/ticketsplitting).

## Why does it not work with v1.6?

The split ticket buyer program "logs in" to dcrwallet in a certain way. This way has [changed](https://github.com/decred/dcrwallet/pull/1867) in dcrwallet v1.6 to improve security and support the new vspd model and possibly other features. A bunch of software talking to dcrwallet (Decrediton, politeiavoter, dcrtime, etc) was updated to this change but the split ticket buyer program [was not](https://github.com/matheusd/dcr-split-ticket-matcher/issues/77).

## Why does it not work with vspd?

The new accountless VSP model is very different from the "legacy" VSP model. It offers [huge benefits](https://blog.decred.org/2020/06/02/A-More-Private-Way-to-Stake/) like private staking and better UX, but existing ticket splitting software does not work with it.

A whole new matching protocol, client and server are [required](https://www.reddit.com/r/decred/comments/lj2her/og_ticket/gnj3zqq/) to work with vspd staking. Put simply, it requires a lot of work.

## Why don't you guys fix it?

There is strong indication that the demand for ticket splitting is not enought to justify pulling our scarce dev resources away from other important work.

Over almost 3 years 2,679 split tickets were purchased at an average rate of 81/month, meaning that roughly 0.2% of tickets are being split. Largest individual month had 127 split ticket purchases (2020-Mar).

In addition, we have this data [gathered](https://www.reddit.com/r/decred/comments/m547to/not_focusing_on_split_tickets_will_affect_us/gr0in3e/) from the blockchain:

- split ticket purchases by month [chart](https://pasteboard.co/JSJHHdY.png)
- split ticket purchases by the number of particpants [chart](https://pasteboard.co/JSJI0f0.png)

## But it was a scary "beta" and hard to use!

There is an argument that ticket splitting was not popular because it was too complex to be popular.

Maybe, but maybe not. @davecgh has [noted](https://www.reddit.com/r/decred/comments/m2o8y8/ticket_prices_too_high/gqr6h7s/):

> It's a fair point in theory, and one I would ordinarily agree with, but we have two very strong counterpoints that say otherwise. Namely, the pre-GUI privacy and the DEX.
> 
> Before privacy was in Decrediton, it already had very strong demand and usage despite it being quite challenging to use (significantly harder than ticket splitting, in fact). See the privacy participation on the dcrdata explorer to see what I mean. Notice that participation has indeed gone up when the barrier to entry was lowered with the introduction into the graphical wallet, but the demand and usage was very clearly there prior to its inclusion as well.
> 
> The other example is DEX which, despite being an MVP that is fairly challenging to install (also ever so slightly more difficult than the ticket splitting tools, but nowhere near as difficult as privacy was), has a boat load of usage.
> 
> So, I have to question why it would be that things that demonstrably have high demand and either were, or still presently are, more difficult to use still had/have super high usage while the same is somehow not true for ticket splitting. It seems to me that the reasonable conclusion is that demand is simply not strong enough for ticket splitting to motivate people to figure out the separate tools which is dissimilar to the other aforementioned cases.
> 
> I agree that making it super easy to use and available in the graphical wallet will induce demand, but that is not at all the same thing as there actually being a ton of pent up demand as these arguments are asserting.

## Ok enough analyzing, what can we do?

We have few devs and they are busy with what they believe is more important. New developers are free to pick up the task.

There are four things that can be done to go from where we are to where buying partial tickets is super smooth.

1. Patch the [splitting client](https://github.com/matheusd/dcr-split-ticket-matcher) to support the new authentication in dcrwallet v1.6. This is the lowest hanging fruit and should make splitting possible with v1.6 and the legacy VSP model.

2. Double check that [dcrstakepool](https://github.com/decred/dcrstakepool) (legacy VSP server) will continue functioning after the new consensus activates around May 7. It has been updated to v1.6 RC4 but we need to know if there will be any issues on the new consensus. I heard there might be an increased chance of missed tickets. { jholdstock karamble clarify }

3. Design a new splitting/matching protocol that will work with vspd staking and write client and server for it. This will give ticket splitting users some benefits of vspd staking.

4. Do it properly on Lightning as matheusd has outlined in the [blog](https://matheusd.com/post/ln-split-tickets-04-summary/) and the 4 linked technical articles. Splitting tickets off-chain could much faster and smoother than on-chain, plus all the supporting tech developed in the process will unlock a host of other cool stuff (e.g. crowdfunding).

## Extras

Discussions:

- https://www.reddit.com/r/decred/comments/lj2her/og_ticket/
- https://www.reddit.com/r/decred/comments/m2o8y8/ticket_prices_too_high/
- https://www.reddit.com/r/decred/comments/m3o5x8/has_anyone_done_ticket_splitting_any/
- https://www.reddit.com/r/decred/comments/m547to/not_focusing_on_split_tickets_will_affect_us/
