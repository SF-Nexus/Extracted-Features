# Extracted Features Analysis

Updated February 2023

This repository provides methods for retrieving and analyzing extracted features from textual corpora. Its intended use is to analyze a collection of science fiction texts at Temple University which are currently under copyright. 

## Contents
This repository contains two folders: 
- **data:** Data inputs and outputs, including csv file of disaggregated texts and visualizations from topic modeling. 
- **notebooks:** Python notebooks for cleaning and analyzing extracted features. Subfolders (google-colab and jupyter-notebooks) contain Google Colaboratory and Jupyter Notebook versions of the code.

## Requirements
1. User must be able to run Python through Google Colab and/or a local environment. Download the latest version of Python here: https://www.python.org/downloads/ 
2. Files uploaded for sectioning and disaggregation must be UTF-8 encoded text (.txt) files 
3. CSV uploaded for LDA topic modeling must contain disaggregated texts. BERTopic works best with aggregated data from which stopwords have NOT been removed.
4. Several parameters are set within the code itself (e.g. chunk size for text sectioning, number of topics, chunk size, iterations, passes for topic modeling). These are explained at more length in the in-code comments. 
