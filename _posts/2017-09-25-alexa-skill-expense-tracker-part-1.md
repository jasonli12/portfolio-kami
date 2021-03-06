---
layout: post
title: Alexa Skill - Expense Tracker (Part 1)
---

My third Alexa skill will be an Expense Tracker. I can say with confidence that I am guilty of impulse buying *at times* and not good at tracking my expenses. Part of the reason is that it is difficult to make an effort to remember, at the end of each day, to go back and look at all your receipts and log what you bought or paid for that day.

So what's a better way? **Alexa!!!** The idea here is whenever you make a purchase or pay for something, once you get the receipt or the amount, you'll call "Alexa" and tell her what expense you made and she'll track all that  information in a database. As a start, I want my skill to be able to write new expenses to a database and read the information from the database.

***What Info Am I Tracking?***

1.Date of purchase or expense

2.Description of expense

3.Cost of expense

***Status of Skill Development***

So far I have the interaction model for the writing piece complete and I plan to continue working on just this part until I am satisfied that it works well. Then I will add the functionality to retrieve historical expense information. The biggest challenge thus far has been defining the slots or what information to track. Part of the reason is because Amazon has only a certain number of built-in slot types. For example, for *cost of expense*, because there is no slot type for amount or currency, I have to track the dollars and cents in two different *AMAZON.NUMBER* slots. The alternative would be to use a custom slot type for the *cost of expense* but that would require a significant amount of training and sample utterances for Alexa.

The next part of the adventure is writing the code that connects the information Alexa gathers and a database. Stay tuned!
