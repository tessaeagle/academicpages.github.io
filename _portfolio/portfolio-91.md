---
title: "Generative AI Projects"
excerpt: "Two projects completed using generative AI. First, implementing the Wave Function Collapse algorithm to explore the generation of computational constellation art using 77 individual tiles designed in Photoshop. Second, developing a Twitterbot using the [Tracery](tracery.io) text generation and [bot creation](https://cheapbotsdonequick.com/) tool to post GPT-2-generated and expandable grammar content.<br><br><img src='/images/CoverImages/GenAI_Cover.png' alt = 'Design. Generative AI Explorations. Two genAI projects - one text-based and one image-based. Data Visualization, Text Generation, GPT'>"
collection: portfolio
---


## Wave Function Collapse Generated Constellations
Wave Function Collapse is an algorithm that takes an input (bitmap or individual tiles) and generates a similar output (see [here](https://github.com/mxgmn/WaveFunctionCollapse)). As part of a class project in CMPM202, my two teammates and I considered themes we wanted to explore through generative art. We considered trying a Where's Waldo style tileset, but ultimately decided to attempt to generate unique sets of star constellations. 

**Project Goal:** Use WFC and our own tiles to generate unique sets of star constellations. <br>
**Project Year:** Winter 2020

## Project Implementation

We initially attempted to use [Isaac Karth's Python port](https://github.com/ikarth/wfc_2019f) of WFC, but ultimately used the initial C# simple tiles implementation. This implementation takes in a set of tiles and adjacency rules indicating how and where tiles can be placed. Utilizing the Wave Function Collapse algorithm with our own tileset to generate computational art. We created a set of 77 tiles in Photoshop (see below) to attempt to generate randomized constellations using WFC. Each tile contained a combination of joints (circles) to represent stars and arms (lines) to represent the drawing of constellations. Joints could connect to arms or blank tiles, while arms could connect to joints or other arms but not blank tiles, as each constellation end had to be a star.

<img src='/images/wfc2.png'>

Our initial attempts led to straight constellations made up of 90 degree angles (see below figure). We adjusted our tileset to include diagonal lines and joints which allowed us to have constellations made up of combinations of 45 and 90 degree angles. 

<img src='/images/wfc5.png'><br>

Below are the finalized images we were able to generate using WFC. 

<img src='/images/wfc.png'><br>

<img src='/images/wfc3.png'><br>

<img src='/images/wfc4.png'><br>

## GPT-2 Tracery Twitterbot

This project uses GPT-2, an open-source language learning model, to learn on tweets downloaded from popular gamer Twitter accounts. We download and analyzed sentiment expression in tweets by popular gamers and within popular gaming hashtags. These tweets were analyzed for valence, saving positive examples. We then utilize [Tracery](http://tracery.io/), a tool built by Kate Compton to generate text using a generative grammar/JSON. Tracery expands text based on user-inputted nodes.

**Project Goal:** Train a GPT-2 model to learn gamer slang (gamer girls) and create a twitter bot with it combining with tweets generated through the Tracery grammer. <br>
**Project Year:** Winter 2020

### Sentiment Analysis
We downloaded tweets from three prominent gamer twitter accounts (Ninja, Pokimane, and LilyPichu). Using sentiment analysis, we analyzed tweets for emotional valence. We trained a recurrent neural network (RNN) classifier with 800,000 labeled tweets and used this model to separate positive and negative tweets. 

#### Positively Classified Tweets
<img src='/images/posSent.png'>

### Generating Tweets
Using a GPT-2 Model we learned on tweets from Game Twitter Personalities. We implemented our data within a pre-existing GPT-2 Google Colab model. First, we input a single-column csv containing our tweet data. We used a 124M “small” model and carried out 2000 steps, testing different temperatures and using .7 in our final model. The temperature controls for the level of randomness present in the output. Temperatures closer to 1 than 0 choose words with a lesser probability of occuring at that point (e.g., "Do you want to go paint a cheetah?": vs. "Do you want to go get ice cream?". This then output a .txt file containing 1000 computer-generated tweets at a time.

<img src='/images/gpt2.png'>

### Creating a Twitterbot
<img src='/images/tracery.png'>
We used Tracery to create a Twitterbot that was set to tweet every six hours. Tracery is a generative grammar that we used to create rules for our human-generated tweets. The origin component contains a rule and denotes how sentences start and their formatting. Rules contain symbols, from which a set of text used for generation is selected. We then tweeted using Tracery rules and human-generated tweets as well as GPT-2-generated tweets. Certain rules provided text from the GPT-2 tweets. We attempted to make our final Twitter profile appear more like a real gamer profile than a bot. <br>

<img src='/images/magik.png'>

### Creation of a Tracery Twitterbot to randomly post bite-sized motivational fitness and wellbeing tweets every hour

**Project Year:** Fall 2020

<img src='/images/twb.png'>

[@tinyworkoutbot Twitter account](https://twitter.com/tinyworkoutbot)

