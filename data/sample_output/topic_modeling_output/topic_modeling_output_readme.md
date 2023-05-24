# Topic Modeling Output 

## LDA Topic Modeling Output

Here is the output from LDA analysis of the Round 3 (Climate Fiction) texts. Prior to analysis, these texts were split into 1000-word "chunks" per chapter and disaggregated. All stopwords and non-English words were removed. 

All 178 topics are visualized below.

![image](/data/LDA_output/LDA_Topic_Modeling_Viz.png "LDA_Topic_Modeling_Viz")

Access the interactive version of the topic visualization [here](https://htmlpreview.github.io/?https://github.com/SF-Nexus/extracted-features/blob/11c04c3a09137eb6898a8b4d9109c6bd98e7a883/data/LDA_output/LDA_Topics_Visualization.html).

## BERTopic Topic Modeling Output

Here is the output from BERTopic analysis of the Round 3 (Climate Fiction) texts. Prior to analysis, these texts were split into 1000-word "chunks" per chapter, since BERTopic does better with smaller pieces of data. These texts were kept in aggregated form and all non-English words were removed. Stopwords were removed after BERTopic analysis occurred.

### Word Clouds with Most Common Words Per Topic
Topic 18: Disease Outbreak

![image](data/sample_output/topic_modeling_output/BERTopic_Epidemic_WordCloud.png)

Topic 33: War Command

![image](data/BERTopic_output/BERTopic_War_Command_WordCloud.png)

Topic 47: Energy

![image](data/sample_output/topic_modeling_output/BERTopic_Energy_WordCloud.png)

### Topic Usage Comparison Between Authors

Topics Used By Brian Aldiss vs. Ursula Leguin

![image](data/sample_output/topic_modeling_output/BERTopic_Topic_Use_Comparison_Between_Aldiss_Leguin.png)

### Topic Usage Over Time

Frequency with which authors use topics of interest throughout the 20th century. 
Note: frequency is calculated each time a "chapter/chunk" from a book uses the topic most frequently, so the most frequently used topics might be frequent because of their prevalence across chapters of a particular book rather than across multiple books. This is something to fine-tune in how we build the visualization.

![image](data/sample_output/topic_modeling_output/BERTopic_Topic_Usage_over_Time.png)

