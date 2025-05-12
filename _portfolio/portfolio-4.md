--
title: "Women's Emotions Bias: A Multilevel Analysis"
excerpt: "Exploring the Multilevel Structure of Women’s Emotional Expression on Social Media"
collection: portfolio
---------------------

## Introduction

This project explores the multilevel structure of women’s emotional expression on social media, analyzing how emotions propagate from individual users to groups, networks, and society. The study leverages natural language processing, social network analysis, and sentiment analysis to uncover the emotional dynamics within different levels.

## Methodology

* **Multilevel Structure:** The analysis is divided into four levels:

  1. **Individual Level:** Captures personal emotional triggers, expressions, and amplification.
  2. **Group Level:** Examines emotional resonance and collective emotion formation.
  3. **Network Level:** Analyzes cross-group emotional interactions and the influence of opinion leaders.
  4. **Macro Level:** Investigates social norms and the impact of emotional topics in society.
  
## Social Media Tag
 * **Tag Analysis:** The primary goal of Tag Analysis is to identify and quantify the frequency and emotional polarity of specific tags (keywords or hashtags) on social media platforms. We aim to use these tags to provide insights into the topics most likely to influence their emotional states.
  1. **Emotional Tags:** Identifying tags associated with emotional expressions (e.g., #anxiety, #happy, #depressed).
	2. **Topical Tags:** Identifying tags related to specific themes (e.g., #selfcare, #relationship, #career, #mentalhealth).
	3. **Platform-Specific Tags:** Recognizing platform-driven tags (e.g., #ForYou on TikTok, #Explore on Instagram).

* **Data Collection:**

  * Twitter API: Extracting tweets related to women’s emotional topics.
  * Instagram API: Collecting comments and emotional hashtags.
  * Reddit API: Analyzing discussions in women-focused communities.
  * Discord API: Analyzing posts in emotional support groups for women.

* **Emotion Detection and Analysis:**

  * BERT and VADER for sentiment classification.
  * NetworkX and Gephi for social network analysis.
  * Hashtag analysis for emotional topic tracking.


## Conclusion

This study employs a hierarchical model to investigate the impact of social media on women’s emotional well-being, structured across three hierarchical levels: individual characteristics, social media platform attributes, and socio-economic context.  Individual women’s emotional states (e.g., anxiety and depression - tag relats to  #DepressionHelp #Healing #PMDDWarrior ) are nested within social media platforms they use, which are further nested within broader socio-economic environments such as countries or regions. We may consider economic factors as a weight measurement in later tests. 

## Key Considerations and Potential Challenges

	1.	Hierarchical Structure Clarification: It is essential to maintain a clear distinction between the different levels of the model:
	•	Level 1 (Individual): Characteristics of women, including age, education, social media usage patterns, and baseline psychological traits.
	•	Level 2 (Social Media Platform): Platform characteristics, such as algorithm transparency, content type (positive vs. negative), and platform usage patterns.
	•	Level 3 (Socio-Economic Context): Regional-level indicators such as gender equality index, income level, and cultural norms.
	2.	Random and Fixed Effects Specification: Careful consideration is required to distinguish between fixed and random effects:
	3.	Multicollinearity Risks: Given the complex interactions between variables (e.g., social media usage and platform characteristics), the model must account for potential multicollinearity. Regular diagnostic checks (e.g., Variance Inflation Factor, VIF) should be performed to ensure model stability.

## Tools and Tech Used

* **Python:** Natural Language Processing (NLP), Data Collection (Twitter API, Reddit API)
* **R:** Sentiment Analysis, Visualization (ggplot2)
* **QGIS:** Geographic Data Processing and Analysis
* **Gephi:** Social Network Analysis
* **NetworkX:** Network Analysis and Visualization
* **Twint:** Twitter data scraping
* **Hashtagify:** Hashtag Tracking and Analysis
