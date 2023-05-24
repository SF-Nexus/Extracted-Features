## Extracting Features README.md

The extracted features notebooks are useful for: 

1) __*Sectioning texts*__

It is useful for many research purposes, such as topic modeling, to break texts into smaller documents.  Such statistical methods  work more reliably, and give more accurate results, when applied to segmented, proportional documents chunked out of longer text files.

The code outputs each chunked section as a series of bag-of-words .txt files (with words re-ordered alphabetically), as well as a single .csv containing each .txt's title and content.

The title of each subsectioned .txt file will be the original title of the raw text file, ending with "ch_1_1_SSExtfeat," with the first number designating the delimited chapter, and the second indicating the subsection. 

2) __*Sub-sectioning the delimited texts*__

Some texts do not have regular delimiters, making sectioning on a delimiter impractical or impossible.  In other instances, long texts may only have a few instances of regular delimiters, resulting in sections that are still longer than desired.  Text data mining methods like topic modeling  work most reliably on sections of text that are roughly the same length - and book chapter length (for example) varies widely between books,  often even within one book.  Sub-sectioning standardizes document length for methods sensitive to this text attribute.

If the 'use_subchapter' argument in the beginning of this code is set to TRUE (as is the default), the code will  perform two steps of analysis.  First, it will section texts based on the common delimiter (exactly as above).  Then, the code will separate longer chapters into subsections of equal length, based on the value of the 'subch_threshold' argument.  Word order is maintained at this point, to ensure that each subsection captures the first, second, third... through nth part of each section.  Short sections/chapters will be kept intact.

Finally, as above, the word order is re-sorted from the order present in the text to alphabetic in order to disagreggate the data for sharing copyrighted corpora.

3) __*Transforming text data into subsectioned "Bags of Words" texts and spreadsheets*__

The functional forms of many text data analysis modeling methods (in particular, methods that work from a term-document-frequency matrix) ignore word order.  Also, while it is illegal to share copyrighted material in its consumable (that is, human-readable) form, it IS legal to share the 'extracted features' of these texts.  

Word counts, presented as a term-document-frequency matrix or as disaggregated (disordered) word tokens (aka "bags of words"), qualify as one of these extracted features.  Therefore, the output of this code can be shared freely for research purposes in instances where the original texts themselves could not be.  This code is ideal for  curation projects focused on analysis of copyrighted text for text data mining / cultural analytics purposes. 

While more advanced forms of extracted features can be produced through similar natural processsing methods methods, we have chosen to focus on producing text files that even a beginner could manipulate for tracking trends in a user-friendly program like Voyant-Tools.

### Additional Directions for Using R Notebook

1) The R code is only compatible with Mac operating systems at this time; sorry if you are using a PC! 

2) Your raw data files must be UTF-8 encoded text (.txt) files, placed in the text_data folder

3) You set three initial parameters within the code itself. These are explained at more length in in-code comments.  They are:  
     a) The text delimiter (a string) (preset to "CHAPTER")
     b) Chunk your delimited sections (each "CHAPTER") into subsections (boolean) (preset to TRUE) (NOTE: this will operate even if your text contains no encoded delimiters)
     c) The subsection size in number of words/tokens (integer) (preset to 1000, this value is ignored if subsection parameter (b) is set to FALSE)

### Using the R Code

1) Follow the instructions above

2) Ensure correct placement of your project folder and proper file format of raw text data as .txt. 

3) Delete old results from bags_of_words and matrix_output folder (to avoid mixing of old and new outputs)

4) Open R script in R Studio, highlight all of the code, and run the entire code.  Outputs are generated and placed automatically
   in the appropriate folders. If these folders do not exist, they will be created for you.
