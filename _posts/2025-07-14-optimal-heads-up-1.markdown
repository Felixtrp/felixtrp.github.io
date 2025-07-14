---
layout: post
title:  "Perfect Heads Up Poker (Part 1)"
date:   2025-07-14 18:11:00 +0100
categories: posts
---

## Poker - Luck or Skill?
 
How much of winning at poker is skill, and how much is luck? 
I mean, really - players will tell you they are running numbers in their heads the whole time, calculating EVs and making sure they are making game-theory optimal decisions or whatever, but at some point we all know your opponent has been sitting on pocket aces and there's nothing you can do about it.
Is there some real way we can estimate how much of poker is luck and how much is skill?
It clearly isn't totally random like snakes and ladders, nor purely 'deterministic' - something like chess, for example.
The truth is, poker lies somewhere in between - but where, **exactly**?


I wanted a nice little metric for this luck vs skill 'vibe' I'm describing (where snakes and ladders scores 0.0 and chess is very close to 1.0) and I think I have a loose approximation to such a metric.
Consider attending the Chess World Championships - the final has just taken place, the champion is crowned and we havesuccessfully identified the best player in the world.  
Now, an amateur who has just learnt the game challenges the world champion and asks for a quick game.  
How do we think this will go?
I suspect most people would place their money on the new world champion - an amateur in this scenario has approximately 0% chance of winning.
In the amateur vs 'world champion' Snakes and Ladders battle, however, the newbie stands a much better chance of success - 50% in fact.


Armed with these two data points and our intuitions, let's define our 'skill' metric, $ S $:
$$
S = 2 \times ( 0.5 - P(\text{A trivial strategy wins against an optimal opponent}) )
$$


## Amateur Vs Pro - The Simplest Possible Game
Poker is really complicated and I want to get a nice answer, so we are going to have to make this as simple a game as possible.  I still want this to be a 'valid' poker game, but that means we are going to have some slightly odd rules for the set-up.

### The Game
We are playing Heads-Up - Texas Hold 'Em.  SB and BB are both equal to 1 unit - we will adjust stack sizes later to see how this impacts play.  Setting small blind equal to the big blind implifies calculations substantially

### The players
We are going to have two players in this ga,e - it's heads-up.

The first player is 'The Pro',  This player is perfectly logical, can read minds and has infinite computing power.  Kinda overpowered, but we're testing the limits here.

The second player is "The Shover". They weren't paying attentioin when the rules were explained to them.  They can't do math and they also forgot all words in the English language apart from "All" and "In".

This may seem a bit silly, but actually I like this case for a number of reasons.
1. This is probabily a reasonable strategy for a total noivce to play against a pro - it gives away no information about their hand (even if they could evaluate it accurately).
2. It's better than folding every hand.
3. It makes the pro's decisions much more straightforward (look at their own cards, then call or fold) which simplifies calculations massively.
4. Most of my friends play like this anyway.

Let's see how a game goes...

## Single Hands

## Optimal Strategy








