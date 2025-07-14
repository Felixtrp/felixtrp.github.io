---
layout: post
title:  "Perfect Heads Up Poker (Part 1)"
date:   2025-07-14 18:11:00 +0100
categories: posts
---

<h2>Poker - Luck or Skill?<\h2>

<p>
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

<\p>

<h2> The Simplest Possible Game </h2>



