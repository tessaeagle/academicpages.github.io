---
title: "GPT-2 Tracery Twitterbot"
excerpt: "Development of a Twitterbot using the [Tracery](tracery.io) text generation and [bot creation](https://cheapbotsdonequick.com/) tool to post GPT-2 generated content<br><br><img src='/images/gpt.png'>"
collection: portfolio
---

## Background
This project uses GPT-2, an open-source language learning model, to learn on tweets downloaded from popular gamer Twitter accounts. We download and analyzed sentiment expression in tweets by popular gamers and within popular gaming hashtags. These tweets were analyzed for valence, saving positive examples. We then utilize [Tracery](http://tracery.io/), a tool built by Kate Compton to generate text using a generative grammar/JSON. Tracery expands text based on user-inputted nodes.

**Project Goal:** Train a GPT-2 model to learn gamer slang (gamer girls) and create a twitter bot with it combining with tweets generated through the Tracery grammer. 

### Sentiment Analysis
We downloaded tweets from three prominent gamer twitter accounts (Ninja, Pokimane, and LilyPichu). Using sentiment analysis, we analyzed tweets for emotional valence. We trained a recurrent neural network (RNN) classifier with 800,000 labeled tweets and used this model to separate positive and negative tweets. 

#### Positively Classified Tweets
<img src='/images/posSent.png'>

### Generating Tweets
Using a GPT-2 Model we learned on tweets from Game Twitter Personalities. We implemented our data within a pre-existing GPT-2 Google Colab model. First, we input a single-column csv containing our tweet data. We used a 124M “small” model and carried out 2000 steps, testing different temperatures and using .7 in our final model. The temperature controls for the level of randomness present in the output. Temperatures closer to 1 than 0 choose words with a lesser probability of occuring at that point (e.g., "Do you want to go paint a cheetah?": vs. "Do you want to go get ice cream?". This then output a .txt file containing 1000 computer-generated tweets at a time.

<img src='/images/gpt2.png'>

### Creating a Twitterbot
<img src='/images/tracery.png'>
We used Tracery to create a Twitterbot that was set to tweet every six hours. Tracery is a generative grammar that we used to create rules for our human-generated tweets. The origin component contains a rule and denotes how sentences start and their formatting. Rules contain symbols, from which a set of text used for generation is selected. We then tweeted using Tracery rules and human-generated tweets as well as GPT-2-generated tweets. Certain rules provided text from the GPT-2 tweets. We attempted to make our final Twitter profile appear more like a real gamer profile than a bot.
<br>
<img src='/images/magik.png'>

