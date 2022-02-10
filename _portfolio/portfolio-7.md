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

<img src='/images/tracery.png'>

### Generating Tweets
Using a GPT-2 Model we learned on tweets from Game Twitter Personalities. We implemented our data within a pre-existing GPT-2 Google Colab model. First, we input a single-column csv containing our tweet data. We used a 124M “small” model and carried out 2000 steps, testing different temperatures and using .7 in our final model. This then output a .txt file containing 1000 computer-generated tweets at a time.

<img src='/images/gpt.png'>

### Creating a Twitterbot
- Using Tracery, we were able to create a bot to tweet out our generated tweets
- Created “bot” Twitter Account
- Set to tweet every 6 hours
- Created set of rules to generate game-related Tweets
- Two types: human created (by us) and GPT-2 generated

