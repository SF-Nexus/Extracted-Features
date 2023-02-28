# Topic Modeling Output Guide

## LDA Topic Modeling Output

Here is the output from LDA analysis of the Round 3 (Climate Fiction) texts. Prior to analysis, these texts were split into 1000-word "chunks" per chapter and disaggregated. All stopwords and non-English words were removed. 

All 178 topics are visualized below. Access complete list with keywords [here](https://github.com/SF-Nexus/extracted-features/blob/main/data/LDA_output/LDA_topics_keywords_df.csv).

![image](/data/LDA_output/LDA_Topic_Modeling_Viz.png "LDA_Topic_Modeling_Viz")

Access the interactive version of the topic visualization [here](https://htmlpreview.github.io/?https://github.com/SF-Nexus/extracted-features/blob/11c04c3a09137eb6898a8b4d9109c6bd98e7a883/data/LDA_output/LDA_Topics_Visualization.html).

## BERTopic Topic Modeling Output

Here is the output from BERTopic analysis of the Round 3 (Climate Fiction) texts. Prior to analysis, these texts were split into 1000-word "chunks" per chapter, since BERTopic does better with smaller pieces of data. These texts were kept in aggregated form and all non-English words were removed. Stopwords were removed after BERTopic analysis occurred.

[Access list of 68 topics (named manually) here](https://github.com/SF-Nexus/extracted-features/blob/main/data/BERTopic_output/Named_BERTopic_Topics.csv).

### Word Clouds with Most Common Words Per Topic
Topic 6: Street and Vehicles

![image](/data/BERTopic_output/BERTopic_Street_Car_Driving_WordCloud.png "Cars_Word_Cloud")

Topic 17: Disease Outbreak

![image](/data/BERTopic_output/BERTopic_Disease_Outbreak_WordCloud.png "Disease_Word_Cloud")

Topic 27: Desert Landscape Exploration

![image](/data/BERTopic_output/BERTopic_Desert_Landscape_Exploration_WordCloud.png "Desert_Word_Cloud")

Topic 61: Air Pollution

![image](/data/BERTopic_output/BERTopic_Air_Pollution_WordCloud.png "Air_Pollution_Word_Cloud")


### Topic Usage Comparison Between Authors

Topics Used By Brian Aldiss vs. Ursula Leguin

![image](/data/BERTopic_output/BERTopic_Topic_Use_Comparison_Between_Aldiss_Leguin.png "Aldiss_Leguin_Topic_Comparison")

