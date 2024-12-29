# Rebooting Friends: A Data-Driven Blueprint for the Ultimate Reboot

Welcome to the **Rebooting Friends** project! 

## Project Overview

Firstly I used **Pandas** to clean and manipulate the dataset, identifying the most experienced directors and writers of *Friends* based on the number of episodes they contributed to. 

- The most experienced directors are **Gary Halvorson** and **Kevin S. Bright**.
- The most experienced writers (story & teleplay) are **Ted Cohen** and **Andrew Reich**.

But then tried to compare  **Gary Halvorson** and **Kevin S. Bright**  based on the mean_rating of episodes. the average rating of episodes that Gary actually directed was 8.4, but the set of episodes he might have directed with additional opportunities (representing his potential as a director) could have had a higher or lower average rating. By looking at a data set of Friends episodes directed by Gary, we are only looking at a sample from a larger population. there fore i conducted bootstraping estimate each director's mean episode rating in the population based on their mean episode in the sample using bootstrapping. then I computed 99% confidence interval 

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


