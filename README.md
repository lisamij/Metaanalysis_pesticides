This github collect the code and files used for my dissertation.
The goal of the project was to conduct a meta-analysis on the differencial toxicity between active ingredients and pesticides, building on the work of Guy Mercer (GitHub - g-mercer/meta-analysis at ae195f9a4a853445a16fbc57f2a3159861f790a5).
It is separated into 5 phases: Searching, Screening, Retrieving, Extracting and Analysis. 

**1 - Searching**
In this part, I conducted the searches on Web of Science and Scopus, and then compared with the extractions realised by Guy.
I also abstract-title screened 100 papers from Guy's extraction to determine an agreement score. 

**2 - Screening**
In this section, I abstract-title screened the results of the comparison of my search with Guy's.
There is a second file to screen the articles I labelled as maybe during the first screen.

**3 - Retrieving**
There is no code for this part, it is just mostly files. 
The full text tracker file was created by joining recent_included, old_included and no_doi_included.
Articles were put into different categories: reviews, nano, bio, EFSA, etc...
All retrieved pdfs were put in the Articles folder.

**4 - Extracting**
At this point, it was decided to first extract on the "normal" articles first and then on the "EFSA" papers. 
The files full_text_first_batch and full_text_second_batch were filled according to the decisions, with reasons if excluded. 
The Excel files data_extraction_Lisa_X were filled when reading the included articles, and then converted to csv with the name "effect_sizes_included...".
The extraction format that I used was not optimal and was modified later. 
The folder Computing_from_figures contained the extraction from WebPlotDigitalizer and markdowns for the fitting of the dose-response curves. 

**5 - Analysis**
This is the proper meta-analysis. The file Analysis_final.rmd is the one used to produce the final results and figures for my dissertation so it is influenced by some decisions. 
The file Analysis.rmd is the older version, where almost all the dataset is used. Analysis_EFSA.rmd is the analysis of the EFSA dataset.
The files from the precedent section were modified following the implementation of the covariance matrix, leading to the "data_extraction_X_formatted" files. 
Essentially, this modification concerned the columns for the control and test groups, that need to be specified according the formatted documents. 

Most of the time, the output of a section becomes the input of the following one. 
