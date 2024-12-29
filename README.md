# Rebooting Friends: A Data-Driven Blueprint for the Ultimate Reboot

Welcome to the **Rebooting Friends** project! 

### Analyzing the Impact of Directors on Episode Ratings and Viewership in *Friends*

In this analysis, we explore the contributions of the most experienced directors and writers in *Friends*, using **Pandas** for data cleaning and manipulation.

#### Most Experienced Directors and Writers
- The most experienced directors: **Gary Halvorson** and **Kevin S. Bright**.
- The most experienced writers: **Ted Cohen** and **Andrew Reich**.

#### Comparing Gary Halvorson and Kevin S. Bright: Episode Ratings

We compared the **average ratings** of episodes directed by Gary and Kevin:

- Kevin's episodes have an average rating of **8.6**.
- Gary's episodes have an average rating of **8.4**.

To account for potential variability, I used **bootstrapping** to estimate the mean rating for the population of episodes each director could have directed. I also calculated the **99% confidence intervals (CIs)** for the mean ratings.

The results showed that while Kevin's episodes are generally rated higher, there is some overlap in the CIs. This suggests that Gary's episodes could perform just as well under different circumstances.

#### Hypothesis Testing: Are the Ratings of Kevin's and Gary's Episodes Different?

To statistically compare the ratings, I conducted a hypothesis test with the following:

- **Null Hypothesis (H₀)**: The mean rating of Kevin’s episodes equals the mean rating of Gary’s episodes.
- **Alternative Hypothesis (H₁)**: The mean ratings of Kevin’s and Gary’s episodes are different.

The result of the test revealed that **0 does not lie within the confidence interval for the difference in ratings** ([0.0627, 0.4682]). Therefore, we reject the null hypothesis and conclude that Kevin’s episodes are rated significantly higher than Gary’s.

#### Comparing Viewership of Gary and Kevin's Episodes

Applying the same bootstrapping technique to **viewership** data, I found that Kevin’s episodes also attract more views than Gary's, suggesting that Kevin’s episodes perform better both in terms of ratings and viewership.

### Conclusion: Which Director is Better for the Reboot?

Based on these analyses:
- **Kevin S. Bright** directs episodes with higher ratings and more viewership than **Gary Halvorson**.
- While there is overlap in the confidence intervals for episode ratings, Kevin's episodes tend to outperform Gary's.

These insights suggest that involving Kevin in the reboot may lead to higher ratings and greater viewership. However, Gary’s episodes might still perform well under different conditions.

---
### Hypothesis Test: Proportion of Lines Spoken by Male vs. Female Main Characters in *Friends*  👩⚖️🧑

In our analysis of the dataset, we observed that the proportion of lines spoken by male main characters ('Ross Geller', 'Chandler Bing', 'Joey Tribbiani') was approximately 0.51, while the proportion of lines spoken by female main characters ('Rachel Green', 'Monica Geller', 'Phoebe Buffay') was slightly lower at approximately 0.49. These proportions are quite similar but not identical.

To determine whether this difference is due to random chance or if male characters are more likely to speak a greater number of lines throughout the series, we performed a hypothesis test with the following hypotheses:

- **Null Hypothesis (H₀):** Male main characters speak the same number of lines as female main characters throughout the ten seasons of *Friends*.
- **Alternative Hypothesis (H₁):** Male main characters speak more lines than female main characters throughout the ten seasons of *Friends*.

### Test Results:

We obtained a **p-value of 0.0738** from the hypothesis test. Since the p-value is greater than the standard significance level of 0.05, we **fail to reject the null hypothesis**. This means that, based on the data from *Friends*, there is no statistically significant evidence to suggest that male characters speak more lines than female characters over the course of the show.

### Conclusion for Reboot:

Given the lack of significant evidence for a gender-based disparity in line distribution, we have decided to assign an **equal number of lines** to both male and female main characters in our reboot, ensuring gender balance in dialogue throughout the series.

---

### Investigating Character Dynamics through Emotions

To better understand the emotional dynamics between characters in *Friends*, we analyzed sentiment data from the first four seasons of the show. Since we only have sentiment data for certain lines during these seasons, our investigation is based on this subset of the data.

#### Methodology

We applied **Bayes' Theorem** to predict the probability that a line spoken by a particular character falls under one of the following emotional categories:

- **Mad**
- **Joyful**
- **Neutral**
- **Peaceful**
- **Powerful**
- **Sad**
- **Scared**

By leveraging Bayes' Theorem, we were able to compute the likelihood that a given line reflects each of these emotions based on historical data from the show. This approach helped us make probabilistic predictions about the emotions conveyed in the dialogue of each character.

#### Visualizing Character Emotions

After predicting the probabilities for each emotion for the various characters, we created a **visualization of speaker emotions**. This visualization illustrates the **similarities and differences** in the types of emotions each character expresses when speaking. It provides insight into how different characters are emotionally portrayed throughout the first four seasons of the show and how they express various emotions like anger, joy, and sadness.

![Alt Text](reboot_friends/images/emotions.png)

The visualization offers a clear representation of the emotional range and tendencies of each character, which can reveal interesting patterns about their personalities and interactions.

---

### Investigating the Impact of Relationships on Episode Ratings and Viewership in *Friends*

