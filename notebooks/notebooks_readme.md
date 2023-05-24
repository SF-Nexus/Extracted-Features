# Notebooks
This folder contains notebooks for cleaning and analyzing extracted features with Python. It is split into two subfolders (Extracting Features and Analyzing Extracted Features) which contain Python and R versions of the code. 

The Extracting Features subfolder contains the following notebooks: 
- **Text Sectioning & Disaggregation:** Segments and disaggregates (alphabetizes) texts in a corpus based on chapters, chunks of chapters, and chunks of n length (R, Jupyter Notebook, and Google Colab versions)
- **BookNLP:** Generates extracted features sets (named entities and supersense tags) using BookNLP (Jupyter Notebook version)

The Analyzing Extracted Features subfolder contains the following notebooks: 
- **Cleaning and Basic Text Analysis:** Methods for cleaning the segmented and disaggregated text files and performing word counts, chapter counts, stopword removal, and other basic frequency calculations and enrichment processes (Jupyter Notebook and Google Colab versions)
- **LDA Topic Modeling:** Performs LDA topic modeling on disaggregated corpus (Jupyter Notebook and Google Colab versions)
- **BERTopic Topic Modeling:** Performs BERTopic topic modeling on aggregated corpus (Jupyter Notebook and Google Colab versions)


