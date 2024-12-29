# Rebooting Friends: A Data-Driven Blueprint for the Ultimate Reboot

Welcome to the **Rebooting Friends** project! 

## Project Overview

Firstly I used **Pandas** to clean and manipulate the dataset, identifying the most experienced directors and writers of *Friends* based on the number of episodes they contributed to. 

- The most experienced directors are **Gary Halvorson** and **Kevin S. Bright**.
- The most experienced writers (story & teleplay) are **Ted Cohen** and **Andrew Reich**.

But then tried to compare  **Gary Halvorson** and **Kevin S. Bright**  based on the mean_rating of episodes. the average rating of episodes that Gary actually directed was 8.4, but the set of episodes he might have directed with additional opportunities (representing his potential as a director) could have had a higher or lower average rating. By looking at a data set of Friends episodes directed by Gary, we are only looking at a sample from a larger population. there fore i conducted bootstraping estimate each director's mean episode rating in the population based on their mean episode in the sample using bootstrapping. then I computed 99% confidence interval 

In our reboot of *Friends*, I used linear regression techniques to analyze how viewership changed with the number of episodes. By examining various episode counts, I found that excitement among viewers remained high up to 30 episodes, but gradually faded as the sitcom progressed. Based on this analysis, I found that **80 episodes** would be the optimal choice for the reboot, striking a balance between maintaining viewer engagement and delivering a compelling storyline.
[Alt text](reboot_friends/images/lr.png)
## Contributions 🤝

This project was developed as part of my [DSC 10](https://catalog.ucsd.edu/courses/DSC.html) course at UC San Diego. I would like to express my gratitude to the [DSC 10 team](https://dsc10.com/staff/)  for their invaluable guidance throughout this project. They provided essential insights, data sources, and helpful hints that significantly shaped my analysis and kept the project on track.

The DSC 10 team also played a key role in transforming my analysis into a more accessible and user-friendly format. I am extremely grateful for their support and contributions, without which this project would not have been possible.

## References and Data Sources 📖

Below are links to all the resources I used in developing this project. Thanks to DSC 10 team who provided these resources!

- The data for this project is sourced from [Kaggle](https://www.kaggle.com), a platform offering publicly accessible datasets, including those related to TV shows like Friends. The dataset includes details on episodes, dialogue lines, and character emotions.

Dataset URL: [Kaggle Friends Dataset](https://www.kaggle.com/datasets/sujaykapadnis/friends?select=friends.csv)


