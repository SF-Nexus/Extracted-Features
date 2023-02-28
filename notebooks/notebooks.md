# Notebooks
This folder contains notebooks for cleaning and analyzing extracted features with Python. It is split into two subfolders (google-colab and jupyter-notebooks) which contain Google Colaboratory and Jupyter Notebook versions of the code. There are four notebooks in each subfolder, representing the four steps in the text processing and analysis pipeline: 
1. **Text Sectioning & Disaggregation:** Segments and disaggregates (alphabetizes) texts in a corpus based on chapters, chunks of chapters, and chunks of n length
2. **Cleaning and Basic Text Analysis:** Methods for cleaning the segmented and disaggregated text files and performing word counts, chapter counts, stopword removal, and other basic frequency calculations and enrichment processes
3. **LDA Topic Modeling:** Performs LDA topic modeling on disaggregated corpus
4. **BERTopic Topic Modeling:** Performs BERTopic topic modeling on aggregated corpus
