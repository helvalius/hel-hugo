+++
title = "Bonn Coding Dojo July"
date = 2013-07-22
math = false
highlight = false
draft = false
tags = []
categories = []
preview = false
+++

## What is a Coding Dojo
A Coding Dojo is a developer meet-up in which they work together in a pre-selected small programming challenge. This is a great way for developers to improve their skills and it's a great activity to encourage learning between developers. Especially in our case, we wanted to have an environment where our students and developers working in companies can learn together and from each other.

During a Code Dojo we work in pairs, using Test-Driven-Development (aka Test-Driven-Design) and adhering to the Clean Code principles in order to solve a problem. These problems are referred to as coding katas as they are meant to be exercised repeatedly and offer learning as well as discussion opportunities. The focus is not on completing the kata in the time available, but rather doing the best that we can, and improving our practice of the above techniques in doing so.  

## The Bonn Coding Dojo
The first Bonn Coding Dojo meeting was on Thursday the 18th. Six people showed up, more than I expected for the first meet-up. The agenda was introduction, selection of a kata to work on and a retrospective at the end. After the introduction we selected the tennis game kata for the coding part.

## What is the Tennis Game Kata
The tennis kata is  a simplified tennis game adopted from Wii sports. A game consists only of a single set.
- A player can have points 0 (love), 15 (fifteen), 30 (thirty) or 40 (forty).
- If a player has 40 points and wins the ball she wins the game.
- If both have 40 it is a "deuce". If the game is in deuce, the player winning the next ball has "advantage" and a game ball. If the player with advantage wins the ball, she wins the game. If the other player wins they are back at deuce.

## Retrospective
In the end we had three different approaches with all three pairs using Java as implementation language. In between we swapped pairs twice. One group for example introduced a class to deal with counting the score. Another group translated a counter for representing the tennis points. Overall we had a lot of fun dealing with this kata and all agreed to to the same kata again in the next meeting.

Questions and ideas that came up in the retrospective:
- What about negative tests and invalid game states?
- Is the tennis game class doing too much? What about an immutable score object?
- Are the tennis game rules at a glance readable and recognizable from the source code?

## Personal Feedback for the next meet-up
This was the first Coding Dojo that I organized, overall I was satisfied with how it worked out, but as always one finds things in which one can improve. I wanted to swap three times, as we had three pairs, but missed taking a look at the time in between. Next time I would like to do the pair sessions with a pomodoro timer, this way all have the same amount of time and a reminder when to switch. Maybe even start at some point to say that we delete all code after a pomodoro so that we could start fresh.

Sometimes I had the impression that we spent too much time on design discussions in a pair when we should have spent the time to implement our ideas in code. The number one rule in a coding dojo: There is only code, and code doesn't exist without tests.

In the future I would like to create and show a basic set of slides in the beginning to remind everyone of the rules and give the meeting a formal frame. I came up with this after taking a look what great working Sleepyfox is doing for the London Coding Dojo. His slides can be seen on speakersdeck: https://speakerdeck.com/sleepyfox. This standard fits into the idea behind katas and would give all participants a well-known framework to work in. Furthermore, after looking at the slides from Sleepyfox, I realized that I still need a banner/logo for putting on the slides and the google+ group.

## Bonn Coding Dojo August
The next Coding Dojo is set for Thursday the 15th August, we will meet again to work on the Tennis Kata in the Römerstrasse 164, A121 at 18:30 till 20:30.  Ideas for a pub  that we can visit after the dojo welcome! :)  Maybe we move to the B-IT building in the Dahlmannstrasse 2  during August/September, as I'm working there in a university lab course fulltime during the time period.

All interested students or developers are welcome! I'll post the event in the Coding Dojo Bonn Google+ Community at the beginning of August.

If you can't make it, don't worry. The plan is to organize (based on interest) at least a dojo per month. The monthly meeting will be on the 3rd Thursday each month.

