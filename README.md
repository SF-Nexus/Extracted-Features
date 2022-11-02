# Extracted Features

Updated September 2022

This repository provides methods for retrieving and analyzing extracted features from textual corpora. Its intended use is to analyze a collection of science fiction texts at Temple University which are currently under copyright. 

## Contents
Along with the readme, this repository contains two folders: 
- **notebooks:** Jupyter and Google Colab notebooks for analyzing extracted features
  - **[1-Text Sectioning & Disaggregation (Colab)](https://github.com/SF-Nexus/Extracted-Features/blob/main/notebooks/1-Text%20Sectioning%20%26%20Disaggregation%20(Colab).ipynb):** Segments and disaggregates (alphabetizes) texts in a corpus based on chapters, chunks of chapters, and chunks of n length
  - **[2-Generating and Evaluating Topic Models (Colab):](https://github.com/SF-Nexus/Extracted-Features/blob/main/notebooks/2-Generating%20and%20Evaluating%20Topic%20Models%20(Colab).ipynb)**  Performs LDA topic modeling on disaggregated corpus using Google Colab
  - **[2-Generating and Evaluating Topic Models (Jupyter Notebook):](https://github.com/SF-Nexus/Extracted-Features/blob/main/notebooks/Generating%20and%20Evaluating%20Topic%20Models%20(Jupyter%20Notebook).ipynb)**  Performs LDA topic modeling on disaggregated corpus using Jupyter Notebook
  - **[3-Complete Pipeline-Text Sectioning, Disaggregation and Topic Modeling.ipynb:](https://github.com/SF-Nexus/Extracted-Features/blob/main/notebooks/3-Complete%20Pipeline-Text%20Sectioning%2C%20Disaggregation%20and%20Topic%20Modeling.ipynb)** Segments and disaggregates, then runs topic modeling on corpus of texts. 
- **data:**  csv file of disaggregated data and sample output from topic modeling code

## Requirements
1. User must be able to run Python through Google Colab and/or a local environment. Download the latest version of Python here: https://www.python.org/downloads/ 
2. Files uploaded for sectioning and disaggregation must be UTF-8 encoded text (.txt) files 
3. CSV uploaded for topic modeling must contain disaggregated texts (ex. https://github.com/SF-Nexus/Extracted-Features/blob/main/data/chapters_sample.csv). Full pipeline from sectioning/disaggregation to topic modeling is available in the folder to streamline the process. 
4. Several parameters are set within the code itself (e.g. chunk size for text sectioning, number of topics, chunk size, iterations, passes for topic modeling). These are explained at more length in the in-code comments. 
