---
layout: post
title:  "Heads-Up Poker - Luck or Skill?"
subtitle:  "What chance would you have against a poker god?"
date:   2026-02-19 00:18:00 +0000
categories: math games poker computing
---

<h2> Luck and Skill </h2>

Chess is a game of skill.  No matter how many times I am in a room with Magnus Carlson, I will lose.  If someone was offering you 1000:1 odds on my victory in a single game, you should still bet on Magnus.

Poker is a game skill *AND* luck.  Placed heads-up against a top rated player in poker, there is a chance, greater than zero, that the cards fall the right way for an amateur challenger.  Someone who has never seen a game of poker in their life can go all-in, get called, and reveal pocket aces.  Chess this ain't.

So, here's an interesting question: precisely how much of poker is luck?  Is there a good way to get a sense of it?  If an amateur played a pro, how much of a chance would they stand?  Let's see what we can find out...


<h2> The Worst Poker Player You Know - Strategy Overview </h2>

What might you do if you were faced with a pro?  Presumably you want to minimise their advantage, while minimising the number of important strategic decisions you have to take (and presumably, mess up).  More decisions equals more wrong decisions.

Therefore, I propose the most annoying strategy one can dream up: goinh all-in every time.  Conveniently, since we want to do some analysis on this in a bit, it also helps a great deal with the math.

How does this strategy do against a pro making all the optimal decisions?  A quick search on the internet produces a trove of incorrect answers and I consider it my public duty to help clear this mess up a litte.  Let's approach this from the point-of-view of the pro and get some quick bounds on a solution.

<h3>Upper and Lower Bounds<h3>
To get an lower bound on the pro's win rate, all we have to do is propose any strategy, find its win rate and claim that.  The simplest possible strategy is to do exactly the same thing - call every time.  This is obviously a suboptimal strategy, but it's easy to see that this game is symmetric, and the win rate for the pro is 50%.

For an upper bound, we can also make a fairly straightforward estimate.  To do this, we imagine giving our pro a massive unfair advantage and seeing how they do.  For instance, consider the case where our pro is the luckiest player in the world - they get pocket aces on every hand.  Clearly, the only move here is to go all-in, just as before.  The win rate for the pro in this case is equal to the win rate of pocket aces against a random hand.  The magic number here is 84.93%.  Nice.

In summary, our optimal pro has a win rate, $w*$ that satisfies:

$$
0.50 <= w* <= 0.85
$$

Can we tighten the bounds on this solution?  Yes, but we're going to need a bit of a run-up...

<h2>Sidequest - Markov Chains and Terminating Probabilities</h2>
Here we ta;l about Markov chains.
