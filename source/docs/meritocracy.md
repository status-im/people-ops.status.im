---
id: meritocracy.md
title: Meritocracy
---

It's time to get the kudos flowing and the meritocracy up and running!

![](https://discuss.status.im/uploads/default/original/1X/4f5caf0fab2e2367843a3c9e78987dbfde8cdaa6.gif)

The Kudos DApp smart contract is still being audited, so we're starting small with a 100 SNT weekly allocation for each person to award to their chosen superstar(s).

### What problem are we trying to solve?

We currently don't have a consistent way to give recognition to other contributors, nor a way to have a transparent view on the contributors most recognised by our network. In the past, the Disco kudos bot in Slack served this function and helped people give spontaneous recognition, but that's been missing since October 2018.

### What's the proposal?

Kudos Rewards - an experiment with awarding kudos each week between Status contributors. Heavily inspired by Giveth's awesome RewardDAO [concept](https://wiki.giveth.io/dac/contributors-guide/), the idea is that contributors get a weekly allowance of SNT which they can distribute amongst other contributors as they see fit. The awarded totals can be withdrawn by contributors who have earned kudos (more on how that works later).

### Why

-   Giving kudos allows us to recognise everyone making impactful contributions in the network. We value everyone's contributions, and want to amplify achievements and give credit for all the great work going on
-   This concept replaces the Disco kudos bot, which was our last kudos system and was (overall) well-used and positively received
-   It's inclusive of the whole community, everyone participating (not just core contributors) can be rewarded with tokens
-   It helps build a leaderboard/meritocracy over time, reflecting contributor impact and social capital.

### How does it work?

-   V1 of this idea is smart contract based, and can be viewed [here]([https://github.com/status-im/meritocracy 14](https://github.com/status-im/meritocracy) (h/t [@jarradhope](https://discuss.status.im/u/jarradhope)) .
-   Weekly pings will be sent out by People Ops, directing everyone to access the DApp, view their allocated SNT, and award their tokens. You can award your tokens to any contributor(s) (core, occasional, anyone).
-   When giving out tokens, you can add praise along with your token reward so that the recipient knows what you're awarding the tokens for.
-   After a certain date, each weekly cycle will be closed out, and contributors will no longer be able to make awards in that cycle. Any unused tokens (i.e. those that were allocated to a person but were not awarded onwards) are burnt at the end of each week (they can't be carried forwards). No one is obliged to take part, and you can opt out from receiving tokens too if it's not your thing.
-   Once a contributor's allocation is reduced to 0 (either by awarding all their tokens onwards to other contributors, or having the remainder of their allocation burnt due to inactivity at the end of each week), they're able to withdraw (claim) their reward tokens.
-   The DApp shows each contributor's allocated, burnt, and awarded balances, i.e. participation stats, along with all the praise commentary they received.
-   Initially, core contributors will receive a flat weekly allocation. All contributors in the Statusphere can participate, by sending funds to the smart contract to signal participation. Contributed funds are allocated evenly across all contributors playing the game.
-   This basic first implementation can be iterated over time, e.g. this v1 will make use of admins to add contributors, manage weekly token calls etc., however in future as this evolves, admins can be phased out. The thinking is to start small with this idea and see how it works out.

### What are the criteria for awarding tokens?

The aim is not to be prescriptive about what actions merit recognition. In the same way as you awarded kudos for any number of reasons in the past, a Reward Kudos can be given out however you see fit. That might be to recognise e.g. Impact, Helpfulness, Collaboration, Contribution to Status and the wider ecosystem, Principles, Quality of output, etc.

### What is it not?

This is not a substitute for routine feedback-giving. We still think there's value in giving qualitative on-the-job feedback to other contributors. This is about recognising positive contributions, but constructive feedback should also ideally happen too elsewhere.

There is also a limitation to be recognised here in that this can only tell us about visible successes. Someone who works in a less visible role, or with a smaller imprint across the network, would naturally maybe not receive as many tokens as someone in another role. As such, this would not make kudos outcomes a reliable single source of truth on contributor impact.

To begin with, it's going to be a basic implementation to kick things off. We want to start strong with the ideal system in mind, so we'd love to hear your feedback on how you want to see this idea evolve.

### Why now?

This is something that's been on People Ops's radar for a few months time in various forms or another, but hasn't been a priority in recent months due to changes taking place. Now seems like a good time to re-initiate this discussion now that swarms are functional and Status is moving along smoothly.

What to do now...
---------------

Navigate to the DApp at [https://kudos.statusnet.eth](https://kudos.statusnet.eth/) - you'll be allocated an amount of SNT by each Friday

1.  Want to know who's participating? See the list [here](https://docs.google.com/spreadsheets/d/13uPS26GDh8V6el7f3vye1G6AtzeAGWrGxXXdBsCE9C4/edit#gid=130514777). Think of your Most Valuable Player(s) and send them some kudos to recognise their awesome work
2.  Search by typing their name in the `Choose Contributor` field
3.  Decide how many SNT you'd like to award them from your total allocatable kudos. Enter the number in the box
4.  Let them know why they're rocking it - leave a comment of praise
5.  Hit `Award` to make it rain! You have until end of the day on Thursday to award your tokens, they'll then be burnt if unused
6.  Check back in your DApp on Tuesday to see if you got any kudos (there are no notifications)
7.  Once you've allocated all your kudos, you can withdraw any kudos you were awarded into your wallet

![](https://discuss.status.im/uploads/default/original/1X/b3e92c31818a52161f99fdf87f2d0cbbfd0fed41.jpeg)

...and then?
----------

Eventually, there'll be a leaderboard format where you can see the contributors setting Status's world on fire (you!) 🔥

We'll keep allocating you SNT each Friday, and you can keep dishing them out. We'll send a reminder each time we allocate SNT, so you can remember to access the DApp and make your award(s).

Troubleshooting
---------------

Having issues with the DApp?

-   Make sure your DApp is connected to mainnet: Profile > Advanced > Network > "Mainnet with upstream RPC"
-   Check you're online - if you see a zero balance and can't select a contributor, there may be a connection issue.
-   De-select privacy mode if enabled: Profile > Settings > Browser privacy mode (toggle off)
-   Sometimes there is a loading delay. If you're seeing a zero balance, give it a couple of minutes to see if the balances update.

If you didn't sign up when the Dapp was in production, your address won't be on the contract's registry - ping [@rramos](https://discuss.status.im/u/rramos) /[@ceri](https://discuss.status.im/u/ceri) to be added. You may have to wait until the next award cycle to get some SNT to dish out.

Getting involved
----------------

We're looking for help to give the app a facelift and create a leaderboard UI - shout if you want to help buidl!

You can check out the swarm page with future plans [here](https://github.com/status-im/swarms/blob/master/ideas/324-meritocracy.md).

A massive caveat
----------------

This is just the start! We'll scale it from here, increasing the amount of allocatable SNT in circulation over time. Think of it as a meritocratic, peer-driven compensation element, open to all. This is very much a v1 and is an experimental idea - nothing in this proposal is set in stone, but we'd like to give it a go to see how it goes and see how valuable people find it for recognising others.

If you have any ideas/feedback on improving this concept, feel free to share them. We'd love to collaborate with anyone interested in rolling out this idea, so if this sounds interesting, feel free to get involved (we don't see this as a People Ops idea, giving recognition and rewards is something that benefits us all).

-- Let's do this!