In this section, we explore the relationship between episode ratings, viewership, and the presence of romantic relationships among characters in *Friends*. By performing **permutation testing**, we aim to determine whether certain factors, such as relationships between characters, influence the success of an episode in terms of viewership and ratings.

#### 1. Viewership: First Half vs. Second Half of the Series

We began by comparing the viewership of episodes in the first half of *Friends* (seasons 1-5) to the second half (seasons 6-10). Based on initial observations, we suspected that viewership was higher in the earlier seasons. To test this hypothesis, we performed a **permutation test** with the following hypotheses:

- **Null Hypothesis**: Viewership between the first and second halves of the series does not differ systematically; any observed difference is due to random chance.
- **Alternative Hypothesis**: Viewership of the first half of episodes is significantly higher than that of the second half.

After conducting the permutation test, we found a **p-value of 0.001**, which suggests strong evidence that viewership was indeed higher in the first half of the series compared to the second half. This indicates that the observed difference is statistically significant, and could have implications for how we plan the pacing of episodes in the reboot.

#### 2. Impact of Romantic Relationships on Episode Ratings

Next, we investigated whether episodes where characters are in romantic relationships tend to have higher ratings than those where characters are not in relationships. In *Friends*, there are two key couples:

- **Ross and Rachel**: In a relationship from Season 2, Episode 14 to Season 3, Episode 15.
- **Monica and Chandler**: In a relationship from Season 4, Episode 24 to Season 10, Episode 18 (the end of the show).

We compared episodes featuring these couples to episodes where no characters were in a relationship. The hypotheses for our **permutation test** were:

- **Null Hypothesis**: There is no difference in average episode ratings between episodes with relationships ("Relationship" group) and episodes without relationships ("Single" group).
- **Alternative Hypothesis**: Episodes with characters in relationships have higher ratings, on average, than those without relationships.

The result of the permutation test yielded a **p-value of 0.038**, suggesting that episodes featuring at least two main characters in a romantic relationship tend to have higher ratings. While this doesn't establish a causal link between relationships and higher ratings, it does indicate an association. 

### Implications for the Reboot

- **Viewership**: The significant difference in viewership between the first and second halves of *Friends* suggests that earlier seasons tended to attract more viewers. This insight can help guide decisions about pacing and structure for our reboot.
  
- **Romantic Relationships**: The association between romantic relationships and higher ratings suggests that including relationship storylines in the reboot could help boost episode ratings. However, while the data suggests an association, it doesn't prove causality, so relationship dynamics should be thoughtfully integrated into the plot.

These findings will play a crucial role in shaping the direction of our reboot, as we consider how to balance character relationships, pacing, and plot development to maximize engagement and viewership.

---

### Random Episode Title Generator Inspired by *Friends*

To create unique and entertaining episode titles for our reboot, we developed a tool that generates random episode titles inspired by the format used in *Friends*. In the show, episode titles follow a distinctive pattern, such as *"The One with the Morning After"* or *"The One with the Bullies"*. 

Our tool works by leveraging **n-grams**, a technique in natural language processing where sequences of 𝑛 words are used to generate new text based on previously observed patterns. Specifically, we use the following approach:

- **n-gram model**: We build sequences of words (n-grams) based on the episode titles and generate new titles by predicting each next word.
- **Conditional probability**: For a given value of 𝑛, the tool generates each subsequent word based on the **previous word** in the sequence, using the conditional probability of that word appearing after the word before it.

For example, when using an **n-gram size of 2 (bigrams)**, the tool predicts each next word by considering only the **previous word**. This allows the generation of plausible and catchy titles that resemble the original *Friends* format.

### Example Generated Titles:
- The One with Rachel's Dream
- The One with the Girl Who Hits Joey Speaks French
- The One with the Birth Mother
- The One Where They're Up All the Haste
- The One with the Birth Mother

This tool adds a fun and creative twist to the process of naming episodes and ensures that each generated title feels authentically *Friends*-inspired.

---

### How many episodes?
In our reboot of *Friends*, I used linear regression techniques to analyze how viewership changed with the number of episodes. By examining various episode counts, I found that excitement among viewers remained high up to 30 episodes, but gradually faded as the sitcom progressed. Based on this analysis, I found that **80 episodes** would be the optimal choice for the reboot, striking a balance between maintaining viewer engagement and delivering a compelling storyline.
![Alt text](reboot_friends/images/lr.png)
## Contributions 🤝

This project was developed as part of my [DSC 10](https://catalog.ucsd.edu/courses/DSC.html) course at UC San Diego. I would like to express my gratitude to the [DSC 10 team](https://dsc10.com/staff/)  for their invaluable guidance throughout this project. They provided essential insights, data sources, and helpful hints that significantly shaped my analysis and kept the project on track.

The DSC 10 team also played a key role in transforming my analysis into a more accessible and user-friendly format. I am extremely grateful for their support and contributions, without which this project would not have been possible.

## References and Data Sources 📖

Below are links to all the resources I used in developing this project. Thanks to DSC 10 team who provided these resources!

- The data for this project is sourced from [Kaggle](https://www.kaggle.com), a platform offering publicly accessible datasets, including those related to TV shows like Friends. The dataset includes details on episodes, dialogue lines, and character emotions.

Dataset URL: [Kaggle Friends Dataset](https://www.kaggle.com/datasets/sujaykapadnis/friends?select=friends.csv)


