# Extracted Features Notebooks

Updated May 2023

This repository contains notebooks for retrieving and analyzing extracted features from textual corpora. Its intended use is to analyze a collection of science fiction texts at Temple University which are currently under copyright. 

## Contents
This repository contains two folders: 
- **notebooks:** Python and R notebooks for retrieving and analyzing ***extracted features***, or non-consumable, disaggregated versions of copyrighted work for research purposes 
- **data:** Sample texts and outputs 

## Requirements
1. User must be able to run Python or R through Google Colab and/or a local environment. Download the latest version of Python here: https://www.python.org/downloads/ Download the latest version of R here: https://posit.co/download/rstudio-desktop/
2. Files uploaded for sectioning and disaggregation must be UTF-8 encoded text (.txt) files 
3. CSV uploaded for LDA topic modeling must contain disaggregated texts. BERTopic works best with aggregated data from which stopwords have NOT been removed.
4. Several parameters are set within the code itself (e.g. chunk size for text sectioning, number of topics, chunk size, iterations, passes for topic modeling). These are explained at more length in the in-code comments. 

## Contributors
**Jeff Antsen:** R notebooks and documentation

**Megan Kane:** Python notebooks and documentation
