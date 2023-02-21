# Extracted Features Analysis

Updated February 2023

This repository provides methods for retrieving and analyzing extracted features from textual corpora. Its intended use is to analyze a collection of science fiction texts at Temple University which are currently under copyright. 

## Contents
This repository contains two folders: 
- **notebooks:** Google Colab notebooks for cleaning and analyzing extracted features with Python. A subfolder (jupyter-notebooks) contains Jupyter Notebook versions of the code.
  - **1-Text Sectioning & Disaggregation:** Segments and disaggregates (alphabetizes) texts in a corpus based on chapters, chunks of chapters, and chunks of n length
  - **2-Cleaning and Basic Text Analysis:**  Methods for cleaning the segmented and disaggregated text files and performing word counts, chapter counts, stopword removal, and other basic frequency calculations and enrichment processes.
  - **3-LDA Topic Modeling:**  Performs LDA topic modeling on disaggregated corpus 
  - **4-BERTopic Topic Modeling:** Performs BERTopic topic modeling on disaggregated corpus
- **data:** Data inputs and outputs, including csv file of disaggregated texts and visualizations from topic modeling 

## Requirements
1. User must be able to run Python through Google Colab and/or a local environment. Download the latest version of Python here: https://www.python.org/downloads/ 
2. Files uploaded for sectioning and disaggregation must be UTF-8 encoded text (.txt) files 
3. CSV uploaded for topic modeling must contain disaggregated texts (ex. https://github.com/SF-Nexus/Extracted-Features/blob/main/data/chapters_sample.csv). Full pipeline from sectioning/disaggregation to topic modeling is available in the folder to streamline the process. 
4. Several parameters are set within the code itself (e.g. chunk size for text sectioning, number of topics, chunk size, iterations, passes for topic modeling). These are explained at more length in the in-code comments. 
