---
title: "Mental Health App Recommendations via Chatbot"
excerpt: Development of a chatbot system through Botsociety to recommend mental health mobile apps and quickly reduce a large set of apps to a handful of personalized options<br><br><img src='/images/featureChatbot.gif'>"
collection: portfolio
---

## Background
Users of mobile apps for mental health are seeking low-cost, stigma-free solutions that are readily accessible and provide support and treatment recommendations. Apps are not a panacea but may provide help to those without other options. There is a clear need for unbiased information on MH apps and third-party systems can provide this. Current app analysis sites have limitations and finding a suitable app on these sites or the app stores can be overwhelming. Providing users with recommendations can increase the speed of decision making [1], but pior app recommender systems have required user app history to make recommendations [2,3]. Task-oriented conversational agents can interact with customers helping them find items or services more effectively [4].

There are currently a small number of academic websites that conduct expert evaluations of mental health apps, but these are ineffective due to constantly evolving apps making site information obsolete as well as the costs involved in generating expert reviews. These sites allow filtering based on several factors, but do not provide personalized options on a user-by-user basis. We developed two rule-based chatbots for providing mental health app recommendations. 

**Project Goal:** Develop a chatbot system to recommend mental health mobile apps and quickly reduce a large set of apps to a handful of personalized options
**Project Year:** 2020-2021

<img src='/images/ab.png'>

## Chatbot Development
The text-based chatbot prototype, AppBot, was designed using Botsociety, an interface designer for conversational systems. Botsociety provides quick high-fidelity modeling of conversation paths and has multiple integration options (e.g., Slack, Messenger, Google Assistant), including embedding directly into websites. Botsociety allows for integration with Google’s Dialogflow system, which would allow for an NLP-backed chatbot system. With this development environment, we have the option of creating a text-based agent or voice assistant which would make the final system more accessible and flexible for a varied user-base.

Based upon our pilot interviews and app store analysis, we decided on two models: Need-based and feature-based. We developed two chatbots in Botsociety following the need-based and feature-based model (shown above). The feature-based model offered more flexibility and relevance to a broader set of users so we decided on testing this one with out pilot users. The final prototype shown below depicts the deployed chatbot system and an example of the recommended apps.

**Methods used:** Competitive Analysis, Conversational Design, Decision Trees, A/B Testing

<img src='/images/chatbotConvo.png'>


### References
1. Theosaksomo, D., & Widyantoro, D. H. (2019, October). Conversational Recommender System Chatbot Based on Functional Requirement. In 2019 IEEE 13th International Conference on Telecommunication Systems, Services, and Applications (TSSA) (pp. 154-159). IEEE.
2. Davidsson, C. (2010). Mobile application recommender system.
3. Costa-Montenegro, E., Barragáns-Martínez, A. B., & Rey-López, M. (2012). Which App? A recommender system of applications in markets: Implementation of the service for monitoring users’ interaction. Expert systems with applications, 39(10), 9367-9375.
4. Zou, J., Chen, Y., & Kanoulas, E. (2020). Towards Question-based Recommender Systems. arXiv preprint arXiv:2005.14255.
